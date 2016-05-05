---
layout: home
title: Mageplaza
meta-title: Mageplaza
meta-description: 
meta-keywords: 
redirect_from:
    - /index.php/
---




<div class="section no-pad-bot" id="index-banner">
    <div class="container">
        <h1 class="header center">Welcome to {{ site.name }}</h1>
        <div class="row center">
            <h4 class="header col s12 light center">{{ site.description }}</h4>
        </div>
        <div class="row center">
            <a href="{{ site.url }}/magento-2-extensions/" class="btn-light btn-large waves-effect waves-light">Magento 2</a>
            <a href="{{ site.url }}/magento-extensions/" class="btn-light btn-large waves-effect waves-light">Magento 1</a>
        </div>
    </div>
</div>



<div class="container">
  <div class="section">



      <div class="row center">
          <h2 class="light header">Why Mageplaza?</h2>
          <p class="col s8 offset-s2 caption">Mageplaza is a library of modules for Magento. Our extensions are open source for any use. Download what you like and get started!</p>
      </div>

        <div class="row">
          <div class="col s12 m4">
            <div class="center promo">
              <i class="material-icons">system_update_alt</i>
              <p class="promo-caption">Free Updates</p>
              <p class="light center"></p>
            </div>
          </div>

          <div class="col s12 m4">
            <div class="center promo">
              <i class="material-icons">thumb_up</i>
              <p class="promo-caption">Free Support For Life</p>
              <p class="light center"></p>
            </div>
          </div>

          <div class="col s12 m4">
            <div class="center promo">
              <i class="material-icons">replay_30</i>
              <p class="promo-caption">Risk-free 30-day Money Back</p>
              <p class="light center"></p>
            </div>
          </div>
        </div>


      <div class="divider"></div>


      


    <div class="row" id="magento-one">

      <h2 class="col s12 header">Magento 1 extensions</h2>

        {% for extension in site.categories.m1e limit:8  | sort: 'sort_order' %}
          
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


  <div class="row" id="magento-two">

      <h2 class="col s12 header">Magento 2 extensions</h2>

        {% for extension in site.categories.m2e limit:12  | sort: 'sort_order' %}
          
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





      </div>
      <!-- section -->
</div>
<!-- End container -->









