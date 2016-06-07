---
layout: person
title:  "Kingfisher redesigned a bullet train"
date:   2016-06-07 08:11:23 +0100
category: videos
share: true
class: videos
og: true
og-type: video
video: 12
twitter: "@worldbiomimetic"
promoter: 00
---


{% assign video_data = site.data.videos | where:"id", page.video %}
{% assign video = video_data | first %}
{% assign promoter_data = site.data.promoters | where:"id", page.promoter %}
{% assign promoter = promoter_data | first %}
<figure class="no-margin margin-bottom-1">
    <div class="embed-container embed-container_{{ video.aspect-ratio }}">
        <video id="teaser" controls preload="auto" poster="{{ video.path }}{{ video.poster }}">
            <source src="{{ video.path }}{{ video.source-webm}}" type='video/webm; codecs="opus,vp9"'>
            <source src="{{ video.path }}{{ video.source-mp4 }}" type='video/mp4; codecs="aac,h264"'>
        </video>
    </div>
    <figcaption>
      <p><small><strong>{{ video.title }}</strong> (more about <a href="{{ promoter.permalink }}">{{ video.author.name }}</a>)</small></p>
    </figcaption>
</figure>

<!--more-->

<p>{{ video.description }}</p>