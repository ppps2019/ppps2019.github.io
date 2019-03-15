---
layout: page
title: Sponsors
modified: 2019-03-15
navigation_weight: 0.2
---

The 2019 IEEE Pulsed Power and Plasma Science Conference would like to acknowledge the very generous support of our sponsors. These sponsors are:


{% for sponsor_hash in site.data.sponsors %}
{% assign sponsor = sponsor_hash[1] %}
<div markdown="1" class="item" style="margin: auto;text-align: center;">
{% if sponsor.logo %} 
![{{ sponsor.name }} logo]({{ site.url }}/images/{{ sponsor.logo }}){: style="width:60%"}{% endif %}<br>
**{{ sponsor.name }}**  
</div>
{% endfor %}

