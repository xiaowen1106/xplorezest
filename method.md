---
title: What I do
layout: landing
description: I listen, reflect what I hear, and ask questions that help you see yourself more clearly.
image: assets/images/pic03.jpg
nav-menu: true
---

<!-- Main -->
<div id="main">

      <!-- One -->
      <section id="one">
        <div class="inner">
                {% for post in site.posts %}
          {% if post.title != 404 %}
          <header class="major">
            <h1>{{ post.title }}</h1>
          </header>
          {% if post.image %}<span class="image main"><img src="{{ site.baseurl }}/{{ post.image }}" alt="" /></span>{% endif %}
          <!-- {% if post.date %}<p>{{ post.date }}</p>{% endif %} -->
          <p>{{ post.description }}</p>
            <ul class="actions">
			        <li><a href="{{ post.url }}" class="button">Read more</a></li>
				</ul>
          {% endif %}
                {% endfor %}
        </div>
      </section>


        <!-- Two -->
        <section id="two">
            <div class="inner">
                <ul class="actions">
                    <li><a href="https://calendly.com/xplorezest/session" class="button next">Book a Free Discovery Call</a></li>
                </ul>
            </div>
        </section>

</div>
