---
layout: page
title: Community Knowledge
permalink: /knowledge/
---

| Topic  | Mailing list URL | Discussion Summary |
| --------  | ------------------- | --------------------- |
| Where to submit code/ research software for review| [For members to continue in the forum](https://groups.google.com/g/rse-nz-au/c/lvzka29_5I4/m/3kedCoDTAQAJ) |  <a class="rse" href="/codereview">Code Review</a>  |

<div class="home">

  {%- if site.posts.size > 0 -%}
    <ul class="post-list">
      {%- for post in site.posts -%}
      {%- if post.tags contains "resource" -%}
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

    <p class="rss-subscribe">Subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
  {%- endif -%}

</div>
