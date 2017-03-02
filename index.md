---
layout: page
title: Recent News
excerpt: "Recent PPPS 2019 news sorted by date."
search_omit: true
headline: Welcome to PPPS 2019!
---

{% include conf-about-blurb.html %}

<h1>Recent News</h1>

<ul class="post-list">
{% for post in site.posts limit:3 %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

