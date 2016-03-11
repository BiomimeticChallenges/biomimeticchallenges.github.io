---
layout: person
title:  "Fira de Barcelona"
date:   2016-03-11 09:11:23 +0100
category: organizers
share: true
class: organizers
og: true
organizer: 00
og-type: article
---

{% assign organizer_data = site.data.organizers | where:"id", page.organizer %}
{% assign organizer = organizer_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/sponsors/{{ organizer.logo }}" alt="{{ organizer.name }}" class="img-responsive"></div>
	<h3 class="name"><a href="{{ organizer.url }}">{{ organizer.name }}</a></h3>
	<p class="text-alt"><small><strong>{{ organizer.jobTitle }}</strong><br/><a href="{{ organizer.worksFor.url }}" title="{{ organizer.worksFor.name }}">{{ organizer.worksFor.name }}</a></small></p>
	<p class="about text-left">{{ organizer.description}} </p>
	<ul class="organizer-socials">
		<li><a href="mailto:{{ organizer.email }}"><span class="fa fa-envelope"></span></a></li>
	</ul>
</div>