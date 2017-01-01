---
layout: post
title: Crear una web con Jekyll
date: 2017-01-01 10:27:31
disqus: y
share: y
categories: ror jekyll
tags: ror jekyll "Ruby on Rails"
---

Pasos para crear una web con **Jekyll**.<br> en 5 minutos.
[Pulsa aquí para ver la documentación completa de Jekyll.](https://jekyllrb.com/docs/home/){:target="_blank"}

---

### Procedimiento de instalación

Crear una carpeta donde instalar Jekyll:

`$ mkdir folder_jekyll`

`$ cd folder_jekyll`

#### Preparar el entorno de Ruby on Rails

Comprobar primero las versiones de ruby y rails:

```
$  ruby -v
$  rails --version
$  rvm list
$  rvm gemset list
```

Seleccionar la versión de ruby que se quiere utilizar:

`$ rvm use ruby-2.3.1@my_web_rails501 --ruby-version --create`

Instalar la versión de rails que se quiere utilizar:

`$ gem install rails --version 5.0.1`

#### Instalar Jekyll
`$ gem install jekyll bundler`

`$ jekyll new .`

#### Probar la instalación

Arrancar el servidor:

`$ bundle exec jekyll serve --drafts`

Y mirar en el navegador:

(http://localhost:4000/)

Listo! (¡menos de 5 minutos!)

### Aplicar una plantilla (theme)

Lo primero será ver los catálogos de plantillas:

Enorme catálogo free: [http://jekyllthemes.org](http://jekyllthemes.org){:target="_blank"}

De pago y gratuítas: [https://jekyllthemes.io](https://jekyllthemes.io){:target="_blank"}

Sin thumbnails: [github.com/jekyll/](https://github.com/jekyll/jekyll/wiki/Themes){:target="_blank"}



---

<a href="https://github.com/mariope/apuntes" target="_blank" class="big-button gray">Get it on GitHub &hearts;</a>

---

### Want more?

Like it? [Tell me](http://twitter.com/mariodevelop){:target="_blank"}.<br/>
Problem? [Use GitHub Issues](https://github.com/mariope/apuntes/issues){:target="_blank"}.
