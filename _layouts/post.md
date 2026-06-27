---
layout: default
---

<h1>{{ page.title }}</h1>
{%- assign date_format = "%Y-%m-%d" -%}
<h4 class="post-date">{{ page.date | date: date_format }}</h4>

<p><i>tags: 

{% for tag in page.tags %}
    <span>
        {% assign last_tag = page.tags | last%}
        {% if tag == last_tag %}
            <a href="/tags#{{tag | downcase}}">{{tag}}</a>
        {% else %}
            <a href="/tags#{{tag | downcase}}">{{tag}}</a>,
        {% endif%}
    </span>
{% endfor %}
</p></i>

<hr/>

{{ content }}