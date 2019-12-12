---
layout: default
title: Agenda
permalink: /schedule/
---

<section class="schedule">
  <h1>Agenda</h1>
  <ul class="schedule__table">
    {% for talk in site.talks %}
      {% if talk.desc %}
        <li>
          <div class="schedule__time"><div>{{ talk.time.start }} - {{ talk.time.end }}</div></div>
          <div class="schedule__data">
            <a href="{{ talk.url }}"><h2>{{ talk.title }}</h2></a>
            {% for speaker in talk.speakers %}
              <p class="schedule__author">{{ speaker.name }}</p>
            {% endfor %}
          </div>
        </li>
      {% else %}
        <li>
          <div class="schedule__time"><span>{{ talk.time.start }} - {{ talk.time.end }}</span></div>
          <div class="schedule__data">
            <h3>{{ talk.title }}</h3>
          </div>
        </li>
      {% endif %}
    {% endfor %}
  </ul>
</section>
