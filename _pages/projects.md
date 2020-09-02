---
layout: page
title: projects
permalink: /projects/
description: A quick rundown of what I've worked on.
nav: true

social: true
---

My research/career interests lie within machine learning and robotics.

Specifically I have worked on several projects:

- [safety analysis for autonomous systems][]{:target="_blank"} 
- [autonomous driving][]{:target="_blank"} 
- [reinforcement learning][]{:target="_blank"}
- [neural network interpretability][]{:target="_blank"}

I also make [android apps][]{:target="_blank"}, and you can view all my projects on my [github profile][]{:target="_blank"}.

If you'd like to collaborate with me on something, please feel free to shoot me an email, I'm always interested in learning something new!

[safety analysis for autonomous systems]: https://rvl.cs.toronto.edu/backwards-reachability/ 
[autonomous driving]: https://github.com/Autonomous-Robotics-UTM/Imitation-Learning-Net/blob/master/Autonomous%20Driving%20Through%20Imitation%20Learning.pdf
[reinforcement learning]: https://github.com/alik-git/Pong-DQN
[neural network interpretability]: https://github.com/alik-git/Feature-Visualization-Notebook




[android apps]: https://play.google.com/store/apps/details?id=com.circuitstudio2016.circuits
[github profile]: https://github.com/alik-git


<!-- <div class="projects grid">

  {% assign sorted_projects = site.projects | sort: "importance" %}
  {% for project in sorted_projects %}
  <div class="grid-item">
    {% if project.redirect %}
    <a href="{{ project.redirect }}" target="_blank">
    {% else %}
    <a href="{{ project.url | relative_url }}">
    {% endif %}
      <div class="card hoverable">
        {% if project.img %}
        <img src="{{ project.img | relative_url }}" alt="project thumbnail">
        {% endif %}
        <div class="card-body">
          <h2 class="card-title text-lowercase">{{ project.title }}</h2>
          <p class="card-text">{{ project.description }}</p>
          <div class="row ml-1 mr-1 p-0">
            {% if project.github %}
            <div class="github-icon">
              <div class="icon" data-toggle="tooltip" title="Code Repository">
                <a href="{{ project.github }}" target="_blank"><i class="fab fa-github gh-icon"></i></a>
              </div>
              {% if project.github_stars %}
              <span class="stars" data-toggle="tooltip" title="GitHub Stars">
                <i class="fas fa-star"></i>
                <span id="{{ project.github_stars }}-stars"></span>
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

</div> -->
