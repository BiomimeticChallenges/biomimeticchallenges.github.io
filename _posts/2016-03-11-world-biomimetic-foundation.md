---
layout: person
title:  "World Biomimetic Foundation"
date:   2016-03-11 09:11:23 +0100
category: promoters
share: true
class: promoters
og: true
promoter: 00
og-type: article
---

{% assign promoter_data = site.data.promoters | where:"id", page.promoter %}
{% assign promoter = promoter_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/sponsors/{{ promoter.logo }}" alt="{{ promoter.name }}" class="img-responsive"></div>
	<h3 class="name"><a href="{{ promoter.url }}">{{ promoter.name }}</a></h3>
	<p class="text-alt"><small><strong>{{ promoter.jobTitle }}</strong><br/><a href="{{ promoter.worksFor.url }}" title="{{ promoter.worksFor.name }}">{{ promoter.worksFor.name }}</a></small></p>
	<p class="about text-left">{{ promoter.description}} </p>
	<ul class="promoter-socials">
		<li><a href="mailto:{{ promoter.email }}"><span class="fa fa-envelope"></span></a></li>
	</ul>
</div>