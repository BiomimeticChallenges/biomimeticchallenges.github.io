---
layout: person
title:  "Zoubeir Azouz Video Support"
date:   2016-05-24 09:11:23 +0100
category: videos
share: true
class: videos
og: true
og-type: video
twitter: "@zoubeirazouz"
video: 1
---

{% assign video_data = site.data.videos | where:"id", page.video %}
{% assign video = video_data | first %}
<figure class="no-margin margin-bottom-1">
    <div class="embed-container embed-container_{{ video.aspect-ratio }}">
        <video id="teaser" controls preload="auto" poster="{{ video.path }}{{ video.poster }}">
            <source src="{{ video.path }}{{ video.source-webm}}" type='video/webm; codecs="vorbis,vp8"'>
            <source src="{{ video.path }}{{ video.source-mp4 }}" type='video/mp4; codecs="aac,h264"'>
        </video>
    </div>
    <figcaption>
      <p><small><strong>{{ video.title }}</strong></small></p>
    </figcaption>
</figure>

<!--more-->

<p>{{ video.description }}</p>