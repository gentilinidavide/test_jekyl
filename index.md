---
layout: default
title: Home
---

## Welcome to my test 
## [ Course 22-23 march 2018](https://bioinfo-dirty-jobs.github.io/master_course/)

___

#### Here you can find a tutorials collection to support the course.

{::nomarkdown}

{% assign pages_list = site.pages | sort:"url" %}
    {% for node in pages_list %}
      {% if node.title != null %}
        {% if node.layout == "page" %}
          <a class="sidebar-nav-item{% if page.url == node.url %} active{% endif %}" href="{{site.url}}{{ node.url }}">{{ node.title }}
          <p class="note">{{node.summary}}</p></a>
        {% endif %}
      {% endif %}
    {% endfor %}
{:/}




 
