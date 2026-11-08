---
title: Journal
---

# Journal

Informal, dated entries. Newest first.

{% assign entries = site.journal | sort: "date" | reverse %}
{% if entries.size > 0 %}
<ul class="entries">
{% for e in entries %}<li>{{ e.date | date: "%b %-d, %Y" }}: <a href="{{ e.url | relative_url }}">{{ e.title }}</a></li>
{% endfor %}</ul>
{% else %}
Nothing here yet.
{% endif %}
