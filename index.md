---
layout: homepage
title: PAssion Card
description: PAssionCard
image: /images/isomer-logo.svg
permalink: /
notification: As our merchants may be updating their operations/operating hours
  to align with the COVID-19 measures, PAssion Card Members are advised to check
  with the respective merchants for the latest updates.
sections:
  - hero:
      background: /images/hero-banner.png
      dropdown:
        title: Let me see
        options:
          - title: PAssion Card
            url: ""
          - title: PAssion Deals
            url: ""
          - title: PAssion Merchants
            url: ""
          - title: PAssion & The Arts
            url: ""
  - infobar:
      title: Featured
      description: Check out the latest offerings from PAssion Card, right here, right now.
      url: /faq/
  - infopic:
      title: MyPassion app
      description: Experience a world of benefits and convenience at your fingertips
      image: /images/mypassionapp.jpg
      alt: MyPAssion Mobile App
  - infopic:
      title: Get on course towards your PAssion!
      button: Full List of Courses
      url: https://www.onepa.gov.sg/
      image: /images/pacourse.jpg
      alt: Image alt text
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
