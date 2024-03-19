---

layout: collection
permalink: /documentation/
title: "Documentation"
excerpt: "Minimal Mistakes is a flexible two-column Jekyll theme."
last_modified_at: 2023-08-09T11:59:26-04:00
toc: false
author_profile: false


#intro: 
#  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'
feature_row1:
  - image_path: /assets/Images/ShopBot/CNC.png
    alt: "placeholder image 2"
    title: "Introduction to ShopBot"
    excerpt: 'This article will guide you through the design of my parametric box and step by step through the process of using the ShopBot'
    url: /documentation/shopbot/
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row2:
  - image_path: /assets/Images/Blob-v3-removebg.png
    alt: "placeholder image 2"
    title: "Introduction to  Cricut Maker 3"
    excerpt: 'This article will take you through step by step through the process off using the Cricut maker 3 and my experience'
    url: /documentation/cricut/
    btn_label: "Read More"
    btn_class: "btn--primary"
#feature_row3:
#  - image_path: /assets/Images/Lasercutter-removebg.png
#    alt: "placeholder image 2"
#    title: "Introduction to a lasercutter"
#    excerpt: 'This article wil take you through the steps and safety measures on how to use the BRM Laser Machine'
#    url: /documentation/lasercutter/
#    btn_label: "Read More"
#    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/Images/Website_building.jpeg
    alt: "Setting up a static website"
    title: "Setting up a static website" #Week 1
    excerpt: 'This article will take you step by step through the process of building your own static website.'
    url: /documentation/setting-up-a-static-website/
    btn_label: "Read More"
    btn_class: "btn--primary"

#{% include feature_row id="feature_row3" type="right" %}

   
---

{% include feature_row id="feature_row1" width="100px" type="right" %}

{% include feature_row id="feature_row2" width="50%" type="left" %}

{% include feature_row id="feature_row4" type="left" %}
