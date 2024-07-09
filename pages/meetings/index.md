---
layout: page
title: Meetings
permalink: /meetings/
has_children: true
has_toc: false
---

<!-- <h2>Next Meeting</h2>
  {% assign all_pages = site.pages %}
  {% assign meetings = all_pages | where: "dir", "/pages/meetings/" %}
  {% assign post = meetings | last %}
  <li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}, {{ post.location }}, {{ post.date }}</a></li>
 -->

<h2>Meetings</h2>

<h3>=== UNDER CONSTRUCTION ===</h3>

<br/>

<ul>
  {% assign all_pages = site.pages %}
  {% assign meetings = all_pages | where: "dir", "/pages/meetings/" %}
  {% assign last_index = meetings.size | minus: 1 %}
  {% assign past_meetings = meetings | slice: 0, last_index %}
  {% for post in past_meetings %}
      <li><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}, {{ post.location }}, {{ post.date }}</a></li>
  {% endfor %}
</ul>
