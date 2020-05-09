---
layout: page
header_image: header-events.jpg
summary: >-
  We're hosting a series of free online events, to bring together people from all kinds of backgrounds and roles to discuss, share, and celebrate stories of and lessons learnt when humans come together to collaborate and create together.
title: "#humansconf Events"
permalink: /events/
---

<div class="events">
 {% for event in site.events %}
   <div class="event">
       <a href="{{ event.url }}" class="event-link">
         <h2 class="event-title">{{ event.title }}</h2>
       </a>
       <div class="event-date">Date of event: {{ event.event_date | date: "%A, %B %-d, %Y at %R %Z" }}</div>
       <p class="event-excerpt">
         {{ event.excerpt }}
         <a href="{{ event.url }}"><div class="read-more">Read more…</div></a>
       </p>
   </div>
 {% endfor %}
</div>
