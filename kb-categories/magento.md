---
layout: page
title: Magento Tutorial
description: 
permalink: /kb/magento/

---




<div class="row">

	<ul class="collection with-header">
      <li class="collection-header"><h1>{{ page.title }}</h1></li>
      {% for post in site.categories.kb | sort: 'date'  %}
        {% if post.tags contains "magento" %}

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
