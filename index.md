---
layout: default
title: Konrad Kühne
subtitle: Greetings, my name is Konrad!
introduction: Welcome to a collection of my thoughts
picture: true
---
 <ul>
{% for post in site.posts offset: 0 limit: 5 %}
  <li class="index-posts">
  <div class="index-post">
    <a class="index-post-item" href="{{ post.url }}">
      <h2>{{ post.title }}</h2>
    </a> 
  </div>
  <div class="index-post">
    <small class="index-post-item">{{ post.date | date_to_string }}</small>
  </div>
  </li>
{% endfor %}
</ul>
