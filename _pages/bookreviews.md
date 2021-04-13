---
layout: page
permalink: /bookreviews/
title: book reviews
description: Here are my thoughts on some of my favorite books I've read.
nav: false

social: true
---

Also, a kernel of wisdom that reminds me to read often:

>    "It might be well for all of us to remember that, while differing widely in the various little bits we know, in our infinite ignorance we are all equal." - Karl Popper, Conjectures and Refutations 

PS: This list is quite incomplete, I need to do a better job of updating it, but often I just spend the time reading instead  ¯\\\_(ツ)\_/¯



<div class="bookreviews grid">

  {% assign sorted_bookreviews = site.bookreviews | sort: "importance" %}
  {% for bookreview in sorted_bookreviews %}
  <div class="grid-item">
    {% if bookreview.redirect %}
    <a href="{{ bookreview.redirect }}" target="_blank">
    {% else %}
    <a href="{{ bookreview.url | relative_url }}">
    {% endif %}
      <div class="card hoverable">
        {% if bookreview.img %}
        <img src="{{ bookreview.img | relative_url }}" alt="bookreview thumbnail">
        {% endif %}
        <div class="card-body">
          <h2 class="card-title text-lowercase">{{ bookreview.title }}</h2>
          <p class="card-text">{{ bookreview.description }}</p>
          <div class="row ml-1 mr-1 p-0">
            {% if bookreview.github %}
            <div class="github-icon">
              <div class="icon" data-toggle="tooltip" title="Code Repository">
                <a href="{{ bookreview.github }}" target="_blank"><i class="fab fa-github gh-icon"></i></a>
              </div>
              {% if bookreview.github_stars %}
              <span class="stars" data-toggle="tooltip" title="GitHub Stars">
                <i class="fas fa-star"></i>
                <span id="{{ bookreview.github_stars }}-stars"></span>
              </span>
              {% endif %}
            </div>
            {% endif %}
          </div>
        </div>
      </div>
    </a>
  </div>
{% endfor %}

</div>

