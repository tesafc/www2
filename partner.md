---
layout: page
title: partner
description:
official-partner:
  - name: pok merdeka cell
    img: /assets/img/POK.png
    
  - name: yeni sembako
    img: /assets/img/yeni-sembako.png

  - name: redline
    img: /assets/img/redline.png
---

<div class="row row-cols-1 row-cols-md-3 g-3">
  {% for partner in page.official-partner %}
  <div class="col">
    <div class="card h-100 align-items-center">
      <div class="card-body">
        <img src="{{ partner.img }}" alt="" class="card-img">
      </div>
    </div>
  </div>
  {% endfor %}
</div>
