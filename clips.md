---
title: Clips
excerpt: "Select media clips of Laurensius Jeffrey Chandra."
layout: page
permalink: /clips/
id: /clips
---

*I regularly speak with the press about open source, open data, and innovation within government. Below are some highlights:*

<ul id="clips">
{% for clip in site.data.clips | sort: "date" | reverse %}
  <li>
    <a href="{{ clip.url }}" class="title" {% if clip.ignore_check %}data-proofer-ignore="true"{% endif %}>{{ clip.title }}</a><br />
    <small><span class="publication">{{ clip.publication }}</span> — <em>{{ clip.date | date: '%B %d, %Y' }}</em></small>
  </li>
{% endfor %}
</ul>
