---
layout: default
---

{{ content }}


<br/><br/>

<h1>recent posts</h1>

<ul class="postfeed">
    {%- for post in site.posts limit: 10 -%}
    <li>
        {%- assign date_format = "%Y-%m-%d" -%}
        <div class="postfeed-title">[ {{ post.date | date: date_format }} ] <a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></div>
        <div class="postfeed-excerpt">{{ post.excerpt }}</div>
    </li>
    {%- endfor -%}
</ul>