---
title: "DCLab - Publications"
layout: gridlay
excerpt: "DCLab -- Publications."
sitemap: false
permalink: /publications/
---

# Publications

## Highlights

(For a full list see [below](#full-list) or go to [Google Scholar](https://scholar.google.ch/citations?user=TqxYWZsAAAAJ), [ResearcherID](https://www.researcherid.com/rid/D-7763-2012))

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Full List

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}


## Predictive methods

<div class="col-lg-6 clearfix">
 <div class="well">
  <pubtit>Predict the timing and location of terrorist attacks in the age of big data</pubtit>
  <p><em>Chong Chen and Xun Pang</em></p>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/terr.png" class="img-responsive" width="33%" style="float: left" />
  <p>A new method. We have imaged the doubling of the current noise due to Andreev reflections in a Josephson scanning tunneling microscope. We have imaged the doubling of the current noise due to Andreev reflections in a Josephson scanning tunneling microscope.A new method. We have imaged the doubling of the current noise due to Andreev reflections in a Josephson scanning tunneling microscope. We have imaged the doubling of the current noise due to Andreev reflections in a Josephson scanning tunneling microscope.</p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
 </div>
</div>
