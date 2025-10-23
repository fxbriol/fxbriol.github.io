---
title: "Research Group"
permalink: /group/
author_profile: true
---

I co-lead the [Fundamentals of Statistical Machine Learning](https://fsml-ucl.github.io) research group within UCL Statistical Science with my colleagues [Jeremias Knoblauch](https://jeremiasknoblauch.github.io) and [Alessandro Barp](https://alebarp.github.io). I have the privilege of working with the following great team of researchers:

## Postdoctoral Researchers

<div id="team" class="col-sm-12">

{% assign number_printed = 0 %}
{% for member in site.data.postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive rounded" width="20%" style="float: left; margin-right: 30px" />
  <h3>{{ member.name }}</h3>
  {% if member.website  %}
  <i>{{ member.info }}<br>email: <{{ member.email }}><br>website: <a href="{{ member.website }}">{{ member.website }}</a></i>
  {% else %}
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  {% endif %}
  
  <ul style="overflow: hidden">
  {% if member.number_educ >= 1 %}<li>{{ member.education1 }}</li>{% endif %}
  {% if member.number_educ >= 2 %}<li>{{ member.education2 }}</li>{% endif %}
  {% if member.number_educ >= 3 %}<li>{{ member.education3 }}</li>{% endif %}
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}

{%- comment -%} Close an unpaired final row {%- endcomment -%}
{% if number_printed | modulo: 2 == 1 %}
</div>
{% endif %}

</div> <!-- /#team -->

<div class="clearfix" style="clear: both;"></div>


## PhD Students

<div id="team" class="col-sm-12">

{% assign number_printed = 0 %}
{% for member in site.data.phd_students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive rounded" width="20%" style="float: left; margin-right: 30px" />
  <h3>{{ member.name }}</h3>
  {% if member.website  %}
  <i>{{ member.info }}<br>email: <{{ member.email }}><br>website: <a href="{{ member.website }}">{{ member.website }}</a></i>
  {% else %}
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  {% endif %}
  
  <ul style="overflow: hidden">
  {% if member.number_educ >= 1 %}<li>{{ member.education1 }}</li>{% endif %}
  {% if member.number_educ >= 2 %}<li>{{ member.education2 }}</li>{% endif %}
  {% if member.number_educ >= 3 %}<li>{{ member.education3 }}</li>{% endif %}
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}

{%- comment -%} Close an unpaired final row {%- endcomment -%}
{% if number_printed | modulo: 2 == 1 %}
</div>
{% endif %}

</div> <!-- /#team -->

<div class="clearfix" style="clear: both;"></div>

## Visitors

<div id="visitors" class="col-sm-12">

{% assign number_printed = 0 %}
{% for member in site.data.visitors %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive rounded" width="20%" style="float: left; margin-right: 30px" />
  <h3>{{ member.name }}</h3>
  {% if member.website  %}
  <i>{{ member.info }}<br>email: <{{ member.email }}><br>website: <a href="{{ member.website }}">{{ member.website }}</a></i>
  {% else %}
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  {% endif %}
  
  <ul style="overflow: hidden">
  {% if member.number_educ >= 1 %}<li>{{ member.education1 }}</li>{% endif %}
  {% if member.number_educ >= 2 %}<li>{{ member.education2 }}</li>{% endif %}
  {% if member.number_educ >= 3 %}<li>{{ member.education3 }}</li>{% endif %}
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}
{% endfor %}

{%- comment -%} Close an unpaired final row {%- endcomment -%}
{% if number_printed | modulo: 2 == 1 %}
</div>
{% endif %}

</div> <!-- /#team -->

<div class="clearfix" style="clear: both;"></div>

## Alumni

  * [Masha Naslidnyk](https://mashanaslidnyk.github.io) - PhD on "Scalable kernel-based distances for statistical inference and integration" (2021-2025). Now postdoctoral research fellow at UCL Statistical Science.
  * [Oscar Key](https://oscarkey.github.io) - PhD on "Scalable deep learning and data assimilation" (2020-2025). Now research scientist at Prior Labs.
  * [Kaiyu Li](https://ceciliakaiyu.github.io) - PhD on "Multilevel methods for Monte Carlo integration, with applications to tsunami modelling" (2019-2024). Now research scientist at Comac.
  * [Zhuo Sun](https://jz-fun.github.io) - PhD on "Transfer learning in Monte Carlo and beyond" (2019-2023). Now assistant professor at Shanghai University of Finance and Economics, and previously research scientist at Huawei.

