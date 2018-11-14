---
layout: page
title: Welcome to PPPS 2019
excerpt: "PPPS 2019 is the premier international conference dedicated to pulsed power and plasma science."
modified: 2017-02-28
---
 
{% include conf-about-blurb.html %}

### Location

[DoubleTree at the Entrance to Universal Orlando]({{ site.baseurl }}{% link _info_articles/accommodations.md %})\\
5780 Major Blvd. \\
Orlando, FL, USA

### Mini-course: June 22-23, 2019

<div class="gallery-ender"></div>

## PPPS Conference History

Starting in 2001, the IEEE Pulsed Power Conference (PPC) and the IEEE International Conference on Plasma Science (ICOPS) have combined once every six years to become the Pulse Power and Plasma Science Conference. PPPS 2019 brings together the fourth combined conference of the PPC (22<sup>nd</sup>) and ICOPS (46<sup>th</sup>).  Keeping the structure of PPPS 2013, there will be no separation between PPC and ICOPS registrants with all functions and publications open to all attendees.

## Latest News and Information

{% for post in site.posts limit:2 %}
{% if post.id %}
  {% assign title = post.title | markdownify | strip_html %}
{% else %}
  {% assign title = post.title %}
{% endif %}

<div class="entries">
<article class="entry">
  <header class="entry-header">
    <h3 class="entry-title">
      <a href="{{ post.url | relative_url }}" rel="bookmark">{{ title }}</a>
    </h3>
  </header>
  <footer class="entry-meta">
    <ul>
    {% if post.date %}
      <li><span class="icon">{% include icon-calendar.svg %}</span><time class="entry-time" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time></li>
    {% endif %}
    {% if post.read_time %}
      <li><span class="icon">{% include icon-stopwatch.svg %}</span>{% capture read_time %}{% include read-time.html %}{% endcapture %}{{ read_time | strip }}</li>
    {% endif %}
    </ul>
  </footer>
  <div class="entry-excerpt">
    {% if post.excerpt %}
      {{ post.excerpt | markdownify }}
      <p><a href="{{ post.url | relative_url }}" class="more-link">{{ site.data.theme.t.read_more | default: 'Read More' }} <span class="icon icon--arrow-right">{% include icon-arrow-right.svg %}</span></a></p>
    {% endif %}
  </div>
</article>
</div>
{% endfor %}



## Main Contacts

<div class="gallery">
{% assign counter = 0 %}
{% for person_hash in site.data.chairs %}
{% assign counter = counter | plus: 1 %}
{% assign person = person_hash[1] %}
<div markdown="1" class="item">
{% if person.avatar %} ![{{ person.name }} bio photo]({{ site.url }}/images/{{ person.avatar }}){: class="bio-photo"}{% endif %}
**{{ person.position }}**  \\
{% if person.email %}[_{{ person.name }}_](mailto:{{ person.email }}){% else %}_{{ person.name }}_{% endif %}
</div>
{% if counter == 3 %}
<div class="gallery-ender"></div>
{% assign counter = 0 %}
{% endif %}
{% endfor %}
<div class="gallery-ender"></div>



