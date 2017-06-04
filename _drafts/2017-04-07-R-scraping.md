---
layout: post
title: R scraping
date: 2017-04-30 16:27:31
disqus: y
share: y
categories: r scrap
tags: r scrap
---

Comandos de **R**.<br>
[Pulsa aquí para ver la documentación completa de R.](https://www.r-project.org){:target="_blank"}

---

### R scraping

```
url <- "http://www.etf.com/channels/spdr-etfs"

library(XML)
x <- XML::readHTMLTable(url, header = T, which = 1, stringsAsFactors = F)
# OR
library(htmltab)
ukLang <- htmltab(doc = url, which = "//th[text() = 'Ability']/ancestor::table")

# Now 'x' is a data.frame
```

---

<a href="https://github.com/mariope/apuntes" target="_blank" class="big-button gray">Get it on GitHub &hearts;</a>

---

### Want more?

Like it? [Tell me](http://twitter.com/mariodevelop){:target="_blank"}.<br/>
Problem? [Use GitHub Issues](https://github.com/mariope/apuntes/issues){:target="_blank"}.
