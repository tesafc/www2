---
layout: page
title: assets
description:
---

<div class="row row-cols-2 g-3">
  {% assign logo-1 = site.data.assets.logo.logo-1 | group_by: "img-type" %}
  {% for type in logo-1 %}
  <h6 class="d-block w-100 text-uppercase mb-0 pt-3">{{ type.name }}</h6>
  {% for logo in type.items %}
  <div class="col">
    <div class="card bg-dark">
      <div class="card-body">
        <img src="{{ logo.img }}" alt="" class="card-img">
      </div>
    </div>
    <small>{{ logo.name }}</small>
  </div>
  {% endfor %}
  {% endfor %}
</div>

<div class="row row-cols-2 g-3">
  {% assign logo-2 = site.data.assets.logo.logo-2 | group_by: "img-type" %}
  {% for type in logo-2 %}
  <h6 class="d-block w-100 text-uppercase mb-0 pt-3">{{ type.name }}</h6>
  {% for logo in type.items %}
  <div class="col">
    <div class="card">
      <div class="card-body">
        <img src="{{ logo.img }}" alt="" class="card-img">
      </div>
    </div>
    <small>{{ logo.name }}</small>
  </div>
  {% endfor %}
  {% endfor %}
</div>
