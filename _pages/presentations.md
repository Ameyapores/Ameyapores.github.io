---
layout: page
permalink: /presentations/
title: Presentations
nav: true
nav_order: 6
---

{% for entry in site.data.cv %}
  {% if entry.title == "Presentations" %}
    <div class="cv">
      <div class="card mt-3 p-3">
        {% include cv/time_table.html entry=entry %}
      </div>
    </div>
  {% endif %}
{% endfor %}
