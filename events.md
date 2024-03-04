---
layout: page
title: Events
permalink: /events/
---


<iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=1&ctz=Australia%2FMelbourne&bgcolor=%23ffffff&src=MWRlZjYzM2E5MTZhZmM3NzliNjdhYjBkNjQ1MmM4NTVhMGU0NGJkMTEyN2VlYmNkNjEyM2U5YzY1MGFiYzkxY0Bncm91cC5jYWxlbmRhci5nb29nbGUuY29t&color=%23E4C441" style="border:solid 1px #777" width="800" height="600" frameborder="0" scrolling="no"></iframe>

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
