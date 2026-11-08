---
title: Ideas
---

# Ideas

Research questions in development. Each page says where the idea stands now and, at the bottom, how it got there.

{% assign ideas = site.ideas | sort: "updated" | reverse %}
{% if ideas.size > 0 %}
<ul class="entries">
{% for i in ideas %}<li><a href="{{ i.url | relative_url }}">{{ i.title }}</a>{% if i.status %} <span class="meta">({{ i.status }}{% if i.updated %}, revised {{ i.updated | date: "%b %Y" }}{% endif %})</span>{% endif %}</li>
{% endfor %}</ul>
{% else %}
Nothing here yet.
{% endif %}
