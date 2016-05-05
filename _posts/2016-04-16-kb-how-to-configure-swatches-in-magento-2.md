---
layout: kb
title: How to configure Swatches in Magento 2
permalink: /kb/how-to-configure-swatches-in-magento-2.html
published: true
categories: kb 
tags: magento-2-tutorial how-to configure swatches
---


In shopping online, shoppers only base the senses to make a judgment and decide whether they will buy this product or not. Because of that, it is necessary to give the true attributes of the items by **Swatches** feature such as color, pattern, and texture. For example, you have a shirt and it is more attractive with unique shades of color than flat color. The more realistic the customers feel, the more products you can sell out.  

**Color Swatch** is a great solution for the configurable products to show customers the variety of color, pattern or design of your product. On the store view, the swatches of product are displayed on the catalog page and product detail page as the following:

![How to configure Swatches Swatches on Product Page]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-swatches-on-product-page.png)


## Text-Based Swatches

However, if you did not set a specific image for color swatch, a text-based will appear instead of true color and behave in the same way as a swatch with an image.

![How to configure Swatches Text-based Swatches]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-text-based-swatches.png)

When text-based swatches are used to show the available sizes, any size that is not available is crossed out.

![How to configure Swatches Text-based Swatches Unavailable Size]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-text-based-swatches-unavailble-size.png)

## Swatches in Layered Navigation 

The swatches including color swatches and text-based swatches can be also used in the layered navigation. 

![How to configure Swatches Swatches in Layered Navigation]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-swatches-in-layered-navigation.png)

## Overview of configuring swatches 

How to configure swatches in Magento 2 as the following steps:

* Step 1: Create the Swatches
* Step 2: Update your product

### Step 1: Create the Swatches

Apply one of the following method to create the swatches.

#### Method 1: Add a Color Swatch
* Identify the exact color for your product.
* On the Admin sidebar, `Stores > Attributes > Product`.
* In the grid, find and edit the `Color` attribute.
* Set `Catalog Input Type for Store Owner` to **Visual Swatch**.
* Under `Manage Swatch`, tap `Add Swatch` to add a new definition to the bottom of the list. Then, do the following:

![How to configure Swatches Manage Swatch Values]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-manage-swatches-value.png)

  * On the swatch menu, select `Choose a color`.
  
  ![How to configure Swatches Choose Swatch Color]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-choose-swatch-color.png)

  * In the color picker, enter the six numbers that represent the hexadecimal value of the new color in the `#` field, and press the Backspace key to delete the current value. Then tap the `Color Wheel` button in the lower-right corner to save the swatch.
  
 ![How to configure Swatches Hexademical Color]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-hexadecimal-color.png)

  * Enter the label for the color in the Admin and Default Store View.
  * Mark the checkbox under the `Is Default` to set the default color as you need.
  * Enable to change the order when tap the icon in the top left of **Manage Swatch** table and drag it to the new position.
* When complete, tap `Save Attribute`, then flush the cache in `Cache Management` tab.
* Finally, go to `Edit` mode in each product, and update `Color` attribute with the correct swatch. To update multiple products at the same time, follow the steps below.

#### Method 2: Upload a Swatch Image
* Collect the swatch image that is correct for your product.
* On the Admin sidebar, `Stores > Attributes > Product`.
* In the grid, find and edit the `Color` attribute.
* Set `Catalog Input Type for Store Owner` to **Visual Swatch**.
* Under `Manage Swatch`, tap `Add Swatch` to add a new definition to the bottom of the list. Then, do the following:
  * On the swatch menu, select `Upload a file`.
  
  ![How to configure Swatches Upload Swatch file]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-upload-swatch-file.png)

  * Choose the desired image from your computer.
  * Repeat these steps for other swatch images.
  * Enter the label for the color in the Admin and Default Store View.
* When complete, tap `Save Attribute`, then remember to flush the cache in `Cache Management` tab.
* Finally, go to `Edit` mode in each product, and update `Color` attribute with the correct swatch. To update multiple products at the same time, follow the steps below.

### Step 2: Update your product
* On the Admin sidebar, Products > Inventory > Catalog.
* `Filter` the list by Name or SKU to include only the applicable products.

![How to configure Swatches Filter Attributes]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-filter-attribute.png)

* Mark the checkbox of each product that you want the swatch to apply. And then, set the `Actions` control to **Update Attributes**.

![How to configure Swatches Upload Attributes]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-upload-attributes.png)

* Look down to the `Color` attribute, and mark the Change checkbox.

![How to configure Swatches Change Color]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-change-color.png)

* Tap `Save` to apply the swatch. Then remember to flush the cache in the `Cache Management` tab.

![How to configure Swatches Color Frontend]({{ site.url }}/assets/img/kb/how-to-configure-swatches-in-magento-2-color-frontend.png)

Reference: Magento 2 user guide