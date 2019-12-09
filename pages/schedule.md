---
layout: default
title: Agenda
permalink: /schedule/
---

<section class="schedule">
  <ul>
    {% for talk in site.talks %}
      <li>
        <p>{{ talk.time }}</p>
        <div>
          {% if talk.desc %}
            <a href="{{ talk.url }}"><h2>{{ talk.title }}</h2></a>
          {% else %}
            <h2>{{ talk.title }}</h2>
          {% endif%}
          {% for speaker in talk.speakers %}
            <p>{{ speaker.name }}</p>
          {% endfor %}
        </div>
      </li>
    {% endfor %}
  </ul>
</section>
