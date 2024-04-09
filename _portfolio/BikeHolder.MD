---
title: "Bike Phone Holder"
excerpt: "A multi-material and multi-component phone holder for a bike with a handlebar diameter ranging from 23 to 25 mm."
header:
  image: /assets/img/20240307_080959.jpg
  teaser: /assets/img/PDMuFluidicDevice.jpg
gallery:
  - image_path: assets/img/SideBySide.jpg
   
---

## Introduction to Top-Down Modeling

Top-down modeling is a design strategy in which the manufacturer starts by creating the overall assembly file and subsequently builds each part component in this singular file. This approach is different compared to bottom-up modeling in which the sub-components are designed separately and ultimately composed in a separate parent assembly file. This secondary strategy was used in the multi-material pliers and syringe pump CAD modeling processes. The traditional bottom-up process is desirable for smaller models with few components. However, top-down assembling should be leveraged with highly complex models with many components. It allows manufacturers to create and modify certain parts with respect to other ones in one file instead of having to analyze many multiple separate files. Furthermore, top-down modeling also allows for easy parametrization of dimensions, which further optimizes the speed and efficiency of the designing process.

## Rationale Behind the Design

Top-down modeling was used when designing this bike-specific phone holder because many separate, connecting components were needed to make this assembly. The first step of the design process was to create a makeshift representation of the handlebars (a simple cylinder with a 25 mm diameter) and to import a model of a phone (an iPhone 15 pro was used in this model). Next, these two bodies were oriented to mimic how the final device would function and look like a physical model, and they were subsequently grounded. With these two fixed molds, the four major components of the model were designed.  

![alt text](/assets/img/Screenshot 2024-03-19 201747.png "Strategies to Increase Diffusion")

Moreover, another way to optimize mixing in microfluidic devices is to increase chaotic advection. Because the flow of fluids in these devices is laminar, mixing can be enhanced by creating microscale disturbances in the smooth flow. An important distinction to note regarding microscale mixing is that turbulent mixing is a high-energy, large-scale phenomenon that does not occur in microfluidics. Chaotic advection induces chaotic flow, but on a smaller scale that is suitable for the small channels in the microfluidic device. 

<img src="/assets/img/Screenshot 2024-03-19 201821.png" style="display:flex; margin:auto;">

Some of the decisions regarding the dimensions of the geometries used in the device relied on the constraints of the manufacturing process. Specifically, the resolution of the printer was limited to 25 micrometers, there had to be two primary mixing sections in the device (one by each team member), the aspect ratio had to be less than 4:1, and all geometries had to be at least 4 mm from the edge of the device. Nevertheless, through creative design techniques, this device utilizes multiple unique geometries that maximize diffusion and chaotic advection of the fluid.

## The Device

* **Part 1: To attach the phone holder to the handlebars, a cylindrical base was first designed. This base had a 0.1 mm tolerance with a 24 mm handlebar. Furthermore, this piece contained two extrusions. One side of the model had a rectangular extrusion with two holes that match the diameter of M5 screws. The extrusion was orthogonal to the model and was split into two sections. The total length of the upper and lower blocks (including the gap between) is 16 mm, thereby manifesting this model is compatible with for a 16 mm M5 screw. This adjustable extrusion allows for this handlebar connector to be suitable with a variety of handlebar sizes. The second extrusion of this piece is a rectangular prism with a 10-degree taper (thereby making it trapezoidal). This extrusion is angle at 45 degrees from the horizontal plane dissecting the connector, which was determined to be an optimal angle for the phone’s visibility to the biker. This trapezoidal extrusion has two bumps at its end to enhance the phone case’s connection to this piece. This piece was printed out of PLA because of its necessary tensile strength and impact resistance.

* **Part 2: The second piece of this assembly was a phone case. On the backside of the case, which has a thickness of 2 mm, there is a tapered rectangular extrusion to connect to the angled extrusion. This tapered designed of the male and female connections of the handlebar connector and the phone case optimizes the attachment between these two components. The female connection on the phone case has outward cutouts that match the bumps on the male connector with a clearance of 0.1 mm. The motivation behind his outward extrusion design is its simplicity. Compared to a ball-and-socket or screw mechanism, this push-and-pull mechanism is suitable for imprecision in 3D printing, and it still allows a biker to quickly adjust the orientation of their phone. This component was printed out of TPU because this elastic material is more susceptible to morphing. This capacity to was necessary because it enhanced the case’s connection to the tapered PLA insert as well as the fit of the phone in the case.

* **Parts 3/4: The final two components of this assembly were lids that were attached into the top and bottom of the phone case. These pieces enhanced the phone’s security in the case. The lids were printed out of PLA because of this plastic’s rigidity and quick printing. 

![alt text](/assets/img/Screenshot 2024-03-14 171945.png "Geometries on Second Half of Device")

## Assembilng the Device

To assemble the model, the user first slides the connector onto the handlebar and screws in the M5 screws. They next attach the case to the angled extrusion on the handlebar connector in the desired orientation. They finally set the phone in the case and ensure its stability by inserting the lids. 

![alt text](/assets/img/ResinMoldUFluidic.jpg "Resin Mold")

## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e40ad6560210ab50b?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Attributions

The CAD model of the iPhone 15 Pro is attributed to Travis Llado and can be found [here](https://grabcad.com/library/iphone-15-pro-1).

{% include gallery caption="Side-By-Side Comparison of Resin and PDMS Molds" %}


