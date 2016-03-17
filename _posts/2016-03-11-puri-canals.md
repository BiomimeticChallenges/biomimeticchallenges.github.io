---
layout: person
title:  "Puri Canals"
date:   2016-03-11 09:11:23 +0100
category: advisors
share: true
class: advisors
og: true
advisor: 08
og-type: article
---

{% assign advisor_data = site.data.advisors | where:"id", page.advisor %}
{% assign advisor = advisor_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/advisors/{{ advisor.image }}" alt="{{ advisor.name }}" class="img-responsive"></div>
	<h3 class="name">{{ advisor.name }}</h3>
	<p class="text-alt"><small><strong>{{ advisor.jobTitle }}</strong><br/><a href="{{ advisor.worksFor.url }}" title="{{ advisor.worksFor.name }}">{{ advisor.worksFor.name }}</a></small></p>
	<p class="about text-left">{{ advisor.description}} </p>
	<ul class="advisor-socials">
		<li><a href="mailto:{{ advisor.email }}"><span class="fa fa-envelope"></span></a></li>
	</ul>
</div>