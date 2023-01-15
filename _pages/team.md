---
title: "Maguire Lab - Team"
layout: gridlay
excerpt: "Maguire Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are looking for new enthusiastic and creative PhD students to [join the team]({{ site.url }}{{ site.baseurl }}/jobs)!** 

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}{% if member.github != 0 %}
<a href="{{ member.github }}/"> <i class="fa fa-github" style="color:black; font-size:24px;"></i></a>
{% endif %}
{% if member.twitter != 0 %}
<a href="{{ member.twitter }}/"> <i class="fa fa-twitter" style="color:#0084b4; font-size:24px;"></i></a>
{% endif %}
</h4>

<i>{{ member.info }}<br></i>

  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 | markdownify }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | markdownify }} </li>
  <li> {{ member.education2 | markdownify }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 | markdownify }} </li>
  <li> {{ member.education2 | markdownify }} </li>
  <li> {{ member.education3 | markdownify }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 | markdownify }} </li>
  <li> {{ member.education2 | markdownify }} </li>
  <li> {{ member.education3 | markdownify }} </li>
  <li> {{ member.education4 | markdownify }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 | markdownify }} </li>
  <li> {{ member.education2 | markdownify }} </li>
  <li> {{ member.education3 | markdownify }} </li>
  <li> {{ member.education4 | markdownify }} </li>
  <li> {{ member.education5 | markdownify }} </li>
  {% endif %}

  </ul>
{% if member.info != 0 %}
{{member.project}}
{% endif %}

</div>



{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

# Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/team/alumni/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}{% if member.github != 0 %}
<a href="{{ member.github }}/"> <i class="fa fa-github" style="color:black; font-size:24px;"></i></a>
{% endif %}
{% if member.twitter != 0 %}
<a href="{{ member.twitter }}/"> <i class="fa fa-twitter" style="color:#0084b4; font-size:24px;"></i></a>
{% endif %}
</h4>

<i>{{ member.info }}<br></i>

  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 | markdownify }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | markdownify }} </li>
  <li> {{ member.education2 | markdownify }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 | markdownify }} </li>
  <li> {{ member.education2 | markdownify }} </li>
  <li> {{ member.education3 | markdownify }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 | markdownify }} </li>
  <li> {{ member.education2 | markdownify }} </li>
  <li> {{ member.education3 | markdownify }} </li>
  <li> {{ member.education4 | markdownify }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 | markdownify }} </li>
  <li> {{ member.education2 | markdownify }} </li>
  <li> {{ member.education3 | markdownify }} </li>
  <li> {{ member.education4 | markdownify }} </li>
  <li> {{ member.education5 | markdownify }} </li>
  {% endif %}

  </ul>
{% if member.info != 0 %}
{{member.project}}
{% endif %}

</div>



{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

