---
layout: page
title: Magento 2 Tutorial
description: "Magento 2 was released with improved performance and better code base than the previous version. In addition, Magento 2 supports new features to boost conversion rates more effectively, and business agility and productivity improvements. These Magento 2 tutorials cover back and front-end development, as well as administration guides to help you get up and running with Magento 2. For the whole eCommerce community, this is a real boom! Magento 1.x has been around for nearly 10 years and it’s very obvious that it needed either a major update or complete replacement."
permalink: /kb/magento-2-tutorial/

---




<div class="row">



	<ul class="collection with-header">
      {% if(page.description) %}
        <li class="collection-header"><p>{{ page.description }}</p></li>
      {% endif %}

      {% for post in site.categories.kb | sort: 'date'  %}
        {% if post.tags contains "magento-2-tutorial" %}

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
