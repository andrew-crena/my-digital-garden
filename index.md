---
title: Notes
---

# Notes

Working notes from [Andrew Crena](https://andrew-crena.github.io/). **Ideas** are research questions I keep revising, each with a record of how it has changed. The **journal** is informal and dated: reading, conversations, and things I noticed.

## Ideas

{% assign ideas = site.ideas | sort: "updated" | reverse %}
{% if ideas.size > 0 %}
<ul class="entries">
{% for i in ideas limit: 5 %}<li><a href="{{ i.url | relative_url }}">{{ i.title }}</a>{% if i.status %} <span class="meta">({{ i.status }})</span>{% endif %}</li>
{% endfor %}</ul>
{% else %}
Nothing here yet.
{% endif %}

## Recent journal entries

{% assign entries = site.journal | sort: "date" | reverse %}
{% if entries.size > 0 %}
<ul class="entries">
{% for e in entries limit: 5 %}<li>{{ e.date | date: "%b %-d, %Y" }}: <a href="{{ e.url | relative_url }}">{{ e.title }}</a></li>
{% endfor %}</ul>
{% else %}
Nothing here yet.
{% endif %}
