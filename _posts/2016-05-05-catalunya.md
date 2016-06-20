---
layout: person
title:  "Catalunya Experience"
date:   2016-05-06 09:11:23 +0100
category: supporters
share: true
class: supporters
og: true
supporter: 0
og-type: article
twitter: "@catexperience"
---

{% assign supporter_data = site.data.supporters | where:"id", page.supporter %}
{% assign supporter = supporter_data | first %}
<div class="speaker">
	<div class="photo-wrapper"><img src="/assets/img/sponsors/{{ supporter.logo }}" alt="{{ supporter.name }}" class="img-responsive"></div>
	<ul class="speaker-socials">
		<li><a href="mailto:{{ supporter.email }}"><span class="fa fa-envelope"></span></a></li>
	</ul>
	<h3 class="name"><a href="{{ supporter.url }}">{{ supporter.name }}</a></h3>
	<p class="about text-left">{{ supporter.description}} </p>
</div>