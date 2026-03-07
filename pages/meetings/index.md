---
layout: page
title: Meetings
permalink: /meetings/
has_children: true
has_toc: false
nav_order: 4
---
{%- assign all_pages = site.pages -%}
{%- assign meetings = all_pages | where: "grand_parent", "Meetings" | sort: "nav_order" -%}
{%- assign upcoming = meetings | first %}

## Next Meeting

[**{{ upcoming.title }}**]({{ upcoming.url | relative_url }}) — {{ upcoming.location }}, {{ upcoming.date }}

## All Meetings

| Meeting | Location | Date |
|---------|----------|------|
{%- for m in meetings %}
| [{{ m.title }}]({{ m.url | relative_url }}) | {{ m.location }} | {{ m.date }} |
{%- endfor %}
