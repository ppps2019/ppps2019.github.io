---
layout: page
title: Conference History
excerpt: "History of the ICOPS and Pulsed Power Conferences"
modified: 2017-06-30
---

## PPPS Conference History

Starting in 2001, the IEEE Pulsed Power Conference (PPC) and the IEEE International Conference on Plasma Science (ICOPS) have combined once every six years to become the Pulse Power and Plasma Science Conference. PPPS 2019 brings together the fourth combined conference of the PPC (22<sup>nd</sup>) and ICOPS (46<sup>th</sup>).  

#### ICOPS
{% for conf in site.data.icops %}{{conf.Year}} &mdash; {{conf.Location}}, {{conf.City}} &mdash; <em>{{conf.Chair}}</em> <br> {% endfor %}

#### Pulsed Power Conference
{% for conf in site.data.pulsedpower %}{{conf.Year}} &mdash; {{conf.City}} &mdash; <em>{{conf.Chair}}</em> <br> {% endfor %}


