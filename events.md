---
layout: page
title: Events
permalink: /events/
---

## Regular networking events hosted by RSE-AUNZ
 
We currently have three events:
- [RSE Monash lunch catchup](https://www.eventbrite.co.nz/e/rse-monash-lunch-catchup-tickets-651261549827) every 1st Thursday of the month
- [RSE Parkville lunch catchup](https://www.eventbrite.co.nz/e/rse-parkville-lunch-catchup-tickets-628136371797) every 2nd Thursday of the month
- [RSE Online Networking Event](https://www.eventbrite.co.nz/e/rse-aunz-online-networking-meeting-tickets-628129090017) every 4th Thursday of the month

You can see these events at [the RSE-AUNZ Eventbrite page](https://www.eventbrite.co.nz/o/the-rse-association-of-australia-and-new-zealand-65201929823) and follow.

Want to host a local catchup - please reach out to events@rse-aunz.org.

## Annual conference - the RSE Asia Australia unconference

Every year in September we host a joint online event with [the RSE Asia Association](https://rse-asia.github.io/RSE_Asia/), for more details see [the RSEAA website](https://rseaa.github.io/).

## Events Calendar

This is a monthly calendar of all the events hosted by the RSE-AUNZ community.

<iframe src="https://calendar.google.com/calendar/embed?height=600&wkst=1&ctz=Australia%2FMelbourne&bgcolor=%23ffffff&src=MWRlZjYzM2E5MTZhZmM3NzliNjdhYjBkNjQ1MmM4NTVhMGU0NGJkMTEyN2VlYmNkNjEyM2U5YzY1MGFiYzkxY0Bncm91cC5jYWxlbmRhci5nb29nbGUuY29t&color=%23E4C441" style="border:solid 1px #777" width="800" height="600" frameborder="0" scrolling="no"></iframe>

## Previous events

These are the previous events for the RSE-AUNZ community.

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
