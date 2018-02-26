---
date: 2018-02-08 21:56:22
tags: 
- Themes
- - Fix
categories: Hexo
title: Меняем формат даты
---
Заменил в файле **Git\Blog\themes\minos\layout\_partial\archive-post.ejs**

Это:

    <%- partial('post/date', {class_name: 'archive-article-date', date_format: 'MMM D'}) %>

На это:

    <%- partial('post/date', {class_name: 'archive-article-date', date_format: 'DD MMMM'}) %

Далее делаем по аналогии, заглядывая в **[мануал по формате даты](http://momentjs.com/docs/#/displaying/format/)**
<!--more-->
Например, формат архивной даты статьи (править там же)

    <%- partial('post/date', {class_name: 'archive-article-date', date_format: 'DD MMMM YYYY года'}) %>