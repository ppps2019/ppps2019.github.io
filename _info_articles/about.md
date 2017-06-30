---
layout: page
title: About the Conference
excerpt: "PPPS 2019 is the premier international conference dedicated to pulsed power and plasma science."
modified: 2017-02-28
image:
  feature: hotel.jpg
  credit: DoubleTree by Hilton Hotel
  creditlink: http://doubletree3.hilton.com/en/hotels/florida/doubletree-by-hilton-hotel-at-the-entrance-to-universal-orlando-MCOUNDT/index.html
---

{% include conf-about-blurb.html %}

## Location

[DoubleTree by Hilton Hotel](http://doubletree3.hilton.com/en/hotels/florida/doubletree-by-hilton-hotel-at-the-entrance-to-universal-orlando-MCOUNDT/index.html) \\
At the Entrance to Universal Orlando \\
5780 Major Blvd. \\
Orlando, FL, USA

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

Since 19xx, the IEEE Pulsed Power Conference and the IEEE International Conference on Plasma Science combine once every four years to become the Pulse Power and Plasma Science Conference. This combined conference...

#### ICOPS
{% for conf in site.data.icops %}{{conf.Year}} &mdash; {{conf.Location}}, {{conf.City}} &mdash; <em>{{conf.Chair}}</em> <br> {% endfor %}

#### Pulsed Power Conference
{% for conf in site.data.pulsedpower %}{{conf.Year}} &mdash; {{conf.City}} &mdash; <em>{{conf.Chair}}</em> <br> {% endfor %}


