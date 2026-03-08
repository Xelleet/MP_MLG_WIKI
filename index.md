---
layout: default
title: Главная страница
---

# Добро пожаловать в MP MLG Wiki

Здесь собраны все персонажи и локации моего проекта.

## Список статей

{% if site.characters.size > 0 %}
  <ul>
    {% for char in site.characters %}
      <li style="margin-bottom: 10px;">
        <a href="{{ char.url | relative_url }}" style="font-size: 1.2em; font-weight: bold;">{{ char.title }}</a>
        {% if char.intro %}
          <br><small style="color: #555;">{{ char.intro | truncate: 120 }}</small>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
{% else %}
  <p>Статей пока нет. Добавьте файлы в папку <code>_characters</code>.</p>
{% endif %}
