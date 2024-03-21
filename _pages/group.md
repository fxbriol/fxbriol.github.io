---
title: "Research Group"
permalink: /group/
author_profile: true
---

## Alumni

  * Dr Zhuo Sun. PhD on "Transfer Learning in Monte Carlo and Beyond" (2019-2023). I was his first supervisor and his second supervisor was Prof. Jinghao Xue. More details available on his website: https://jz-fun.github.io
<br/>

## Current Members

I have the privilege of working with the following great team of researchers:

<div id="team" class="col-sm-12">

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = 0 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive rounded" width="20%" style="float: left; margin-right: 30px" />
  <h3>{{ member.name }}</h3>
  {% if member.website  %}
  <i>{{ member.info }}<br>email: <{{ member.email }}><br>website: <a href="{{ member.website }}">{{ member.website }}</a></i>
  <i></i>
  {% else %}
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  {% endif %}
  
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}
</div>

</div>
