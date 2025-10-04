---
layout: default
title: Daily Journal
---

# Daily Journal

My personal journal where I reflect on each day, track progress, and set intentions.

## Entries

{% for entry in site.journal %}
<article class="journal-preview">
    <h3><a href="{{ entry.url }}">{{ entry.title }}</a></h3>
    <p class="date">{{ entry.date | date: "%B %d, %Y" }}</p>
</article>
{% endfor %}

{% if site.journal.size == 0 %}
<p>No journal entries yet. Start by creating your first entry!</p>
<p><a href="/templates/journal-template">Use the journal template</a></p>
{% endif %}
