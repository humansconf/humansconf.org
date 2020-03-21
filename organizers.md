---
layout: page
meta_description: >-
  Meet the organizers of #humansconf
summary: >-
  Meet the organizers of #humansconf
title: Organizers
permalink: /organizers
---

#humansconf is organized by a number of volunteers.

Approach any of us directly with any kind of questions before and during the conference, or write an <a href="mailto:{{ site.email }}">email to the team</a>. We're happy to help!

<ul class="organizers">
  {% for organizer in site.data.organizers %}
  <li>
    <figure>
      {% if organizer.gravatar_digest %}
        <img src="//www.gravatar.com/avatar/{{organizer.gravatar_digest}}?s=200" />
      {% elsif organizer.image_path %}
        <img src="{{organizer.image_path}}" />
      {% endif %}
      <figcaption>
        <a href="https://twitter.com/{{ organizer.twitter_handle }}"><small>{{organizer.name}}</small></a>
      </figcaption>
    </figure>
  </li>
  {% endfor %}
</ul>
