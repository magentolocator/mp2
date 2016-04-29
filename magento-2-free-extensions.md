---
layout: listing
title: Magento 2 Free Extensions
description: "List of all Magento 2 Free extensions that people love"
permalink:  "/magento-2-free-extensions/"
rating: 97
review_count: 5
---


<div class="row" id="magento-two">

        {% for extension in site.categories.m2e  | sort: 'sort_order' %}
          {% if extension.price == 0 %}
	        <div class="col s12 m3">
	          <div class="card medium">
	            <div class="card-image waves-effect waves-block waves-light">
	              <a href="{{ site.url }}{{ extension.url }}">
	                <img class="activator" src="{{ site.url }}{{ extension.image }}">
	              </a>
	            </div>
	            <div class="card-content">
	              <a href="{{ site.url }}{{ extension.url }}">
	              <span class="card-title activator grey-text text-darken-4">
	                {{ extension.title }}
	              </span>
	              </a>
	              

	              <div class="card-action">
	               

	              <p>
	                <div class="left">
	                <span>
	                  {% if extension.price == 0 %}FREE{% else %} ${{ extension.price }}{% endif %}
	                </span>
	                  <!-- <a href="{{ site.url }}{{ extension.purchase_link }}">
	                    <i class="tiny material-icons">shopping_cart</i>
	                  </a> -->
	                </div>



	                <span class="right">

	                    {% if extension.review_count == 1 %}
	                      {{ extension.review_count }} review
	                    {% elsif extension.review_count > 1 %}  
	                      {{ extension.review_count }} reviews
	                    {% else %}
	                      no review
	                    {% endif %}
	                  
	                </span>

	              

	              </p>
	              </div>

	            </div>
	            
	          </div>
	        </div>
        	{% endif %}
        {% endfor %}

</div>
