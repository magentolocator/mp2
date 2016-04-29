---
layout: kb
title: How to Change Favicon in Magento 2
permalink: /kb/how-upload-favicon-magento-2.html
published: true
categories: magento-2 magento-2-tutorial magento-2-manage-store magento-2-user-guide
tags: magento-2 how-to manage store logo
---


**Favicon** is short for “favorite icon,” and refers to the little icon on the tab of each browser page.
Depending on the browser, the favicon also appears in address bar, just before the URL.
Favicons are generally 16 x 16 pixels or 32 x 32 pixels in size. Magento accepts ICO, PNG, JPG,
and SVG file types, although not all browsers support these formats. The most widelysupported
file format to use for a favicon is ICO. There are many free tools available online that
you can use to generate an ICO image or convert an exiting image to the format.

![magento 2 favicon](https://lh3.googleusercontent.com/hPSjhNLSK0gYc0AWvy698IcbMSiCZzCUUnHHTuCSMG1tm6H1WmB4Brm9a-Uef4_8iTuhqctne7aHYyRO9ZqqANsQWSLO2uQcR5tj1b-f9csxY8acZ8PnOw-BzGVq2ZdlqckGp96v)

## Step 1: Create a Favicon

* Create a 16x16 or 32x32 graphic image of your logo, using the image editor of your choice.
* (Optional) Use one of the available online tools to convert the file to the .ico format. Then, save
the file to your computer.


## Step 2: Upload the Favicon to Your Store

* On the Admin sidebar, tap Stores. Then under Settings, choose Configuration.
* In the panel on the left under General, choose Design.
* Expand the HTML Head section. Then, do the following:

![how to upload favicon magento 2](https://lh3.googleusercontent.com/0yWNmAO7NoehKmQTqHl9grB4dHMolZtXOpRGMqxD_jbcf5MHAbMzspuF2u3c4J1tOhP1Klh4gSAlAnk6gXRA-AttiUoP-Ov6sXVtLB1sglsnirNJ3RVhK0lIK9iM28DriMrQOzoj)

	* Tap Choose File. Then, find the favicon file that you prepared.
	* If you want to delete the current favicon, mark the Delete Image checkbox.

* When complete, tap Save Config.

## Step 3: Refresh the Cache

* When prompted to refresh the cache, click the Cache Management link in the message at the
top of the workspace.
* In the list, mark the Page Cache checkbox that is marked “Invalidated.”
* Set Actions to “Refresh.” Then, tap Submit.
* To view the new favicon, return to your storefront and press F5 to refresh the browser.





Ref: Magento 2 User Guide
