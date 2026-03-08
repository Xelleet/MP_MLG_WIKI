---
layout: default
title: "Главная - Моя Вики"
---

# Добро пожаловать в мою Вики

ОФИЦИАЛЬНАЯ вики по вселенной MP&MLG
## Список персонажей

{% assign characters = site.pages | where: "dir", "/_characters/" | sort: "title" %}

<ul>
  {% for char in characters %}
    <li><a href="https://xelleet.github.io/MP_MLG_WIKI/{{ char.url }}">{{ char.title }}</a></li>
    <p>test</p>
  {% endfor %}
</ul>

*Примечание: Если список пуст, убедитесь, что файлы лежат в папке _characters.*
