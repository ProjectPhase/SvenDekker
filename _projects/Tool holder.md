---
title: "Tool holder"
excerpt: "Process of developing a 'Tool holder' for composite motion"
toc: true
toc_sticky: true
classes: wide
header:
  image: /assets/Images/Custom_Loadbearing_slip_ring/Slew_Bearing_v2.png
  teaser: assets/Images/Custom_Loadbearing_slip_ring/Slew_Bearing_v2.png
---

## Introduction

I was hired as a freelancer by Waag Futurelab in Amsterdam, following a successful internship with the organization. My role involved further developing the tool holder they were working on, focusing on optimizing its functionality and design. The project lasted about a week, during which I applied my technical knowledge and deepened my expertise in creating a product specifically designed for 3D production and easly open-source fabrication.

I will link their devolopment here: ...

## Criteria 

The ultimate goal is to create an interactive, universal tool holder that seamlessly integrates composite motions with user input and allowing for easy tool interchangeability.

Here's an improved version of your design criteria points for better clarity and flow:

### Design Criteria:

* **Develop in Fusion 360:**<br>
 The tool holder must be designed using Fusion 360 to ensure Waag Futurelab can easily access and modify the design after my involvement.

* **Adaptable, Self-Centering Mechanism:** <br>
The design must accommodate tools of varying diameters (with a max of 32mm) and lengths, allowing them to be installed and automatically centered within the holder.

* **Composite Motion:** <br>
The holder should support two types of motion—swinging/rotating along the y-axis and revolving around the z-axis.

* **Design Constraints:**
  * The attachment point must align with two predefined screw holes.
  * Two servo motors need to be embedded to control motion in both axes (y and z).
  * The overall size must fit within the constraints of the AxiDraw plotter.
  * The tool holder must be durable enough to withstand upward pressure during operation.

## Previos development

<figure style="width: 400px" class="align-right">
  <img src="/assets/Images/Tool_Holder/Tool Holder v1.png" alt="">
  <figcaption>Figure 1</figcaption>
</figure> 

Several iterations have been made, with the final iteration visible in `Figure 1`. This iteration closely followed the design criteria.

**Issues Encountered**

1. **Sturdiness:**<br>
The design lacks sturdiness, as indicated by the orange arrow in `Figure 1`. All weight and pressure from the tool are concentrated on the servo motor axis, leading to stability issues.

2. **Revolving Cylinder:** <br>
The revolving cylinder was not properly mounted. Under upward pressure, shown with the purple arrow in `Figure 1`, it tends to pop out of place.

3. **Bearings:** <br>
The use of store-bought bearings is a limiting factor due to their expense and limited size options, as shown with the green arrow in `Figure 1`.

4. **Self-Centering Mechanism:**<br>
The centering is achieved by clamping with sponges, but this method lacks precision, as demonstrated in `Video 1`.

**Potential**

Despite these issues, the design shows promise. The technical concept appears to work, as demonstrated in `Figure 1`. Further development and refinement are needed, preferably with the assistance of someone skilled in technical drawing.


<figure style="width: 800px" class="centre">
  <video width="800" controls loop>
    <source src="/assets/Images/Tool_Holder/revolving-tool-holder.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <figcaption>Video 1</figcaption>
</figure>

## Research

After identifying the issues in the previous iterations, I immediately recalled a past project I worked on called **"Load-bearing Slip Ring"**. You can [read more about this project here](https://www.sven-dekker.com/projects/Load-bearing%20slip%20ring//). A 3D-printed bearing, like the one from `stocki_occ` by `thegoofy` on [Thingiverse](https://www.thingiverse.com/thing:4665998), can address three of the four major problems:

1. **Load-bearing**: It can handle the load on the orange axis.
2. **Mounting Points**: Custom bearings can be designed with mounting points for the revolving part.
3. **Customizable Dimensions**: With 3D printing, bearings of any dimension can be created.

For the fourth issue (self-centering mechanism), I conducted secondary research and found a 3D-printable collet clamping system from `dodasch` on [Printables](https://www.printables.com/model/109942-kraftform-tool-holder-collet-clamping-system). By printing collets of various diameters, a wide range of tools can be accommodated.





