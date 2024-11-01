---
title: "Load-bearing slip ring"
excerpt: "Custom load-bearing slip ring to mount UV nail lamp on a articulating arm"
date: 17-1-2024
toc: true
toc_sticky: true
breadcrumbs: true  # disabled by default
classes: wide
header:
  image: /assets/Images/Custom_Loadbearing_slip_ring/Color_Bearing.png
  teaser: assets/Images/Custom_Loadbearing_slip_ring/Color_Bearing.png
---
<figure style="width: 200px" class="align-right">
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/clearoff.jpeg" alt="">
  <figcaption>Figure 1</figcaption>
</figure> 
<br />
My mother is a pedicurist and from her pedicure practice, she has requested an engineering task. It involves a UV lamp that needs to hang from an articulating arm to be multipurpose, serving both hands and feet. In the past, I attempted to solve this without a slip ring, which turned out to be very dangerous as the wire was twisted and posed a fire hazard, depicted in `Figure 1`.



<figure style="width: 200px" class="align-left">
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/Slip_Ring.jpg" alt="">
  <figcaption>Figure 2</figcaption>
</figure>

<br />
I began this project with the search for a slip ring. On Aliexpress, I found a slip ring with 3 channels capable of handling 10A for 15 euros `Figure 2`. In hindsight, this was considerable overkill, and the slip ring was quite large. Then I searched for a bearing to carry the weight of the UV lamp. These are available in large diameters but never come with mounting holes. Therefore, I started looking for 3D-printed bearings capable of axial loads. That's when I found the bearing by thegoofy on Thingiverse, which is a slew bearing and a parametric design downloadable for Fusion 360. More detail in `Step 2`.

<br />
Now that my essential components were specified, I could begin the design process. 

## Step 1: Sketch slip ring in CAD

- To create a design, it is necessary to have a 3D sketch of the slip ring to use as a reference `Figure 3`.

<figure style="width: 300px" class="centre">
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/GOCO_Bearing.png" alt="">
  <figcaption>Figure 3</figcaption>
</figure>

## Step 2: Download slew bearing

- Download the slew bearing from thegoofy on [`Thingiverse`](https://www.thingiverse.com/thing:2375124) 
  - Download the slew bearing with correct parameters from stocki_occ by thegoofy on [`Thingiverse`](https://www.thingiverse.com/thing:4665998)
  - Download the slew bearing with spacers from thegoofy on [`Thingiverse`](https://www.thingiverse.com/thing:2381833)

<p float="centre">
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/Slew_Bearing.jpg" width="470" title="Figure 4"/>
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/Slew_Bearing_Spacers.jpg" width="350" title="Figure 5"/> 
</p>
 
 - Modify the parameters of the slew bearing to ensure that its holes align with those of the reference slip ring in the design workspace

## Step 3: Sketch mounting point of the articulating arm

- Sketch the mount point from the articulating arm to the slew bearing `Figure 6`. This is done using a loft. 

<figure style="width: 300px" class="centre">
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/Mount_Point.png" alt="">
  <figcaption>Figure 6</figcaption>
</figure>

## Step 4: Sketching the mounting point of the UV lamp

- Sketching the mount point from the UV lamp to the slew bearing `Figure 7`. 
  - Requiring disassembly of the UV lamp to neatly conceal the mounting, utilizing heat inserts `Figure 8&9`.

<p float="left">
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/Mount_Point_UV.png" width="250" title="Figure 7"/>
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/IMG_4119.jpg" width="250" title="Figure 8"/>
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/IMG_4118.jpg" width="250" title="Figure 9"/> 
</p>


## Step 5: Soldering 

- Soldering the the wiring for the plug that goes into the UV lamp.

- Soldering the wiring that goes thorugh the articulation arm.

<p float="left">
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/IMG_4121.jpg" width="450" title="Figure 10"/>
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/IMG_4122.jpg" width="250" title="Figure 11"/> 
</p>

## Result
The end result is visable in the section view and the video below.

<figure style="width: 300px" class="centre">
  <img src="/assets/Images/Custom_Loadbearing_slip_ring/Section_View.png" alt="">
  <figcaption>Figure 12</figcaption>
</figure>

{% include video id="RjCyNpwfA4M" provider="youtube" %}

## Conclusion
With the excellent design by thegoofy, designing the Custom Load-Bearing slip ring was manageable. The result looks professional, and compared to the previous solution, there can be no user error by turning the UV lamp in the same direction too often.

## Recommendations
For next time, I would consider a different slip ring for several reasons: This slip ring was rather large, it was overkill and quite expensive. Also, the top could be merged with the outside of the slew bearing. This simplifies the design by saving three screws and three heat inserts.


## Download Project
[Download .f3z File]({{ sven-dekker.com }}/assets/Downloadable/Slew_Bearing.f3z){: .btn .btn--warning}