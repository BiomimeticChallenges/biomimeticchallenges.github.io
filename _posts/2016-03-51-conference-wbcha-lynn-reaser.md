---
layout: person
title:  "Conference WBChA: Lynn Reaser"
date:   2016-03-11 09:11:23 +0100
category: conferences
share: true
class: conferences
og: true
conference: 02
og-type: article
---

{% assign conference_data = site.data.conferences | where:"id", page.conference %}
{% assign conference = conference_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/speakers/{{ conference.performer.image }}" alt="{{ conference.performer.name }}" class="img-responsive"></div>
	<p class="text-alt"><small><strong>{{ conference.performer.name }}</strong><br/>{{ conference.performer.jobTitle }}<br/><a href="mailto:{{ conference.perfotrmer.email }}" title="Email to {{ conference.performer.name }}">{{ conference.performer.email }}</a></small></p>
	<h3 class="name"><a href="{{ conference.offers.url }}">{{ conference.name }}</a></h3>
	<p class="text-alt"><small>{{ conference.startDate | date: "%B %d %-H:%M, %Y" }} | <strong>{{ conference.location.name }}</strong> | <a href="{{ conference.location.googleMap }}">{{ conference.location.address }}</a></small></p>
	<p class="about text-left">{{ conference.description}} </p>
</div>