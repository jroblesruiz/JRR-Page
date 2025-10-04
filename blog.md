---
layout: default
title: Blog
---

# Blog Posts

{% for post in site.posts %}
<article class="post-preview">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p class="excerpt">{{ post.excerpt }}</p>
    <a href="{{ post.url }}" class="read-more">Read more &rarr;</a>
</article>
{% endfor %}

{% if site.posts.size == 0 %}
<p>No blog posts yet. Check back soon!</p>
{% endif %}
