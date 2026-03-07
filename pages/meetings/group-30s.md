---
layout: page
title: "Meetings 30–39"
parent: Meetings
has_children: true
has_toc: false
nav_order: 4
---

{%- assign group_meetings = site.pages | where: "parent", "Meetings 30–39" | sort: "nav_order" -%}

| Meeting | Location | Date |
|---------|----------|------|
{%- for m in group_meetings %}
| [{{ m.title }}]({{ m.url | relative_url }}) | {{ m.location }} | {{ m.date }} |
{%- endfor %}
