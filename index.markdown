---
layout: default
---

# Hello, World!

This is my collection of projects I've made over time. And my blog.

### Recent projects

 * [LegacyGPT](https://legacygpt.pavliktt.pp.ua/) (June 3) – old ChatGPT UI (pollinations.ai as API)
 * [dLaunch](https://gitlab.com/pavlik-dev/darklauncher) (May 14) – a very simple launcher
 * [url shortener](https://url.pavliktt.pp.ua/) (April 12) – a link shortening service crafted with care and love by me
 * ~~ChatGPT on Telegram (August 26 2023) – ChatGPT as a Telegram bot~~ (RIP June 1)
 * *[more projects here](projects/)*

## Blog posts

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
