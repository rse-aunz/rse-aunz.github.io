---
layout: page
title: Previous events
permalink: /previous_events
---


# Previous events

These are the previous events involving the RSE_AUNZ community:

{%- for post in site.posts -%}
    {%- if post.tags contains "events" -%}
    	  {%- assign has_events = true -%}
	{%- endif -%}
  {%- endfor -%}

  {%- if has_events -%}
  <table class="w3-table">
    <!--
  	<tr class="w3-headrow">
 		<th><h3>Date</h3></th>
  		<th><h3>Location</h3></th>
  		<th><h3>From</h3></th>
  		<th><h3>To</h3></th>
  	<tr>
  	-->
  	
  {%- assign date_format = site.minima.date_format | default: "%a %-d %b, %Y" -%} 
  {%- assign time_format = "%l:%M %P" -%} 
  {%- for post in site.posts -%}
  
    {%- if post.tags contains "events" -%}
    <tr>
    	<td colspan="3">
			<h3>
				<a class="post-link" href="{{ post.url | relative_url }}">
					{{ post.title | escape }} 
				</a>
			</h3>
			{%- if site.show_excerpts -%}
				{{ post.excerpt }}
			{%- endif -%}
		</td>
    </tr>
    <tr class="lastrow">
		<td>{{ post.location }}</td>
		<td>{{ post.from | date: date_format }}</td>
		<td>
			{{ post.from | date: time_format }}
			{%- if post.to -%}
				&nbsp; - &nbsp;
				{{ post.to | date: time_format }}
			{%- endif -%}
		</td>
	</tr>	

	{%- endif -%}
  {%- endfor -%}
  
{%- else -%}
  	<h3>No events available.</h3>
{%- endif -%}
