---
layout: default
title: Algebra | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/algebra/
---
<h1>Algebra Content</h1>
<ul class="breadcrumb">
	<li><a href="{{ site.baseurl }}/">Olympiadium</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/algebra/">Algebra</a></li>
</ul>
{% for topic in site.data.algebra_topic_list %}
{% capture topic_name %}{{ topic | first }}{% endcapture %}
{% assign page_topic = site.data.algebra_topic_list[topic_name] %}
  <ul class="actions fit big">
  <li><a href="{{ page.url}}olym-{{ forloop.index | plus:0 }}a" class="button fit big">Olym {{ forloop.index | plus:0 }}A. {{ page_topic.name }}</a></li>
  </ul>
{% endfor %}
