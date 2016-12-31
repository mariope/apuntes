---
layout: post
title: R - Crear paquetes con devtools
date: 2016-12-30 16:27:31
disqus: y
share: y
categories: r devtools packages
tags: r devtools packages
---

Comandos básicos para crear paquetes con **devtools** en **R**.<br>
[Pulsa aquí para ver la documentación completa de R devtools.](https://cran.r-project.org/web/packages/devtools/devtools.pdf){:target="_blank"}
<br><br>
Ver el libro [R packages by Hadley Wickham](http://r-pkgs.had.co.nz){:target="_blank"}

---

### R switch

RSwitch - is a small GUI that allows you to switch between R versions quickly (if you have multiple versions of R framework installed).
[RSwitch](https://r.research.att.com){:target="_blank"}

### R packrat package

Packrat is a dependency management system for R.
[Packrat doc](https://rstudio.github.io/packrat/){:target="_blank"}

### Create a package with devtools

Install devtools package:

```R
install.packages("devtools")
```

Some basic devtools commands:

```R
devtools::load_all()  	# checks that the packages are installed
devtools::check()	# checks package
devtools::install_github() # install from Github
```

#### Basic package files

Basic packages files:

- DESCRIPTION
- .Rbuildignore
- .gitignore
- README
- NEWS
- CONTRIBUTING
- NAMESPACE
- package_name.R
- functions_name.R
- LICENSE

#### Basic commands

Load functions from local workspace:

```R
devtools::load_all()
```
Install the package and load functions:

```R
devtools::install()	# install from local
devtools::install_github() # install from Github
devtools:: install_bitbucket() # install from Bitbucket
```

To save data with the package:

```R
devtools::use_data(x, internal = TRUE) # to save data
load(“file.rda”) # to load data
```

The safest way to exclude a specific file or directory is to use:

```R
devtools:: use_build_ignore("notes")
```
In the rare case that you do need a bundle, call:

```R
devtools:: build()
```

---

<a href="https://github.com/mariope/apuntes" target="_blank" class="big-button gray">Get it on GitHub &hearts;</a>

---

### Want more?

Like it? [Tell me](http://twitter.com/mariodevelop){:target="_blank"}.<br/>
Problem? [Use GitHub Issues](https://github.com/mariope/apuntes/issues){:target="_blank"}.
