---
layout: default
title: Chemical Principles | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /science-olympiads/lecture-notes/brain-valley-biology/
---
<h1>Brain Valley Biology</h1>
<ul class="breadcrumb">
	<li><a href="{{ site.homeurl }}">Olympiadium</a></li> 
	<li><a href="{{ site.homeurl }}science-olympiads/">Science Olympiads</a></li> 
	<li><a href="{{ site.homeurl }}science-olympiads/lecture-notes/">Lecture Notes</a></li> 
	<li><a href="{{ site.homeurl }}science-olympiads/lecture-notes/brain-valley-biology/">Brain Valley Biology</a></li>
</ul>

{% for topic in site.data.brain_valley_biology_topic_list %}
{% capture topic_name %}{{ topic | first }}{% endcapture %}
{% assign page_topic = site.data.brain_valley_biology_topic_list[topic_name] %}
  <ul class="actions fit big">
  <li><a href="{{ site.baseurl }}{{ page.permalink}}chapter-{{ forloop.index | plus:-1 }}" class="button fit big">{{ forloop.index | plus:-1 }}강. {{ page_topic.name }}</a></li>
  </ul>
{% endfor %}