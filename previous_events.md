---
layout: page
title: Previous events
permalink: /previous_events
---

These are the previous events involving the RSE_AUNZ community:

<div class="home">
	<ul class="post-list">
		{%- for post in site.posts -%}
			{%- if post.tags contains "events" -%}
				<li>
					{%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
					<span class="post-meta">{{ post.date | date: date_format }}</span>
					<h3>
						<a class="post-link" href="{{ post.url | relative_url }}">
							{{ post.title | escape }}
						</a>
					</h3>
					{%- if site.show_excerpts -%}
						{{ post.excerpt }}
					{%- endif -%}
				</li>
			{%- endif -%}
		{%- endfor -%}
	</ul>
</div>
