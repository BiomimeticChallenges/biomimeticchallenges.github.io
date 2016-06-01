---
layout: person
title:  "Gala Dinner Inspired By Nature: Nandu Jubany"
date:   2016-05-23 09:11:23 +0100
category: conferences
share: true
class: conferences
og: true
conference: 03
og-type: article
twitter: "@nandujubany"
---

{% assign conference_data = site.data.conferences | where:"id", page.conference %}
{% assign conference = conference_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/speakers/{{ conference.performer.image }}" alt="{{ conference.performer.name }}" class="img-responsive"></div><br/>
	<div class="photo-wrapper rounded"><img src="/assets/img/speakers/{{ conference.performer.image-recipe }}" alt="{{ conference.description-2 }}" class="img-responsive"></div>
	<p class="text-alt"><small><strong>{{ conference.performer.name }}</strong><br/>{{ conference.performer.jobTitle }}</small></p>
	<h3 class="name"><a href="{{ conference.offers.url }}">{{ conference.name }}</a></h3>
	<p class="text-alt"><small>{{ conference.startDate | date: "%B %d %-H:%M, %Y" }} | <strong>{{ conference.location.name }}</strong> | <a href="{{ conference.location.googleMap }}">{{ conference.location.address }}</a></small></p>
	<p class="about text-left">{{ conference.description}} </p>
	<p class="about text-left">{{ conference.description-2}} </p>
	<div class="btns-container">
		<a href="/#inscriptions" class="btn btn-md">SIGN UP TO THE EVENT!</a>
	</div>
</div>