---
layout: person
title:  "Barcelona acogerá una jornada mundial sobre biomimética a mediados de junio"
date:   2016-04-04 09:11:23 +0100
category: newsartiles
share: true
class: newsarticles
og: true
newsarticle: 00
og-type: article
---

{% assign newsarticle_data = site.data.newsarticles | where:"id", page.newsarticle %}
{% assign newsarticle = newsarticle_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="{{ newsarticle.publisher.logo.url }}" alt="{{ newsarticle.publisher.name }}" class="img-responsive" /></div><br/>
	<div class="photo-wrapper rounded"><img src="{{ newsarticle.image.url }}" alt="{{ newsarticle.headline }}" class="img-responsive" /></div>
	<h3 class="name">{{ newsarticle.publisher.name }}</h3>
	<p class="about text-left">{{ newsarticle.description}} </p>
</div>