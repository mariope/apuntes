---
layout: post
title: Send knitr html report by SES mail
date: 2017-01-20 16:27:31
disqus: y
share: y
categories: paas r aws ses
tags: paas aws ses r knitr mail
---

How to send knitr html report with base64 images by SES mail!

## Generating html report with knitr
You need a \*.Rmd markdown file with R code to generate the report.

```
#!/usr/bin/env Rscript
library(rmarkdown)
rmarkdown::render("report.Rmd")
```

The output is a html file.

## AWS SES html mail with base64 images
Then read the report.html with `cat`, clean with `xmllint` to get only all the body tag and send it!

```
#!/bin/bash

TO="Email To <to@gmail.com>"
FROM="Email From <from@gmail.com>"
SUBJECT="Hey SES"
MESSAGE="This work!"

date="$(date -R)"
priv_key="$AWS_SECRET_KEY"
access_key="$AWS_ACCESS_KEY"
signature="$(echo -n "$date" | openssl dgst -sha256 -hmac "$priv_key" -binary | base64 -w 0)"
auth_header="X-Amzn-Authorization: AWS3-HTTPS AWSAccessKeyId=$access_key, Algorithm=HmacSHA256, Signature=$signature"
endpoint="https://email.us-east-1.amazonaws.com/"

mime_version="MIME-Version: 1.0"

action="Action=SendEmail"
source="Source=$FROM"
to="Destination.ToAddresses.member.1=$TO"
subject="Message.Subject.Data=$SUBJECT"
xmllint --html --xpath "//body" report.html 2>/dev/null >> report2.html
message="Message.Body.Html.Data="$(cat report2.html)

curl -v -X POST -H "Date: $date" -H "$content_type" -H "$mime_version" -H "$auth_header" --data-urlencode "$message" --data-urlencode "$to" --data-urlencode "$source" --data-urlencode "$action" --data-urlencode "$subject" "$endpoint"
```

Voilà!

---

<a href="https://github.com/mariope/apuntes" target="_blank" class="big-button gray">Get it on GitHub &hearts;</a>

---

### Want more?

Like it? [Tell me](http://twitter.com/mariodevelop){:target="_blank"}.<br/>
Problem? [Use GitHub Issues](https://github.com/mariope/apuntes/issues){:target="_blank"}.
