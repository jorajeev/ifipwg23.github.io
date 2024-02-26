---
layout: default
title: Members
nav_order: 2
---

<style>
  table, th, td {
    border: none;
    border-collapse: collapse;
    background-color: transparent; /* Ensure no shading */
  }

  table {
    width: 100%;
  }
  td {
    padding: 8px;
    text-align: left;
  }
</style>

<h2>Current Members</h2>

<table>
  <tr>
    {% assign sorted_members = site.data.active_members | sort: 'last_name' %}
    {% assign size_mod = page.items.size | modulo:3 %}
    {% for item in sorted_members %}
      {% assign mod_index = forloop.index0 | modulo:3 %}
      <td>
        {% if item.url | len > 0 %}      
           <a href="{{ item.url }}">{{ item.first_names }} {{ item.last_name }}</a>
	{% else %}
           {{ item.first_names }} {{ item.last_name }}
	{% endif %}
        {% if item.position | len > 0 %}
	( {{ item.position }} )
	{% endif %}
      </td>
      
      {% if mod_index == 2 %}
        </tr><tr>
      {% endif %}
    {% endfor %}
    
    {% if size_mod != 0 %}
      {% for i in (1..3) %}
        {% if size_mod == i %}
          {% assign empty_cells = 3 | minus: i %}
          {% for j in (1..empty_cells) %}
            <td></td>
          {% endfor %}
        {% endif %}
      {% endfor %}
    {% endif %}
  </tr>    
</table>

<h2>Past Members</h2>

<table>
  <tr>
    {% assign sorted_members = site.data.past_members | sort: 'last_name' %}
    {% assign size_mod = page.items.size | modulo:3 %}
    {% for item in sorted_members %}
      {% assign mod_index = forloop.index0 | modulo:3 %}
      <td>
        {% if item.url | len > 0 %}      
           <a href="{{ item.url }}">{{ item.first_names }} {{ item.last_name }}</a>
	{% else %}
           {{ item.first_names }} {{ item.last_name }}
	{% endif %}
      </td>
      
      {% if mod_index == 2 %}
        </tr><tr>
      {% endif %}
    {% endfor %}
    
    {% if size_mod != 0 %}
      {% for i in (1..3) %}
        {% if size_mod == i %}
          {% assign empty_cells = 3 | minus: i %}
          {% for j in (1..empty_cells) %}
            <td></td>
          {% endfor %}
        {% endif %}
      {% endfor %}
    {% endif %}
  </tr>    
</table>

<h2>Deceased Members</h2>

<table>
  <tr>
    {% assign sorted_members = site.data.deceased_members | sort: 'last_name' %}
    {% assign size_mod = page.items.size | modulo:3 %}
    {% for item in sorted_members %}
      {% assign mod_index = forloop.index0 | modulo:3 %}
      <td>
        {% if item.url | len > 0 %}      
           <a href="{{ item.url }}">{{ item.first_names }} {{ item.last_name }}</a>  (d. {{ item.deceased }})
	{% else %}
           {{ item.first_names }} {{ item.last_name }}  (d. {{ item.deceased }})
	{% endif %}
      </td>
      
      {% if mod_index == 2 %}
        </tr><tr>
      {% endif %}
    {% endfor %}
    
    {% if size_mod != 0 %}
      {% for i in (1..3) %}
        {% if size_mod == i %}
          {% assign empty_cells = 3 | minus: i %}
          {% for j in (1..empty_cells) %}
            <td></td>
          {% endfor %}
        {% endif %}
      {% endfor %}
    {% endif %}
  </tr>    
</table>
