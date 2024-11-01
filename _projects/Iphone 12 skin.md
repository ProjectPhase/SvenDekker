---
title: "iPhone 12 skin"
excerpt: "Custom vinyl skin for the back of my iPhone 12"
date: 20-6-2024
toc: true
toc_sticky: true
breadcrumbs: true  # disabled by default
classes: wide
header:
  image: /assets/Images/iPhone_12_skin/IMG_6092.jpg
  teaser: assets/Images/iPhone_12_skin/IMG_6092-preview.png
---

I'm not a fan of bulky phone cases, so instead of opting for those, I came across dbrand skins. However, at 25 euros, I'd rather customize my own and save some money. Here's how I created my custom iPhone 12 skin:

## Step 1: Get template iPhone

After searching fot `.svg` or `.dxf` iPhone templates on the internet i only could find payed options, so I searched for CAD file of an iPhone 12.

- Download the iPhone 12 model from [`GrabCAD`](https://grabcad.com/library/iphone-12-4) 

I use this model to get the template of the back of the Iphone 12 in Fusion 360

- Open the downloaded file in Fusion
- Create sketch on the back of the iPhone and project only the glass `Figure 1`
- Export the sketch as a `.dxf` `Figure 2`

<p float="centre">
  <img src="/assets/Images/iPhone_12_skin/Sketch_Project.png" width="470" title="Figure 1"/>
  <img src="/assets/Images/iPhone_12_skin/Export_DXF.png" width="450" title="Figure 2"/> 
</p>

## Step 2: Costom design in Rhino Grasshoper

While making this skin i'm following a minor course at the RobotLab where I used this tutorial about thalluses to create a drawing. I will use this to create the design on the skin.

<figure style="width: 400px" class="align-right">
  <img src="/assets/Images/iPhone_12_skin/Canvas.png" alt="">
  <figcaption>Figure 3</figcaption>
</figure> 

- Watch [`this`](https://www.youtube.com/watch?v=dVv6zLicE4s&) tutorial on YouTube from "The Different Design" 

- Install the pluging `Kangaroo2` from [`food4Rhino`](https://www.food4rhino.com/en/app/kangaroo-physics&)

- Download my 2 files or follow `Figure 3`

[Download .3dm File]({{ sven-dekker.com }}/assets/Downloadable/Thallus Phone Case v2.3dm){: .btn .btn--warning}
[Download .gh File]({{ sven-dekker.com }}/assets/Downloadable/Thallus Phone Case v2.gh){: .btn .btn--warning}

As you can see you can change the bounary box if you till want to fit text underith 

- Bake the last node in grasshoper and sellect it in Rhino
- Sellect the curve you just baked in Rhino and go to `File` in the upper right corner and in the drop down menu sellect `Export Sellected...`
- In the next menu you want to save it as an `.dxf` 

<figure style="width: 500px" class="centre">
  <img src="/assets/Images/iPhone_12_skin/Export_Rhino.png" alt="">
  <figcaption>Figure 4</figcaption>
</figure> 


## Step 3: Impored in LightBurn
LightBurn is a laser cutting and engraving software I use for my laser cutter. Iam going to combine the two .dxf files and at text and that is what im evaltualy going to laser cut and engrave.
<figure style="width: 400px" class="align-right">
  <img src="/assets/Images/iPhone_12_skin/Laser_Cut_Setting.png" alt="">
  <figcaption>Figure 5</figcaption>
</figure> 
- Import the two `.dxf`into LightBurn
- Alline and scale them as you like 
- At text underneath 
- Devide the part into two layers. 
    - Layer 1: Line
    - Layer 2: Fill 

It should look something like `Figure 5`

**For the correct engraving and laser cut setting you should do some small experiment for you!**





## Step 4: Engraving and Laser Cutting

When your happy with the design and the settings are correct you can send it to the lasercutter.
I have a small clip of the process

<figure style="width: 300px" class="centre">
  <img src="/assets/Images/iPhone_12_skin/Process.gif" alt="">
  <figcaption>Figure 6</figcaption>
</figure> 

## Result

<p float="left">
  <img src="/assets/Images/iPhone_12_skin/IMG_6092.jpg" width="400" title="Figure 7"/>
  <img src="/assets/Images/iPhone_12_skin/IMG_6094.png" width="400" title="Figure 8"/> 
</p>