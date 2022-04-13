---
layout: page
title: assets
description:
---

<h2 class="border-bottom pb-1">Logo</h2>
<h3 class="pt-3">Logo 1</h3>
<div class="row row-cols-2 row-cols-md-3 g-3">
  {% assign logo-1 = site.data.assets.logo.logo-1 | group_by: "img-type" %}
  {% for type in logo-1 %}
  <h6 class="d-block w-100 text-uppercase mb-0">{{ type.name }}</h6>
  {% for logo in type.items %}
  <div class="col">
    <div class="card bg-dark">
      <div class="card-body">
        <img src="{{ logo.img }}" alt="" class="card-img">
      </div>
    </div>
    <small class="lh-1 text-secondary">{{ logo.name }}</small>
  </div>
  {% endfor %}
  {% endfor %}
</div>

<h3 class="pt-3">Logo 2</h3>
<div class="row row-cols-2 row-cols-md-3 g-3">
  {% assign logo-2 = site.data.assets.logo.logo-2 | group_by: "img-type" %}
  {% for type in logo-2 %}
  <h6 class="d-block w-100 text-uppercase mb-0">{{ type.name }}</h6>
  {% for logo in type.items %}
  <div class="col">
    <div class="card bg-light">
      <div class="card-body">
        <img src="{{ logo.img }}" alt="" class="card-img">
      </div>
    </div>
    <small class="lh-1 text-secondary">{{ logo.name }}</small>
  </div>
  {% endfor %}
  {% endfor %}
</div>
