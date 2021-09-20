---
title: Alle Blogposts
layout: post
noindex: true
---

| Datum | Artikel | Autor |
|---|---|---|
{% for post in site.posts -%}
| <span class='text-gray-400 text-nowrap'>{{ post.date | date: site.minima.date_format }}</span> | [{{ post.title }}]({{ post.url | relative_url }}) | {{ post.author }} |
{% endfor -%}
{: class='table' }
