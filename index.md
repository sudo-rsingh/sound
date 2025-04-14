---
layout: default
title: Home
---

# Welcome to My Blog

{% raw %}{% for post in site.posts %}
<div class="post">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-date">{{ post.date | date: "%B %d, %Y" }}</p>
    {{ post.excerpt }}
    <p><a href="{{ post.url }}">Continue reading →</a></p>
</div>
{% endfor %}{% endraw %}