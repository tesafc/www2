---
layout: page
title: partner
description: tesa fc official partner & apparel.
---

<div class="row row-cols-1 row-cols-md-3 g-3">
  {% assign partner-group = site.data.partner | group_by: "type" %}
  {% for type in partner-group %}
  <h6 class="d-block w-100 fw-bolder text-uppercase mb-0">{{ type.name }}</h6>
  {% for partner in type.items %}
  <div class="col mb-5">
    <div class="card h-100 bg-light">
      <div class="card-body">
        <img src="{{ partner.img }}" alt="" class="card-img">
      </div>
    </div> 
  </div>
  {% endfor %}
  {% endfor %}
</div>
