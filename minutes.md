---
layout: page
title: Minutes
permalink: /minutes/
---

| Meeting number  | Status | Reference  |
| --------  | ------------------- | --------------------- |
| SCM No.22 | Pending | &nbsp; &nbsp;  &nbsp; **2021.11.23** |
| SCM No.21 | Final | <a class="rse" href="/assets/pdfs/SCM-21.pdf">2021.10.26</a> |
| SCM No.20 | Final | <a class="rse" href="/assets/pdfs/SCM-20.pdf">2021.09.28</a> |
| SCM No.19 | Final | <a class="rse" href="/assets/pdfs/SCM-19.pdf">2021.08.24</a> |
| SCM No.18 | Final | <a class="rse" href="/assets/pdfs/SCM-18.pdf">2021.07.27</a> |
| SCM No.17 | Final | <a class="rse" href="/assets/pdfs/SCM-17.pdf">2021.06.22</a> |
| SCM No.16 | Final | <a class="rse" href="/assets/pdfs/SCM-16.pdf">2021.05.18</a> |
| SCM No.15 | Final | <a class="rse" href="/assets/pdfs/SCM-15.pdf">2021.04.23</a> |
| SCM No.14 | Final | <a class="rse" href="/assets/pdfs/SCM-14.pdf">2021.03.23</a> |
| SCM No.13 | Final | <a class="rse" href="/assets/pdfs/SCM-13.pdf">2021.02.23</a> |
| SCM No.12 | Final | <a class="rse" href="/assets/pdfs/SCM-12.pdf">2020.12.08</a> |
| SCM No.11 | Final | <a class="rse" href="/assets/pdfs/SCM-11.pdf">2020.11.05</a> |
| SCM No.10 | Final | <a class="rse" href="/assets/pdfs/SCM-10.pdf">2020.09.24</a> |
| SCM No.9 | Final | <a class="rse" href="/2020/08/25/Minutes-of-SCM-09">2020.08.25</a> |
| SCM No.8 | Final | <a class="rse" href="/2020/08/04/Minutes-of-SCM-08">2020.08.04</a> |
| SCM No.7 | Final | <a class="rse" href="/2020/06/23/Minutes-of-SCM-07">2020.06.23</a> |
| SCM No.6 | Final | <a class="rse" href="/2020/05/26/Minutes-of-SCM-06">2020.05.26</a> |
| SCM No.5 | Final | <a class="rse" href="/2020/04/28/Minutes-of-SCM-05">2020.04.28</a> |
| SCM No.4 | Final | <a class="rse" href="/2020/02/25/Minutes-of-SCM-04">2020.02.25</a> |
| SCM No.3 | Final | <a class="rse" href="/2020/01/28/Minutes-of-SCM-03">2020.01.28</a> |
| SCM No.2 | Final | <a class="rse" href="/2019/11/01/Minutes-of-SCM-02">2019.11.01</a> |
| SCM No.1 | Final | <a class="rse" href="/2019/10/17/Minutes-of-SCM-01">2019.10.17</a> |


<div class="home">

  {%- if site.posts.size > 0 -%}
    <ul class="post-list">
      {%- for post in site.posts -%}
	  {%- if post.tags contains "minutes" -%}
      <li>
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
      </li>
      {%- endif -%}
      {%- endfor -%}
    </ul>

  {%- endif -%}

</div>
