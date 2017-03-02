---
layout: page
title: Recent News
excerpt: "Recent PPPS 2019 news sorted by date."
search_omit: true
headline: Welcome to PPPS 2019!
---

<div markdown="1">
The **2019 IEEE Pulsed Power and Plasma Science Conference** is the premier international conference dedicated to pulsed power and plasma science, combining the IEEE International Conference on Plasma Science and the IEEE International Pulsed Power Conference.

The conference will be held from 22 June to 28 June, 2019, at the [DoubleTree by Hilton Hotel](http://doubletree3.hilton.com/en/hotels/florida/doubletree-by-hilton-hotel-at-the-entrance-to-universal-orlando-MCOUNDT/index.html) in Orlando, FL, USA.

Sponsored by the [IEEE Nuclear and Plasma Sciences Society](http://ieee-npss.org/).
</div>

<h1>Recent News</h1>

<ul class="post-list">
{% for post in site.posts limit:3 %}
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

