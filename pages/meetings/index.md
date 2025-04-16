---
layout: page
title: Meetings
permalink: /meetings/
has_children: true
has_toc: false
---

{% assign meetings = site.pages | where: "dir", "/pages/meetings/" %}
{% assign latest_meeting = meetings | last %}

<h2>
{% if latest_meeting %}
    Next Meeting: <a href="{{ latest_meeting.url | prepend: site.baseurl }}">
      {{ latest_meeting.title }}, {{ latest_meeting.location }}, {{ latest_meeting.date }}
    </a>
{% endif %}
</h2>

## Past Meetings

### _UNDER CONSTRUCTION_

<br>

<ul>
  {% assign all_pages = site.pages %}
  {% assign meetings = all_pages | where: "dir", "/pages/meetings/" %}
  {% assign last_index = meetings.size | minus: 1 %}
  {% assign past_meetings = meetings | slice: 0, last_index %}
  {% for post in past_meetings %}
      <li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}, {{ post.location }}, {{ post.date }}</a></li>
  {% endfor %}
</ul>
