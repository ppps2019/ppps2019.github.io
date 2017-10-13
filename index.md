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


<div class="gallery-ender"></div>

## Conference Organizing Committee

<div class="gallery">
{% for person_hash in site.data.chairs %}
{% assign person = person_hash[1] %}
<div markdown="1" class="item">
{% if person.avatar %} ![{{ person.name }} bio photo]({{ site.url }}/images/{{ person.avatar }}){: class="bio-photo"}{% endif %}
**{{ person.position }}**  \\
{% if person.email %}[_{{ person.name }}_](mailto:{{ person.email }}){% else %}_{{ person.name }}_{% endif %}
</div>
{% endfor %}
</div>

<div class="gallery-ender"></div>


## PPPS Conference History

Starting in 2001, the IEEE Pulsed Power Conference (PPC) and the IEEE International Conference on Plasma Science (ICOPS) have combined once every six years to become the Pulse Power and Plasma Science Conference. PPPS 2019 brings together the fourth combined conference of the PPC (22<sup>nd</sup>) and ICOPS (46<sup>th</sup>).  Keeping the structure of PPPS 2013, there will be no separation between PPC and ICOPS registrants with all functions and publications open to all attendees.

