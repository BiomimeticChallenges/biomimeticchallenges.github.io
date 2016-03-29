---
layout: person
title:  "Nel Hofstra"
date:   2016-03-19 10:44:23 +0100
category: speakers
share: true
class: speakers
og: true
speaker: 00
og-type: article
twitter: "@nelhofstra"
---

{% assign speaker_data = site.data.speakers | where:"id", page.speaker %}
{% assign speaker = speaker_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/speakers/{{ speaker.image }}" alt="{{ speaker.name }}" class="img-responsive"></div>
	<h3 class="name">{{ speaker.name }}</h3>
	<p class="text-alt"><small><strong>{{ speaker.jobTitle }}</strong><br/><a href="{{ speaker.worksFor.url }}" title="{{ speaker.worksFor.name }}">{{ speaker.worksFor.name }}</a></small></p>
	<p class="about text-left">{{ speaker.description}} </p>
</div>