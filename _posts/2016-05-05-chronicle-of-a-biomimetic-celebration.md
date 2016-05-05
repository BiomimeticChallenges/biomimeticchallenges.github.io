---
layout: person
title:  "Chronicle of a biomimetic celebration"
date:   2016-05-05 08:11:23 +0100
category: newsarticles
share: true
class: newsarticle
og: true
newsarticle: 12
og-type: article
twitter: "@UOCunescochair"
---

{% assign newsarticle_data = site.data.newsarticles | where:"id", page.newsarticle %}
{% assign newsarticle = newsarticle_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="{{ newsarticle.logo-no-amp }}" alt="{{ newsarticle.publisher.name }}" class="img-responsive" /></div><br/>
	<div class="photo-wrapper rounded"><a href="{{ newsarticle.mainEntityOfPage.id }}"><img src="{{ newsarticle.image.url }}" alt="{{ newsarticle.headline }}" class="img-responsive" /></a></div>
	<h3 class="name">{{ newsarticle.publisher.name }}</h3>
	<p class="text-alt"><small><a href="{{ newsarticle.mainEntityOfPage.id }}"><strong>"{{ newsarticle.headline }}"</strong></a><br/>{{ newsarticle.datePublished | date: '%B %d, %Y' }}</small></p>
	<p class="about text-left">{{ newsarticle.description}} </p>
</div>