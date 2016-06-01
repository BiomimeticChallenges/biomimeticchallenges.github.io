---
layout: person
title:  "Javier Collado Ruano"
date:   2016-03-10 12:44:23 +0100
category: speakers
share: true
class: speakers
og: true
speaker: 01
video: 3
og-type: article
twitter: "@Javier_Collado1"
---

{% assign speaker_data = site.data.speakers | where:"id", page.speaker %}
{% assign speaker = speaker_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/speakers/{{ speaker.image }}" alt="{{ speaker.name }}" class="img-responsive"></div>
	<h3 class="name">{{ speaker.name }}</h3>
	<p class="text-alt"><small><strong>{{ speaker.jobTitle }}</strong><br/><a href="{{ speaker.worksFor.url }}" title="{{ speaker.worksFor.name }}">{{ speaker.worksFor.name }}</a></small></p>
	<p class="about text-left">{{ speaker.description}} </p>
{% assign video_data = site.data.videos | where:"id", page.video %}
{% assign video = video_data | first %}
<figure class="no-margin margin-bottom-1">
    <div class="embed-container embed-container_{{ video.aspect-ratio }}">
        <video id="teaser" controls preload="auto" poster="{{ video.path }}{{ video.poster }}">
            <source src="{{ video.path }}{{ video.source-webm}}" type='video/webm; codecs="opus,vp9"'>
            <source src="{{ video.path }}{{ video.source-mp4 }}" type='video/mp4; codecs="aac,h264"'>
        </video>
    </div>
    <figcaption>
      <p><small><strong>{{ video.title }}</strong></small></p>
    </figcaption>
</figure>
</div>