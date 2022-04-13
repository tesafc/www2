---
layout: page
title: partner
description:
---

<div class="row row-cols-1 row-cols-md-3 g-3">
  {% for partner in site.data.partner | group_by: "type" %}
  <h6>{{ partner.type }}</h6>
  <div class="col">
    <div class="card h-100 d-flex flex-column justify-content-center bg-light">
      <div class="card-body">
        <img src="{{ partner.img }}" alt="" class="card-img">
      </div>
    </div>
  </div>
  {% endfor %}
</div>
