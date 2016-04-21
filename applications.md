---
layout: page
title: Applications
permalink: /applications/
---

This should be our index of applications

{% for application in site.applications %}

  <div class="panel panel-default">
    <div class="panel-heading">
      <a href="{{ application.url | prepend: site.baseurl }}">{{ application.title }}</a>
    </div>
    <div class="panel-body">
      <div class="media">

        <div class="media-left media-middle">
          <a href="{{ application.url | prepend: site.baseurl }}">
            <img class="media-object" src="{{ application.screenshot }}" alt="screenshot for {{ application.title }}" style="width:512px;">
          </a>
        </div>

        <div class="media-body">
          {{ application.content }}
        </div>
      </div>
    </div>
  </div>
{% endfor %}
