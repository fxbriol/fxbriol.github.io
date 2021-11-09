---
title: "Team"
permalink: /team/
author_profile: true
---



## Current Students

I am currently supervising the following great team of PhD students:


<div id="team" class="col-sm-12">

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive rounded" width="5%" style="float: left" />
  <h4>{{ member.name }}</h4>
  {% if member.website  %}
  <i>{{ member.info }}<br>email: <{{ member.email }}><br>website: <a href="{{ member.website }}">{{ member.website }}</a></i>
  <i></i>
  {% else %}
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  {% endif %}
 
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}
</div>
