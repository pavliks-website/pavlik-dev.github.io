---
layout: default
---

<h1 style="text-align:center;">Hello, World!</h1>
I'm an ordinary guy who sometimes codes things. I also like photography too!

  * Bday: Jan 22
  * Preferred programming languages:
    * Golang
    * C++
    * Python
    * C
    * PHP
    * JavaScript
  * Especially like:
    * Retro computing
    * Linux
    * Pineapple on pizza
    * Photography

---

# 🐢 Kogame Translate

<span style="font-size:18px;">The only text translator you'll ever want. And it's free!</span>

<a href="https://github.com/pavlik-dev/kogame-translate" style="font-weight:500;font-size:25px;display:block">GitHub</a>

---

<h1 style="text-align:center;">Blog</h1>

{% assign count = 0 %}
{% for post in site.posts %}
  {% assign date = post.date | date: "%s" | plus: 0 %}
  {% if date < 1704067200 %}
    {% continue %}
  {% endif %}

  {% include post.html post=post %}
  {% assign count = count | plus: 1 %}
  {% if count == 5 %}
    {% break %}
  {% endif %}
{% endfor %}
