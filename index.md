---
layout: default
title: Home
---

# Welcome to My Personal Blog

This is my personal space where I share my thoughts, track my gratitude, and maintain my daily journal.

## Latest Blog Posts

{% for post in site.posts limit:5 %}
  - [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

## Recent Gratitude Entries

{% for entry in site.gratitude limit:5 %}
  - [{{ entry.title }}]({{ entry.url }}) - {{ entry.date | date: "%B %d, %Y" }}
{% endfor %}

## Navigation

- [Blog](/blog) - Read my blog posts
- [Gratitude Diary](/gratitude) - My daily gratitude entries
- [Journal](/journal) - My daily journal entries
- [About](/about) - Learn more about me

## Quick Links

- [Create a new gratitude entry](/templates/gratitude-template)
- [Create a new journal entry](/templates/journal-template)
