---
layout: default
title: Gratitude Diary
---

# Gratitude Diary

Welcome to my gratitude diary. Here I document the things I'm grateful for each day.

## Entries

{% for entry in site.gratitude %}
<article class="gratitude-preview">
    <h3><a href="{{ entry.url }}">{{ entry.title }}</a></h3>
    <p class="date">{{ entry.date | date: "%B %d, %Y" }}</p>
    {% if entry.mood %}
    <p class="mood">Mood: {{ entry.mood }}</p>
    {% endif %}
</article>
{% endfor %}

{% if site.gratitude.size == 0 %}
<p>No gratitude entries yet. Start by creating your first entry!</p>
<p><a href="/templates/gratitude-template">Use the gratitude template</a></p>
{% endif %}
