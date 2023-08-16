---
title: "hugo"
date: 2023-08-16T10:19:21+03:00
draft: false
---

[hugo](https://github.com/gohugoio/hugo/releases) это быстрый генератор статических сайтов

Я снял [видео](https://youtu.be/x8w9zlGOnGY) о том, как бесплатно

( используя hugo ) развернуть сайт

Для этого вам потребуется

+ установить [git](https://git-scm.com/downloads)

+ зарегистрироваться на сайте https://github.com

### 1. скачиваем [hugo](https://github.com/gohugoio/hugo/releases)

### 2. Создаём папку C:\HUGO и туда переносим то, что скачали

### 3. Настраиваем пути PATH ( смотри [видео](https://youtu.be/x8w9zlGOnGY?t=182) как )

### 4. Выдаём команды в любой папке с именем сайта

*в моём примере ниже мой сайт называется hugo*

hugo new site **hugo**

    cd hugo
    git init
    git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
    echo "theme = 'ananke'" >> hugo.toml
    hugo server

Запускается локальный сервер, открываем его [http://localhost:1313](http://localhost:1313)

Далее ( [смотри видео](https://youtu.be/sAMgA-yn0U8) ) выкладываем наш сайт в интернет

Для этого

+ добавляем новый репозиторий *hugo*

+ копируем ссылку на репозиторий 

в моём случае ссылка выглядит как

 `https://github.com/alex1vere2/hugo.git`

+ **Изменяем файл hugo.toml** в папке сайта

в первой строчке baseURL пишем адрес сайта в виде

baseURL = 'https://ваше_имя.github.io/hugo'

Вот как выглядит у меня файл [hugo.toml](https://raw.githubusercontent.com/alex1vere2/hugo/main/hugo.toml)

    baseURL = 'https://alex1vere2.github.io/hugo'
    languageCode = 'en-us'
    title = 'My New Hugo Site'
    theme = 'ananke'

+ выдаём команды

    git config --global user.name ваше_имя

    git config --global user.email ваша_почта

    git add .

    git commit -m initial

    git remote add origin `тут_ваша_ссылка`

    git push -u origin main

+ заходим на https://github.com

+ открываем репозиторий *hugo*

+ нажимаем Settings - Pages

+ выбираем Source - GitHub Actions

+ нажимаем browse all workflows, ищем hugo и нажимаем **Configure**

+ затем **Commit changes...** и ещё раз **Commit changes**

+ строке About нажимаем на колёсико

+ ставим галочку в строчке *Use your GitHub Pages website*

Нажимаем **Save changes**

Теперь ваш сайт доступен по адресу

[https://alex1vere2.github.io/hugo](https://alex1vere2.github.io/hugo)

где, *alex1vere2* - это ваше имя



