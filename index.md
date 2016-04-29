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
        <h1 class="header center">{{ site.slogan }}</h1>
        <div class="row center">
            <h4 class="header col s12 light center">{{ site.description }}</h4>
        </div>
        <div class="row center">
            <a href="#live-demo" class="btn-light btn-large waves-effect waves-light modal-trigger">Demo</a>
            <a href="{{ site.url }}/pricing/" class="btn-light btn-large waves-effect waves-light">Pricing</a>
        </div>
    </div>
</div>



<div class="container">
  <div class="section">


      <div class="row">
          <div class="col s12 m8 offset-m2">
            <br>
            <img id="responsive-img" src="http://materializecss.com/images/responsive.png">
          </div>
        </div>


        <div class="row">
          <h3 class="col s12 light center header">Materialize simplifies life for developers and the users they serve.</h3>
        </div>


        <div class="row">
          <div class="col s12 m4">
            <div class="center promo">
              <i class="material-icons">flash_on</i>
              <p class="promo-caption">Speeds up development</p>
              <p class="light center">We did most of the heavy lifting for you to provide a default stylings that incorporate our custom components. Additionally, we refined animations and transitions to provide a smoother experience for developers.</p>
            </div>
          </div>

          <div class="col s12 m4">
            <div class="center promo">
              <i class="material-icons">group</i>
              <p class="promo-caption">User Experience Focused</p>
              <p class="light center">By utilizing elements and principles of Material Design, we were able to create a framework that incorporates components and animations that provide more feedback to users. Additionally, a single underlying responsive system across all platforms allow for a more unified user experience.</p>
            </div>
          </div>

          <div class="col s12 m4">
            <div class="center promo">
              <i class="material-icons">settings</i>
              <p class="promo-caption">Easy to work with</p>
              <p class="light center">We have provided detailed documentation as well as specific code examples to help new users get started. We are also always open to feedback and can answer any questions a user may have about Materialize.</p>
            </div>
          </div>
        </div>


      <div class="divider"></div>


      <div class="row center">
          <h2 class="light header">Free, open source, and easy to use.</h2>
          <p class="col s8 offset-s2 caption">Mageplaza is a library of modules for Magento. Our extensions are open source for any use. Download what you like and get started!</p>
      </div>



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








