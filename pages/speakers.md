---
layout: default
title: Ponentes
permalink: /speakers/
---

<section class="speakers">
  <h1>Ponentes</h1>
  {% for talk in site.talks %}
    {% for speaker in talk.speakers %}
      <div class="speaker">
        <a href="{{ talk.url }}">
          <div class="speaker-pic">
            <div class="speaker-pic-img">
              <img src="{{ '/assets/img/speakers/' | relative_url }}{{ speaker.pic }}">
            </div>
          </div>
        </a>
        <div class="speaker-text">
          <a href="{{ talk.url }}">
            <h2>{{ speaker.name }}</h2>
          </a>
          <p>{{ speaker.headline }}</p>
        </div>
      </div>
    {% endfor %}
  {% endfor %}
</section>
