---
title: PAssion Merchants
permalink: /passion-merchants
date: 2022-01-12
layout: post
description: ""
---

<div class="card">
  {%   for merchant in site.data.merchants   %}
    <a href="{{ merchant.detil-url }}">
      <div class="divFeaturedSmall">
        <img class="featuredImageSmall" src= "{{ merchant.image-url }}" alt="{{ merchant.name }}" />
      </div>
      <div class="cardContent">
        <div class="eventName">{{ merchant.name }}</div>
        <div class="eventTitle">{{ merchant.category }}</div>
      </div>
    </a>
  {% endfor %} 
</div>
