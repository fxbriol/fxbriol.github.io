---
title: "Research Group"
permalink: /group/
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

<br />


I also have honorary PhD students i.e. PhD students with which I work with regularly and mentor, but that are not based at UCL:

* [**Takuo Matsubara**](https://sites.google.com/view/takuomatsubara/home), PhD student in Statistics at Newcastle University and The Alan Turing Institute (since September 2019). Main supervisor: Prof. Chris J. Oates (Newcastle). *Projects*: Bayesian neural networks and Stein discrepancies.


## Past Students doing Research

I have previously supervised a number of students currently doing research:

* [***Johanna Meier***](https://de.linkedin.com/in/johanna-meier-3737a6195), MSc Data Science thesis (UCL, 2020), title: "Scalable Inference for Generative
Models using Quasi-Monte Carlo". Now PhD student at Leibniz Universitat Hannover under the supervision of Prof. Philipp Sibbertsen.
* [**Charline le Lan**](http://csml.stats.ox.ac.uk/people/lelan/), MSc Statistics thesis (Imperial College London, 2018), title: "Neural Networks for Variance Reduction in MCMC". Now PhD student at the University of Oxford under the supervision of Prof. Yee Whye Teh. 
* [**Xiaoyue Xi**](https://www.researchgate.net/profile/Xiaoyue_Xi), MSc Statistics thesis (Imperial College London, 2017), title: "Bayesian Monte Carlo in Computer Graphics". Received best MSc thesis award. Now PhD student at Imperial College under the supervision of Dr. Oliver Ratmann. 
