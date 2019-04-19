---
layout: page
title: Plenary Speakers
excerpt: 
modified: 2019-04-12
---

{% for phash in site.data.plenary %}
{% assign person = phash[1] %}
{::options parse_block_html="true" /}
{% raw %}
<div class="plenary-date">
{% endraw %}
{{ person.date }}
{% raw %}
</div>
{% endraw %}
{% if person.pic %}
![{{ person.name }}]({{ site.url }}/images/plenary/{{ person.pic }}){: class="plenary-bio" alt="{{person.name}}"}
{% endif %} 
### {{person.title}}

__{{person.name}}__<br>
{{person.aff}}

{% if person.abstract %}__Abstract__:<br>
{{person.abstract}}{% endif %}

{% if person.bio %}__Biography__:<br>
{{person.bio}}{% endif %}

{% if person.name == "John Verboncoeur" %}
<br><br><br><br><br><br><br>
{% endif %}

{% endfor %}
