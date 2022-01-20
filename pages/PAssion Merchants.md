---
title: PAssion Merchants
permalink: /passion-merchants
date: 2022-01-12
layout: post
description: ""
---
<ul class="block-grid">
  {%   for merchant in site.data.merchants   %}
  <li class="grid-item">
    <a href="{{ merchant.detail-url }}"><img src= "{{ merchant.image-url }}" alt="{{ merchant.name }}" />
      <h5>{{ merchant.name }}</h5>
      <p>{{ merchant.category }}</p>
			<p>&nbsp;</p>
    </a>
  </li>
  {% endfor %} 
</ul>