---
layout: listing
title: Magento 2 Extensions
description: 
meta-title: 
meta-description: 
permalink:  "/magento-2-extensions/"
rating: 95
review_count: 9
---

<div class="row" id="magento-two">

        {% for extension in site.categories.m2e  | sort: 'sort_order' %}
          
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

        {% endfor %}

</div>



<div class="row">

	<ul class="collection with-header">
      <li class="collection-header"><h3>Magento guides</h3></li>
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




