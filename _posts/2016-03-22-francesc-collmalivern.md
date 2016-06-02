---
layout: person
title:  "Frnacesc Collmalivern"
date:   2016-03-22 07:11:23 +0100
category: advisors
share: true
class: advisors
og: true
advisor: 10
video: 10
og-type: article
twitter: "@fcollmalivern"
---

{% assign advisor_data = site.data.advisors | where:"id", page.advisor %}
{% assign advisor = advisor_data | first %}
<div class="speaker">
	<div class="photo-wrapper rounded"><img src="/assets/img/advisors/{{ advisor.image }}" alt="{{ advisor.name }}" class="img-responsive"></div>
	<h3 class="name">{{ advisor.name }}</h3>
	<p class="text-alt"><small><strong>{{ advisor.jobTitle }}</strong><br/><a href="{{ advisor.worksFor.url }}" title="{{ advisor.worksFor.name }}">{{ advisor.worksFor.name }}</a></small></p>
	<p class="about text-left">{{ advisor.description}} </p>
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