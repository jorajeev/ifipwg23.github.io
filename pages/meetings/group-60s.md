---
layout: page
title: "Meetings 60–70"
parent: Meetings
has_children: true
has_toc: false
nav_order: 1
---

{%- assign group_meetings = site.pages | where: "parent", "Meetings 60–70" | sort: "nav_order" -%}

| Meeting | Location | Date |
|---------|----------|------|
{%- for m in group_meetings %}
| [{{ m.title }}]({{ m.url | relative_url }}) | {{ m.location }} | {{ m.date }} |
{%- endfor %}
