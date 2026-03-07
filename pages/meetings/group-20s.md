---
layout: page
title: "Meetings 20–29"
parent: Meetings
has_children: true
has_toc: false
nav_order: 5
---

{%- assign group_meetings = site.pages | where: "parent", "Meetings 20–29" | sort: "nav_order" -%}

| Meeting | Location | Date |
|---------|----------|------|
{%- for m in group_meetings %}
| [{{ m.title }}]({{ m.url | relative_url }}) | {{ m.location }} | {{ m.date }} |
{%- endfor %}
