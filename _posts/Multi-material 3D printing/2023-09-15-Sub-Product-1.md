---
title:  "Sub-Product 1" 
permalink: /multi-material 3d printing/sub-product 1/
layout: single
last_modified_at: 18-9-2023
read_time: true
toc: true
toc_label: "Table of contents"
toc_icon: "stream"
toc_sticky: "false"
classes: wide

gallery:
   - url: /assets/Images/Push to Release ball.png
     image_path: /assets/Images/Push to Release ball.png
     alt: "Ball"
   - url: /assets/Images/Push to Release linear.png
     image_path: assets/Images/Push to Release linear.png
     alt: "Linear"
   - url: /assets/Images/Push to Release spring.jpg
     image_path: assets/Images/Push to Release spring.jpg
     alt: "Spring"

gallery1:
   - url: /assets/Images/A1 Hotend.png
     image_path: /assets/Images/A1 Hotend.png
     alt: "A1 Hotend"
   - url: /assets/Images/QuickSwap.png
     image_path: /assets/Images/QuickSwap.png
     alt: "QuickSwap"
---

## 1. Research

In the research, the research questions (sub-questions) are answered one by one with justification. For this purpose, reference will be made to the used sources using the APA method.

### 1.1 What specific multi-material 3D printing products exist?

In Chapter 2 of the "Plan of Approach," under the heading "Problem Statement," six different methods for multi-material 3D printing are discussed: MMU, Filament splicing, Dual extruder printhead, IDEX, Toolchanger, and CNC nozzle changing. Before specific products are examined, it is important to determine which of these methods are not suitable for the assignment, within the defined scope and in line with the objectives. Therefore, each method will now be briefly discussed.

#### 1.1.1 Further investigate

---
<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/ERCF.png" alt="">
  <figcaption>Figure 1</figcaption>
</figure> 

##### 1.1.1.1 MMU

It's interesting that multiple materials can be printed with a single extruder. However, it's unfortunate that material needs to be purged from the hotend. Could this be resolved? Is this an interesting solution?

**Further investigate =** ✔

<figure style="width: 300px" class="align-left">
  <img src="/assets/Images/Filament splicing.png" alt="">
  <figcaption>Figure 2</figcaption>
</figure>
##### 1.1.1.2 Filament splicing

The market for existing products is limited. Currently, there is only one known product that utilizes this technology, namely the Palette 3 by Mosaic, priced at $599 `Figure 2`. When we search for [`Review Palette 3`](https://www.reddit.com/r/3Dprinting/comments/qmg3eu/is_mosaic_palette_3_worth_it_any_users_feedback_i/) on "Duck Duck Go", the first link leads to a Reddit discussion. In the discussion, opinions are generally negative, and furthermore, this technology has not seen any innovative or developmental advancements for quite some time.

**Further investigate =** ❌

##### 1.1.1.3 Dual extruder printhead

Calibrating a **"Dual nozzle hotend"** can be challenging because you need to precisely adjust two points on the print bed to the same level. If these points are not equal, it can be difficult to properly align the two print heads since there may be limited or no adjustment options. This is also highlighted in an article on  [`xyzdims.com`](https://xyzdims.com/2019/09/22/3d-printing-dual-nozzle-printhead/).

**Further investigate =** ❌

The initial impression of the **"Dual Switching Hotend"** appears to be a reasonable solution for printing with two materials. However, adding more print heads does not seem like a suitable idea due to potential issues related to weight, precision, and complexity. This can be gleaned from the [`Multiple Switching Extrusions project`](https://xyzdims.com/2021/01/31/3d-printing-multiple-switching-extrusions-mse/)

**Further investigate =** ❌

##### 1.1.1.4 IDEX

For multi-material 3D printing with two materials, IDEX technology appears to be one of the most suitable methods. This approach has extensive online documentation. However, innovating this technique can be challenging, and furthermore, it is limited to the use of only two materials.

**Further investigate =** ❌

##### 1.1.1.5 Toolchanger

The toolchange method is most commonly used in the professional industry. This is because it offers many possibilities in terms of materials, nozzle diameters, and potentially other tools. Cost considerations are less significant for large companies. In cases where costs can be kept limited, this method is also interesting.

**Further investigate =** ✔

##### 1.1.1.6 CNC nozzle changing

The Swapper3D by BigBrain3D is currently the only one on the market that performs a nozzle change similar to a CNC tool changer. This concept provides the opportunity to create various variations, and there is still ample room for innovation in this field.

**Further investigate =** ✔



#### 1.1.2 MMU

---

In this chapter, various MMUs (Multi-Material Units) are examined and evaluated.
<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/Prusa MMU2 print.jpg" alt="">
  <figcaption>Figure 3</figcaption>
</figure>
##### 1.1.2.1 Prusa MMU (spcific MMU2)

At Waag FabLab, they have a Prusa MK3 with an MMU2. To gain experience for this project, a calibration cube was printed with two colors to keep the complexity low. It took two days to achieve a semi-successful print `Figure 3`. The filament switch did not go well on various layers, resulting in the printer not producing anything. To obtain this result, more than 6 interventions were required, mainly at the beginning. This print with one color takes 1 hour and 15 minutes, and with two colors, it takes 4 hours and 34 minutes, which is also a significant drawback.

After having 5 unsuccessful prints and 1 semi-successful print, it can be concluded that this MMU is not reliable, and it should not serve as an example.

Meanwhile, Prusa has released an MMU3 priced at €329 with better reviews. The most significant drawback mentioned in the review is "The problems start when trying to use mixed materials or PETG" <cite><a href="https://www.reddit.com/r/prusa3d/comments/15k3kia/mmu3_review/">Reddit - Dive into anything</a></cite>. Printing with various materials is precisely the goal.

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/Filament shape.png" alt="">
  <figcaption>Figure 4</figcaption>
</figure>

##### 1.1.2.2 Enraged Rabit Carrot Feeder (ERCF)

This is an open-source MMU, and all the documentation is available on GitHub. Within this documentation, you can also find a link to the BOM (Bill of Materials) with various links to websites where the components can be purchased. It is clearly indicated that these are affiliated links. Kits are also available from other suppliers for around €150.

The video review by [`NERO 3D`](https://www.youtube.com/watch?v=ccwiylrg7KM) discusses both the strengths and weaknesses, as well as some issues and successes. One of the biggest problems the reviewer encountered was the improperly shaped filament end during retraction `Figure 4`. Later, it was found that this was due to an unsuitable combination of the hotend and nozzle. The old hotend consists of multiple parts, which can result in plastic getting stuck in various places `Figure 6`. However, the new hotend, the RapidChange Revo, has a nozzle with an integrated heatbreak. This has the advantage of preventing any snagging due to the smooth interior `Figure 5`. Additionally, the reviewer noted that even if you're not printing with all 6 materials, you always have 6 materials available without the need to change filament rolls each time.

<figure style="width: 600px" class="center">
  <img src="/assets/Images/Split view Revo.png" alt="">
  <figcaption>Figure 5, Figure 6</figcaption>
</figure>

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/3DChameleon.jpg" alt="">
  <figcaption>Figure 7</figcaption>
</figure>
##### 1.1.2.3 3DChameleon

The 3DChameleon mk3 costs $179 with shipping costs of €220 and can switch between four colors. Their website explains how this system works. They describe it as follows: 
> The 3D Chameleon operates by utilizing your 3D printer's existing mechanical hardware to      automatically remove and reload filaments when a color (or material) change is needed. By leveraging your existing electronics, we can use standard GCode commands to tell the 3D Chameleon which color to select.
> <cite><a href="https://www.3dchameleon.com/">Home of the 3DCHameleon</a></cite>

To simplify this explanation, the 3DChameleon uses its own microcontroller and a button. During a filament change, the G-code includes instructions to press the button a certain number of times for the desired color, allowing the microcontroller to know which color to load. There is no direct integration between the printer and the 3DChameleon. This makes it a suitable product for more affordable printers like the Ender 3 V2 and other similar models.

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/ROME.png" alt="">
  <figcaption>Figure 8</figcaption>
</figure>

##### 1.1.2.4 ROME

The explanation of ROME on HelgeKeck's [`GitHub repository ROME`](https://github.com/HelgeKeck/rome) is much faster than a regular MMU or ERCF setup. The entire process of loading and unloading filament is several times faster, not only because ROME simply needs to park the filament behind the Y-split. In its own mode, ROME handles the filament loading and unloading, skipping the phase controlled by the slicer. This process is highly optimized for a specific Hotend/Filament combination.

A significant time-saving, as HelgeKeck explained, is that the filament only needs to be parked behind the Y-split. For each filament change, this may be only a few seconds, but with quickly accumulating more than hundreds of filament changes, this adds up. This also applies to the 3DChameleon.

<figure style="width: 300px" class="align-left">
  <img src="/assets/Images/X1P.png" alt="">
  <figcaption>Figure 9</figcaption>
</figure>

##### 1.1.2.5 Bambu Lab

Bambu Lab is a prominent player in the 3D printing industry, particularly in the field of multi-material printing. Their printers, the P1P (€1015.80 incl. AMS) and the X1-Carbon (€1524.19 incl. AMS), have proven to be significant successes, especially when used with their Automatic Material System (AMS) priced at €365.03. However, it's important to note that the AMS is specifically designed for use with their own printers and is not compatible with other brands.

Recently, as of the day of writing, Bambu Lab has launched a new system, the A1-mini (€497.21 incl. AMS Lite), in conjunction with the AMS Lite.

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/A1 mini.png" alt="">
  <figcaption>Figure 10</figcaption>
</figure>

The AMS Lite is an evolution of the AMS system, with some notable improvements. Filament spools are now placed in the center instead of on the outside, which is convenient for using cardboard spools. Additionally, the splitter, where the filament is retracted to, is now directly above the extruder rather than in a separate box above, which was previously seen as a positive change. Moreover, the amount of plastic that needs to be purged with this system has been reduced.

Although Bambu Lab's products are not open source, they currently offer a wide range of individual spare parts on their website. This may provide opportunities for the development of an open-source multi-material unit, which is included in the research question "Which purchased components offer possibilities within the budget." It is difficult to predict how long they will continue to offer spare parts.



#### 1.1.3 Toolchanger

---

In this chapter, various tool changers are investigated and evaluated.

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/E3D.png" alt="">
  <figcaption>Figure 11</figcaption>
</figure>

##### 1.1.3.1 E3D ToolChanger

E3D, which stands for "Engineering 3D Printing Solutions," was one of the first leading manufacturers to introduce the ToolChanger system in 2019, marking a significant breakthrough. Many open-source toolchangers are still based on their technology.

The toolchanger mechanism has three contact points that are reasonably spaced apart on the exterior for stability. To securely hold the tool, a key is used that rotates a quarter turn. `Figure 11` shows the printhead, and Figure 12 displays the tools.

<figure style="width: 600px" class="centre">
  <img src="/assets/Images/E3D dock.png" alt="">
  <figcaption>Figure 12</figcaption>
</figure>

##### 1.1.3.2 Wham Bam: The MUTANT V2

The MUTANT V2 is a universal tool-changing system that offers the possibility to make your FDM printer more versatile. It allows for easy swapping of the hotend with tools such as laser cutters, pen plotters, vinyl cutters, and more. However, this system is not intended for changing tools within a 3D printing process.

The elegance of this design lies in the two plates easily sliding together using a dovetail connection and securely locking in place with a lever. Electrical contact is managed through a series of pogo pins, also known as spring contact pins or compression spring pins. This is ideal for tool changers.

<figure style="width: 600px" class="centre">
  <img src="/assets/Images/Wham Bam.png" alt="">
  <figcaption>Figure 13</figcaption>
</figure>

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/XChange.png" alt="">
  <figcaption>Figure 14</figcaption>
</figure>

##### 1.1.3.3 XChange

XChange by PrinterMods is a quick-change tool head for any 3D printer. This product is not yet available but is live on Kickstarter, where they are still seeking backers.

This product bears a resemblance to the MUTANT V2. In both products, it's not possible to change tools during the print, but XChange approaches the coupling differently, offering potential possibilities. XChange utilizes magnets and pins, allowing the coupling to move only forward and backward, unlike the MUTANT V2, which also involves vertical movement.

The detachment is achieved by using the polarity of the magnets. Moving the lever upward causes the magnets to rotate so that they repel each other. This can be clearly seen in `Figure 15`, which is a different design but follows the same principle.

<figure style="width: 600px" class="centre">
  <img src="/assets/Images/Magnet changer.png" alt="">
  <figcaption>Figure 15</figcaption>
</figure>

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/Tapchanger.png" alt="">
  <figcaption>Figure 16</figcaption>
</figure>

##### 1.1.3.4 Tapchanger

Tapchanger is an open-source project by Viesturz [`GitHub repository Tapchanger`](https://github.com/viesturz/tapchanger).
The concept behind his design is that you don't need servo motors or other moving parts to couple and uncouple it. A sensor is used to verify the successful coupling and uncoupling.

Viesturz has shared the CAD files along with a Bill of Materials (BOM) and other documentation in a GitHub repository. He is also actively participating in a Discord channel called "Voron Toolchangers Discord."



#### 1.1.4 CNC nozzle changing

---

In Chapter 2 of the "Plan of Approach," in the "Problem Statement" section, we have already extensively discussed The Swapper3D. Currently, there are no other products on the market that apply the same method. The concept of combining each material or color with its own nozzle is exceptionally inspiring. What's interesting is that in recent years, and even months, new products have emerged on the market that enable innovation within this concept. This will be further explored in research question 3.



### 1.2 What tool change methods exist in other production machines?

---
<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/Carousel.png" alt="">
  <figcaption>Figure 17</figcaption>
</figure>

3D printers are not the first machines where tool changes are desired during production. Inspiration can perhaps be drawn from existing methods.

#### 1.2.1 Carousel Automatic Tool Changer

Also known as a Carousel Automatic Tool Changer, it is an essential component commonly found in CNC machines. Its primary purpose is to automate the process of changing tools during machining operations, thereby improving efficiency and reducing downtime.

Disadvantages:

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/Vertical carousel.png" alt="">
  <figcaption>Figure 18</figcaption>
</figure>

- High complexity with more moving parts
- The parts are not designed for 3D printers
- Existing printers like the Ratrig Vcore-3.1 and Voron printers require significant modifications to create space for a carousel. A Side Mount Carousel Automatic Tool Changer `Figure 18` could be of assistance in this regard, as seen with the Swapper3D `Figure 20`, but the complexity remains.

#### 1.2.2 Linear automatic tool changer

Also known as a Linear Automatic Tool Changer, it is a device commonly used in machining centers and CNC machines to automate the process of changing cutting tools during various machining operations. In contrast to the Carousel automatic tool changer, which uses a rotating tool storage carousel, a linear automatic tool changer employs a linear motion mechanism to achieve tool changes.

This technique is also evident in current toolchanger 3D printers.

<figure style="width: 900px" class="centre">
  <img src="/assets/Images/Linear dock.png" alt="">
  <figcaption>Figure 19, Figuur 20</figcaption>
</figure>

#### 1.2.3 Push to release mechanism

In the event that the tool change method is to be used, there are various options to mechanically secure the tool without the need for motors. This helps keep costs low. The complexity of the suspension is higher, but you do not need to program and connect one less motor.

The best examples are drawer locks. There are three images of three different technical mechanisms. `Figuur 21, 22, 23`

{% include gallery id="gallery" caption="Figure 21, Figure 22, Figure 23" %}


### 1.3 What purchased components offer possibilities within the budget?

---

#### 1.3.1 RapidChange Revo

Unlike other nozzles, the Revo hotend can be easily swapped by the user for €26.99. This is because the heatbreak and the nozzle form a single object. Furthermore, the hotend can be gripped by the silicone sock and hand-tightened.

To tighten the Revo, it takes about 15 revolutions. This would be automated using a stepper motor and the same software technology as sensorless homing. Sensorless homing utilizes the motor and the load it moves to determine when the component has reached its end position.

<figure style="width: 600px" class="centre">
  <img src="/assets/Images/Revo.png" alt="">
  <figcaption>Figure 24</figcaption>
</figure>

<figure style="width: 300px" class="align-right">
  <img src="/assets/Images/A1 Hotend.png" alt="">
  <figcaption>Figure 25</figcaption>
</figure>

#### 1.3.2 Bambu Lab hotend 

Bambu Lab offers a printer, the A1 mini, for which they provide a wide range of spare parts and accessories. They also offer their hotend heating construction and hotends with nozzles `Figure 25`. "The Hotend heating construction is specially designed to support the fast-changeable hotend design. A quick clamping mechanism is used to secure the heating block and the heating base, enabling easy separation of the thermal and electronic components of the hotend" <cite><a href="https://eu.store.bambulab.com/nl-nl/collections/accessories-for-a1-mini/products/hotend-with-0-4-mm-nozzle-a1-mini">Bambu Lab</a></cite>

So, a one-time purchase of the hotend heating construction is needed, priced at €21.34, and for each additional hotend with a nozzle, the cost is €13.21. These products allow for the easy replacement of just the hotend with the nozzle. With this concept, all the cables are kept on the printhead, eliminating the need for an extra extruder, hotend fan, and part cooling fan. This can significantly reduce costs and complexity.

<figure style="width: 200px" class="align-right">
  <img src="/assets/Images/QuickSwap.png" alt="">
  <figcaption>Figure 26</figcaption>
</figure>

#### 1.3.3 QuickSwap - Hotend and Insert

BigBrain3D also offers their QuickSwap Hotend `Figure 26` separately for $99. They sell the inserts separately for $24.99, but you still need to add your own nozzle. These products also provide possibilities. However, they are currently out of stock. BigBrain3D is not a well-known name in the 3D printing world, which also doesn't provide certainty for the future.

<figure style="width: 300px" class="align-left">
  <img src="/assets/Images/Ultimaker.png" alt="">
  <figcaption>Figure 27</figcaption>
</figure>

#### 1.3.4 Ultimaker print core

UltiMaker offers quick-change print cores for their S-series at a price of $114.95. However, the cost of a hotend with a nozzle is too high to integrate into an open-source multi-material 3D printer. Nevertheless, the attachment mechanism is very robust, as can be seen in the GIF on the  [`MatterHackers website`](https://www.matterhackers.com/store/l/ultimaker-print-core-aa/sk/M7YUTWSY). Inspiration can be drawn from this.

### 1.4 What possibilities exist between the slicer and G-code?

Klipper has a fairly basic interrogation for multiple extruders/printheads. To assign individual variables to each extruder/printhead, the user must create macros themselves.

#### 1.4.1 Tools for klipper (KTCC-Klipper Tool Changer Code)

TypQxQ has created something here to provide a basic configuration. This is called "Tools for Klipper" (KTCC - Klipper Tool Changer Code).

> These are Python modules, macros, and example configurations for the Klipper 3D printer firmware to operate as a tool changer.

> In its simplest form, you need to specify the extruder, fan, and offset for each printhead. Then, add your macros for picking up, dropping off, locking, and unlocking tools.

> <cite><a href="https://github.com/TypQxQ/Klipper_ToolChanger">TypQxQ</a></cite>

#### 1.4.2 ROME 

The multi-extruder setup ROME by HelgeKeck, as discussed in `1.1.2 MMU`, has its own Klipper plugin created. This only needs to be installed and requires very little user input. [`GitHub repository ROME`](https://github.com/HelgeKeck/rome)

#### 1.4.3 Happy Hare

Happy Hare is a Universal MMU driver for Klipper. It simplifies the configuration and calibration of MMUs. Depending on the specific brand of your MMU, the calibration may vary slightly, although the steps are essentially the same for all brands. [`GitHub repository Happy Hare`](https://github.com/moggieuk/Happy-Hare)

#### 1.4.4 ERCF-Software-V3 aka "Happy Hare v1"

Klipper control software for the Enraged Rabit Carrot Feeder (ERCF v1.1) based on Happy Hare. [`GitHub repository ERCF-Software-V3`](https://github.com/moggieuk/Happy-Hare)



### 1.5 What methods can switch materials within 30 seconds?

---

To gain a better understanding of the discussed products, the key information has been summarized in a table. The time estimates are based on YouTube videos of the products, and due to variations in settings, the times are approximate. In the "Wipe tower" column, it is indicated whether the wipe tower consists of more than just a single line of plastic. In cases where "no" is listed, there may still be a wipe tower with a single line to ensure that the plastic flows normally, as oozing can cause plastic to flow out of the nozzle when it's not in use.

|         | Time    |Wipe Tower|  Costs|
|:--------|:-------:|--------:|-------:|
|Prusa MMU| >60 sec | Yes     | €329,- |
| ERCF    | >60 sec | Yes     | €150,- |
|----
|3DChameleon| >60 sec | Yes   | €220,- |
| A1 mini   | >90 sec | Yes   | €497,- |*
|----
|E3D Toolchanger| >30 sec | No| €2956,-|**
| Tapchanger    | >30 sec | No| €500,- |***
|=====
| Swapper3D| >30 sec | No     | €400,- |

|* Currently, can only be purchased in combination with the printer
|** Printer in combination with 4x direct drive extruder tool changers
|***Adding 4 tool changers

## 2 Program of requirements

The program of requirements is an important tool to kickstart the creative thinking process and ultimately define a final design.

### 2.1 Requirements

| No. | Requirements                                                     | Unit      | Source                         | Date       | Verification                |
| --- | --------------------------------------------------------------- | --------- | ------------------------------- | ---------- | ---------------------------- |
| 1   | 3D printing of 2 or more materials                             | Numbers   | Sven Dekker                    | 27-09-2023 | Performance after realization |
| 2   | Applicable to 2 or more 3D printers that may vary in size       | -         | Sven Dekker                    | 27-09-2023 | Assembly after realization   |
| 3   | Cost is less than €350                                          | Euro      | Sven Dekker, based on similar products | 27-09-2023 | Sum of costs of the final product only |
| 4   | Changing material takes less than 30 seconds                   | Seconds   | Sven Dekker                    | 27-09-2023 | Timing after realization     |
| 5   | Feasible for anyone with a 3D printer                           | -         | Sven Dekker                    | 27-09-2023 | Verification after realization |
| 6   | Open-source sharing of the project                               | -         | FabLab Waag                    | 27-09-2023 | Downloadable via Github      |
| 7   | Reliability so no user interaction is required during 3D printing | -       | Sven Dekker                    | 27-09-2023 | Checking interactions during print |
| 8   | 3D printer automatically calibrates when calibration is needed after initial setup | -       | Sven Dekker                    | 27-09-2023 | No manual calibration        |

### 2.2 Success criteria

| Requirement No. | Requirement                                                        |
| --------------- | ----------------------------------------------------------------- |
| 1               | The Multi-material addition can 3D print with as many materials as possible |
| 2               | The Multi-material addition can be mounted on as many printers as possible  |
| 5               | The Multi-material addition consists of as many 3D print components as possible |
| 7               | The Multi-material addition must be as reliable as possible          |
| 8               | The Multi-material addition requires as few user interactions as possible after installation on the printer, |

