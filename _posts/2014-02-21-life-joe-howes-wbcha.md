---
layout: person
title:  "Life"
date:   2014-02-21 05:11:23 +0100
category: videos
share: true
class: videos
og: true
og-type: video
twitter: "@rhythmjoe"
video: 2
---

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
      <p><small><strong>{{ video.title }}</strong>, {{ video.datePublished | date: "%B %d, %Y" }} by {{ video.author.name }} (more about <a href="{{ video.author.sameAs | first }}">{{ video.author.name }}</a> on Vimeo)</small></p>
    </figcaption>
</figure>

<!--more-->

<p>{{ video.description }}</p>