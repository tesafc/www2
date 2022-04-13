---
layout: page
title: partner
description:
---

<div class="row row-cols-1 row-cols-md-3 g-3">
  {% assign partner-group = site.data.partner | group_by: "type" %}
  {% for type in partner-group %}
  <h6>{{ type.name }}</h6>
  {% for partner in type.items %}
  <div class="col">
    <div class="card h-100 d-flex flex-column justify-content-center bg-light">
      <div class="card-body">
        <img src="{{ partner.img }}" alt="" class="card-img">
      </div>
    </div>
  </div>
  {% endfor %}
  {% endfor %}
</div>
