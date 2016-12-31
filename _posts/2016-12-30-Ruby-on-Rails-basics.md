---
layout: post
title: Ruby on Rails basics
date: 2016-12-30 16:27:31
disqus: y
share: y
categories: ror
tags: ror
---

Básicos de **Ruby on Rails**.<br>

- Here you will find pointers to manuals, tutorials and references that will come in handy when you feel like coding in Ruby.
[Ruby, a programmer's best friend.](https://www.ruby-lang.org/en/documentation/){:target="_blank"}
- Getting Started with Rails guide covers getting up and running with Ruby on Rails.
[Rails guides](http://guides.rubyonrails.org/getting_started.html){:target="_blank"}
- Help and documentation for the Ruby programming language.
[Ruby doc](http://ruby-doc.org){:target="_blank"}
- Ruby on Rails API.
[Ruby on Rails API](http://api.rubyonrails.org){:target="_blank"}

---

## Básicos

### Empezando con Ruby on Rails

#### Preparar el entorno para Ruby on Rails

[Install Ruby on Rails on Mac](http://railsapps.github.io/installrubyonrails-mac.html){:target="_blank"}<br><br>

The rails new command generates the default Rails starter app. If you wish, you can use the Rails Composer tool to generate a starter application with a choice of basic features and popular gems.

```
$ rails init .
```

#### Instalar las dependencias

Bundler’sbundle install command reads the Gemfile, then downloads and saves each listed gem to the hidden gem folder.

```
bundle install
```

Bundler provides a bundle update command when we want to replace any gems with newer versions.<br>
Be aware that updating gems can break your application, so only update gems when you have time to test and resolve any issues. You can run bundle outdated to see which gems are available in newer versions.

#### Some useful gems
- better_errors
- cancancan  =>  this authorization gem lets you define what a user can do on your website by using abilities defined in a single place.
- pundit  => m·s moderno que el anterior.
- simple_form
- devise   => authentication
- Kaminari - Pagination
- Ransack - Scoping/Searching/Filtering
- twitter-bootstrap-rails - Frontend
- THE OTHER BASIC FRONTEND - DESDE EL LIBRO
- Searchkick - Intelligent Searching (Nature Language)
- Metamagic - SEO
- RuboCop - Static Code Analyzer, Code Smell
- Brakeman - Static Code Analyzer, Security
- acts-as-taggable-on - For tagging, thereís no need to do it from scratch
- RDiscountor -> adding Markdown to longer text,
- Chronic  -> For date parsing, is pretty amazing and fully featured.
- Paranoia -> In case your users are likely to accidentally delete things, can let your users undo.
- For any kind of content management, I use Active Admin
- For image and file uploads, I always use Paperclip
- Haml (Better Views)
- Compass (Better CSS)
- Has Scope (Collection Filtering)
- Rack SSL Enforcer (HTTPS Redirection)

[Gem selection from hothero](https://github.com/hothero/awesome-rails-gem){:target="_blank"}

#### Bootstrap rails generator app examples:
          1)  None
          2)  1 Col Portfolio
          3)  2 Col Portfolio
          4)  3 Col Portfolio
          5)  4 Col Portfolio
          6)  Bare
          7)  Blog Home
          8)  Business Casual
          9)  Business Frontpage
         10)  Clean Blog
         11)  Full Width Pics
         12)  Heroic Features
         13)  Landing Page
         14)  Modern Business
         15)  One Page Wonder
         16)  Portfolio Item
         17)  Round About
         18)  Shop Homepage
         19)  Shop Item
         20)  Simple Sidebar
         21)  Small Business
         22)  Stylish Portfolio
         23)  The Big Picture
         24)  Thumbnail Gallery
      choose  Enter your selection: 7
---

<a href="https://github.com/mariope/apuntes" target="_blank" class="big-button gray">Get it on GitHub &hearts;</a>

---

### Want more?

Like it? [Tell me](http://twitter.com/mariodevelop){:target="_blank"}.<br/>
Problem? [Use GitHub Issues](https://github.com/mariope/apuntes/issues){:target="_blank"}.
