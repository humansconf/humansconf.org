---
layout: page
header_image: "header-organizers.jpg"
meta_description: >-
  #humansconf is organized by these people
summary: >-
  #humansconf is organized by this group of people
title: Team
permalink: /organizers
---

The humansconf is organized by a number of volunteers.

Approach them with any kind of questions before and during the conference, they will be happy to help.

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
        {{organizer.name}}
      </figcaption>
    </figure>
  </li>
  {% endfor %}
</ul>
