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
	<p><small>(<a target="_blank" title="{{ conference.name }} | Menu" href="/assets/pdf/{{ conference.featured_doc }}"><i class="fa fa-download"></i> the menu</a>)</small></p>
	<p class="text-alt"><small>{{ conference.startDate | date: "%B %d %-H:%M, %Y" }} | <strong>{{ conference.location.name }}</strong> | <a href="{{ conference.location.googleMap }}">{{ conference.location.address }}</a></small></p>
	<div class="btns-container">
		<p>Enjoy the experience!</p>
		<a href="https://www.eventbrite.es/e/entradas-1st-world-biomimetic-challenges-and-conscience-23980115170" class="btn btn-md">Buy now!</a>
		<p><small>(you will be redirected to our partner <strong>EventBrite</strong> in order to get your ticket)</small></p>
	</div>
	<hr/>
	<p class="about text-left">{{ conference.description}} </p>
</div>