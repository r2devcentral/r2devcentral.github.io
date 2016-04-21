---
layout: page
title: APIs
permalink: /apis/
---

This should be our index of apis

{% for api in site.apis %}

  <div class="panel panel-default">
    <div class="panel-heading">
      <a href="{{ api.url | prepend: site.baseurl }}">{{ api.title }}</a>
    </div>
    <div class="panel-body">
      {{ api.content }}
    </div>
  </div>
{% endfor %}
