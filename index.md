---
layout: page
title: 世界美好与你环环相扣 ～～～～～ 主页
---
## 近期分享

{% for post in site.posts limit:5 %}

- [{{ post.title }}]({{ post.url }}), *{{ post.date | date_to_string }}*

{% if post.description %}

  > {{ post.description }}

{% endif %}

{% endfor %}

- [更多生活分享…](/archive)

{% for tag in site.index.showtag %}

## {{ tag }}

{% for post in site.tags[tag] %}

- [{{ post.title }}]({{ post.url }})

{% if post.description %}

  > {{ post.description }}

{% endif %}

{% endfor %}

{% endfor %}

<a href ="">兄弟连</a>