---
layout: page
title: Magento 2 User Guide
description: 
permalink: /kb/magento-2-user-guide/

---


<div class="row">

	<ul class="collection with-header">
      <li class="collection-header"><h1>{{ page.title }}</h1></li>
      {% for post in site.categories.kb | sort: 'date'  %}
        {% if post.tags contains "magento-2-user-guide" %}

        <li class="collection-item avatar">
        	<i class="material-icons circle green">insert_chart</i>
        	<span class="title">
          	<a href="{{ site.url }}{{ post.url }}" >
    	        {{ post.title }}
            </a>
          </span>

          <p>{{ post.excerpt | strip_html }}</p>

          
        </li>

        {% endif %}
      {% endfor %}

  </ul>


</div>
