---
title: "Multimaterial Pliers"
excerpt: "A print-in-place pair of pliers 3-D printed with elastic TPU and rigid PLA."
header:
  image: /assets/img/PliersTopImage.png
  teaser: /assets/img/PliersHeaderImage.png
gallery:
  - image_path: assets/img/SideBySide.jpg
   
---

## Introduction to Print-in-Place Parts

Print-in-place 3D printing refers to the process of creating objects with multiple components or movable parts as a single piece. This methodology effectively eliminates the process of assembling multiple prints to create one final part. An example of a single material print in place part is a bolt lock, which requires an internal feature that can slide and subsequently extend outwards to create a barrier. Furthermore, print-in-place parts can also be multi-material. An example of a multi-material print-in-place part is a lead screw bearing block, which couples high strength and rigid material with a flexible, low wear filament into a single part. 

Print-in-Place Bolt Lock|Print-in-Place Multi-Material Bearing Block
--|--
![](/assets/img/Screenshot 2024-03-31 211111.png)|![](/assets/img/Screenshot 2024-03-31 213312.png)

## Printing Multi-Material Parts

For two separate plastics to effectively bond together, they must have similar qualities. Firstly, they must have surface energy, which determines how much they flow upon extrusion. Next, they must have similar chemical properties. Highly polar polymers with a net dipole moment are unlikely to bond well with a long, non-polar polymer chain. Thirdly, the polymers should have similar shrinkage and cooling rates. A discrepancy in this property will cause separation between layers if the printed parts warp. Finally, the materials should have relatively similar mechanical properties. However, this quality is less important than the other aforementioned characteristics. Therefore, it is possible to print a multi-material part with a flexible filament and a rigid polymer. Some combinations of polymers that work well together include PLA and TPU, PLA and PVA, and ABS and HIPS. 

![alt text](/assets/img/Screenshot 2024-03-19 201747.png "Strategies to Increase Diffusion")

## The Model

The final model of the multi-material pliers had five pieces: two legs, two jaws, and a flexible body. The legs and jaws were 3D-printed with rigid PLA and the body was printed with flexible TPU. The legs were designed to mimic commercial pliers. They had circular bases and interior extrusions to allow for a better grip on the pliers. The jaws were angled so that they would get closer to each other with increasing length. The final length of the pliers that was chosen ensured the distance between their tips was approximately 3 mm when the pliers were in the un-clamped position.  

![alt text](/assets/img/ElasticPieces.png)

The central flexible component is a square with three t-shaped extrusions on each side (see image). These “teeth” slot into similar cutouts on the pliers and legs. This mechanism restrained the spring in the model. The clearance between the teeth and the cutouts ranged from 0.1 to 0.2 mm. To maximize the flexibility of this piece, a grid design was used with thin walls. The thin walls of the grid design were susceptible to significant bending  after force was applied to the legs.

![alt text](/assets/img/ElasticPieces.png)

## Design Process

I designed two models of pliers. In both iterations, the design of the jaws and the leg components stayed the same, while the flexible piece changed. In the first model, the depth of the matrix and its border was offset from this piece’s outward extrusions that connected to the jaws and legs. This decision stemmed from the fact that thinner geometries are more flexible and have higher capacity to translate the clamping motion on the legs to the jaws. However, this model was flawed because the depth between the flexible grid and the attachment extrusions was too great. Therefore, when the legs were squeezed with different amounts of force, which occurred when the pliers were operated with one hand, the legs were prone to bending inwards. 

![](/assets/img/Multimaterial Pliers Version 1 (failure)- Made with Clipchamp.gif)

Nevertheless, the pliers worked very well when used with two hands because the forces on each leg were approximately equivalent. To address this challenge, the next iteration only offset the flexible grid, not its border (see above image of grids). This design also decreased the thickness of the matrix, thereby making the component more flexible. This design worked much better and addressed the imbalance issue. However, this model also had a flaw. Specifically, a different filament was used for this second flexible component. The filament of the first iteration had a much higher Young’s Modulus compared to the filament used for the second model, which also explains why  the second design was much more flexible. However, this added flexibility affected the connection between the flexible piece and the legs and pliers. The approximate 0.1 to 0.2 mm clearance between these pieces, which worked very well for this first iteration, was less effective with the more elastic filament. Nevertheless, this added flexibility unlocked a new feature for the pliers. Specifically, this second model of the pliers had the capability to readily open and close, thereby increasing the plier’s jaw capacity. 

Iteration 1|Iteration 2
--|--
![](/assets/img/Multimaterial Pliers Version 1 - Made with Clipchamp.gif)|![](/assets/img/Multimaterial Pliers Version 2.gif)

The legs, pliers, and body were designed as separate bodies in CAD and printed separately using a Voron single extrusion printer. Nevertheless, an assembly file was created that coupled all these bodies together that would allow someone to print these pliers using a dual-extrusion printer. Some notable print settings to control if using a dual-extrusion printer are temperature, speed, and layer height. These parameters ensure that the differences in surface energy, mechanical properties, chemical attributes, and cooling rates are minimized so that proper adhesion between different components can be ensured.

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e76906e8ae02228d5?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Attributions

All images not of the device are attributed to the lecture material of Dr. David Florian.

{% include gallery caption="Side-By-Side Comparison of Resin and PDMS Molds" %}


