---
layout: post
title: Initiatives
published: true
---

<!-- {{ page.title }} Section -->
<section id="initiatives" class="content-section text-center">
  <div id="map"></div>
  <h2>Initiatives</h2>

<div class="events">
  {% for initiative in site.data.initiatives %}
  {% if initiative.published == true %}
    <div class="event">
      <h3><a href="{{ initiative.url }}" alt="link to initiative"><img src='{{ initiative.logo }}' alt='initiative logo' style="width:120px"></a></h3>
      <h5>{{ initiative.freq }}</h5>
      <p class="description">{{ initiative.description }}<br/>
      </p>
      <h4>{{ initiative.more }}</h4>
    </div>
  {% endif %}
  {% endfor %}
</div>

</section>