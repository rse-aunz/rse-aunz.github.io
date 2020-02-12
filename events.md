---
layout: page
title: Events
permalink: /events/
---

{%- for post in site.posts -%}
    {%- if post.tags contains "events" -%}
    	  {%- assign has_events = true -%}
	{%- endif -%}
  {%- endfor -%}

  {%- if has_events -%}
  <table class="w3-table">
  	<tr class="w3-headrow">
 		<th><h3>Date</h3></th>
  		<th><h3>Location</h3></th>
  		<th><h3>From</h3></th>
  		<th><h3>To</h3></th>
  	<tr>
  	
  {%- assign date_format = site.minima.date_format | default: "%a %-d %b, %Y" -%} 
  {%- assign time_format = "%l:%M %P" -%} 
  {%- for post in site.posts -%}
  
    {%- if post.tags contains "events" -%}
    <tr>
		<td class="lastrow" rowspan="2">{{ post.from | date: date_format }}</td>
		<td>{{ post.location }}</td>
		<td>{{ post.from | date: time_format }}</td>
		<td>{{ post.to   | date: time_format }}</td>
	</tr>	
    <tr >
    	<td class="lastrow" colspan="3">
			<h3>
				<a class="post-link" href="{{ post.url | relative_url }}">
					{{ post.title | escape }} 
						{%- if site.show_excerpts -%}
						<br/> {{ post.excerpt }}
					{%- endif -%}
				</a>
			</h3>
		</td>
    </tr>
	
	{%- endif -%}
  {%- endfor -%}
  
{%- else -%}
  	<h3>No events available.</h3>
{%- endif -%}
