---
layout: default
title: "Главная - Моя Вики"
---

# Добро пожаловать в мою Вики

Здесь собраны все персонажи и лор моего проекта.

## Список персонажей

{% assign characters = site.pages | where: "dir", "/_characters/" | sort: "title" %}

<ul>
  {% for char in characters %}
    <li><a href="{{ char.url }}">{{ char.title }}</a></li>
  {% endfor %}
</ul>

*Примечание: Если список пуст, убедитесь, что файлы лежат в папке _characters.*