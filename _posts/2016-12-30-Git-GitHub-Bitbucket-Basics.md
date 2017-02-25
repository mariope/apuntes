---
layout: post
title: Git/GitHub/Bitbucket basics
date: 2016-12-30 16:27:31
disqus: y
share: y
categories: git saas
tags: git github bitbucket git-start saas "version control"
---

Comandos básicos para manejar el control de versiones con **Git**,
y también para los repositorios remotos **GitHub** y **Bitbucket**.<br>
[Pulsa aquí para ver la documentación completa de Git.](https://git-scm.com/book/es/v1){:target="_blank"}

---

### Crear el repositorio local

``$ git init .``

---

### Clonar un repositorio Git

```bash
$ cd ~/workspace

$ git clone https://github.com/RailsApps/learn-rails.git

$ cd learn-rails

$ bundle install --without production
```

---

### Preparar ficheros para la copia

Preparar un fichero (staged):

``$ git add file.txt``

Preparar todos los ficheros:  

``$ git add -A``

---

### Añadir al repositorio local todos los ficheros preparados(staged).

``$ git commit -m “comment in present”``

Para hacer un commit añadido al anterior por si se ha olvidado algo:

``$ git commit —-amend``

---

### Comandos para comprobar estado e histórico de logs

The git syntax works like this: program | action | destination.

``$ git status``

``$ git log``

``$ git log --oneline``

---

### Configurar repositorio remoto

``$ git remote show origin``

``$ git remote add origin https://github.com/mariope/learnrails.git``

``$ git remote add origin git@bitbucket.org:mariope/learnrails.git``

``$ git remote rm origin``

---

### Subir a repositorio remoto

``$ git push -u origin master``

``$ git push -u origin --all # pushes up the repo and its refs for the first time``

``$ git push origin --tags # pushes up any tags``

``$ git push heroku``

---

### Resetear últimos cambios

The Git command `git reset -hard HEAD` discards any changes you’ve made since the most recent commit.

``$ git reset --hard HEAD``

---

### Crear y manejar tracks

Se crea el track:

``$ git checkout -b track1``

Se cambia al track principal (master) y se fusiona:

```
$ git checkout master

$ git merge track1
```

### Working with tags

```
$ git tag -a v1.4 -m "my version 1.4"
$ git tag
$ git tag -l "v1.8.5*"
$ git show v1.4
# By default, the git push command doesn’t transfer tags to remote servers.
# You will have to explicitly push tags to a shared server after you have created them.
$ git push origin v1.5
```

---

<a href="https://github.com/mariope/apuntes" target="_blank" class="big-button gray">Get it on GitHub &hearts;</a>

---

### Want more?

Like it? [Tell me](http://twitter.com/mariodevelop){:target="_blank"}.<br/>
Problem? [Use GitHub Issues](https://github.com/mariope/apuntes/issues){:target="_blank"}.
