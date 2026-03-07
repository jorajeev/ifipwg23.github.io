---
layout: page
title: "Meetings 10–19"
parent: Meetings
has_children: true
has_toc: false
nav_order: 6
---

{%- assign group_meetings = site.pages | where: "parent", "Meetings 10–19" | sort: "nav_order" -%}

| Meeting | Location | Date |
|---------|----------|------|
{%- for m in group_meetings %}
| [{{ m.title }}]({{ m.url | relative_url }}) | {{ m.location }} | {{ m.date }} |
{%- endfor %}
