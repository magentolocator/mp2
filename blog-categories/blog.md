---
layout: page
title: Blog
pagetitle: Magento Blog Tutorial by Mageplaza
description: "The Magento Blog posts"
pagedescription: "The Magento Blog posts"
permalink: "/blog/"

redirect_from:
  - /blog-posts/
  - /posts/
  - /categories/blog
  - /categories/blog/
---


<div class="row">

	<ul class="collection with-header">
      {% if(page.description) %}
        <li class="collection-header"><p>{{ page.description }}</p></li>
      {% endif %}

      {% for post in site.categories.blog | sort: 'date'  %}

        <li class="collection-item avatar">
        	<i class="material-icons circle green">insert_chart</i>
        	<span class="title">
          	<a href="{{ site.url }}{{ post.url }}" >
    	        {{ post.title }}
            </a>
          </span>
          <p>{{ post.excerpt | strip_html }}</p>
          
        </li>

      {% endfor %}

  </ul>


</div>
