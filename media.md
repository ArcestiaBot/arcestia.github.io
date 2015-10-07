---
layout: default
permalink: /Clips/
---
<ul class="posts">
{% for page in site.media %}
  <li class="post">
    <div class="row">
        <div class="col-sm-9">
            <a href="{{ url_base }}{{ page.url }}">{% include smartify text=page.title %}</a>
        </div>
        <div class="col-sm-3 date">
            {{ page.date | date: '%B %d, %Y' }}
        </div>
    </div>
  </li>
{% endfor %}
</ul>
