---
layout: default
title: Ponentes
permalink: /speakers/
---

<section class="speakers">
  <h1>Ponentes</h1>
  {% for talk in site.talks %}
    {% for speaker in talk.speakers %}
      <a href="{{ talk.url }}">
        <div class="speaker">
          <div class="speaker-pic">
            <div class="speaker-pic-img">
              <img src="{{ '/assets/img/speakers/' | relative_url }}{{ speaker.pic }}">
            </div>
          </div>
          <div class="speaker-text">
            <h2>{{ speaker.name }}</h2>
            <p>{{ speaker.headline }}</p>
          </div>
        </div>
      </a>
    {% endfor %}
  {% endfor %}
</section>
