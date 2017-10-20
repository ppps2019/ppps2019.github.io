---
layout: page
title: Organizing Committee
modified: 2017-06-30
---
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


{% assign counter = 0 %}
{% for person_hash in site.data.organizers %}
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


</div>

<div class="gallery-ender"></div>