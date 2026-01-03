---
layout: page
permalink: /awards/
title: Awards
nav: true
nav_order: 5
---

{% for entry in site.data.cv %}
  {% if entry.title == "Honors and Awards" %}
    <div class="cv">
      <div class="card mt-3 p-3">
        <h3 class="card-title font-weight-medium">{{ entry.title }}</h3>
        <div>
          {% include cv/time_table.html entry=entry %}
        </div>
      </div>
    </div>
  {% endif %}
{% endfor %}
