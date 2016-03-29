---
layout: person
title:  "LOU Comunicació"
date:   2016-03-11 09:11:23 +0100
category: collaborators
share: true
class: collaborators
og: true
collaborator: 04
og-type: article
---

{% assign collaborator_data = site.data.collaborators | where:"id", page.collaborator %}
{% assign collaborator = collaborator_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/sponsors/{{ collaborator.logo }}" alt="{{ collaborator.name }}" class="img-responsive"></div>
	<ul class="speaker-socials">
		<li><a href="mailto:{{ collaborator.email }}"><span class="fa fa-envelope"></span></a></li>
	</ul>
	<h3 class="name"><a href="{{ collaborator.url }}">{{ collaborator.name }}</a></h3>
	<p class="about text-left">{{ collaborator.description}} </p>
</div>