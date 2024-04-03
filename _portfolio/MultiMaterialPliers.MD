---
title: "Multi-Material Pliers"
excerpt: "A print-in-place pair of pliers 3-D printed with elastic TPU and rigid PLA."
header:
  image: /assets/img/PliersTopImage.png
  teaser: /assets/img/PliersHeaderImage.png


   
---

## Introduction to Print-in-Place Parts

Print-in-place 3D printing refers to the process of creating objects with multiple components or movable parts as a single piece. This methodology effectively eliminates the need to assemble multiple separate prints to create one final part. It also allows for more sophisticated parts to be manufactured with internal complex geometries. An example of a single material print-in-place part is a bolt lock, which requires an internal feature that can slide and subsequently extend outwards to create a barrier. Furthermore, print-in-place parts can also be multi-material. An example of a multi-material print-in-place part is a flange bearing. The pictures bearing couples high strength and rigid material with a flexible, low wear filament into a single part. The manufacturer consequently claims this part is suitable in a variety of machines in agricultural, robotic, and food-machinery applications. 

[Print-in-Place Bolt Lock](https://www.pinterest.com/pin/359936195224395037/)|[Print-in-Place Multi-Material Bearings](https://www.igus.com/info/bolt-flange-bearings)
--|--
![](/assets/img/Screenshot 2024-03-31 211111.png)|![](/assets/img/MMFlangeBearing.png)

## Printing Multi-Material Parts

For two separate plastics to effectively bond together, they must have similar qualities. Firstly, they must have similar surface energies, which determines how much they flow upon extrusion. Next, they must have similar chemical properties. Highly polar polymers with a net dipole moment are unlikely to bond well with a long, non-polar polymer chain. Thirdly, the polymers should have similar shrinkage and cooling rates. A discrepancy in this property will cause separation between layers if the printed parts warp. Finally, the materials should have relatively similar mechanical properties. However, this quality is less important than the other aforementioned characteristics. Therefore, it is possible to print a multi-material part with a flexible filament and a rigid polymer. Some combinations of polymers that work well together include PLA and TPU, PLA and PVA, and ABS and HIPS. 

## The Final Model

The final model of the multi-material pliers had five pieces: two legs, two jaws, and a flexible body. The legs and jaws were 3D-printed with rigid PLA and the body was printed with flexible TPU. The geometry of legs was designed to mimic commercial pliers. They had circular bases and interior extrusions to allow for a better grip on the pliers. The jaws were angled so that they would get closer to each other with increasing length. The final length of the pliers that was chosen ensured the distance between their tips was approximately 3 mm when the pliers were in the un-clamped position.  

![alt text](/assets/img/PliersImage.png)

The central flexible component is a square with three t-shaped extrusions on each side (see image). These “teeth” slot into similar cutouts on the pliers and legs. This mechanism restrained the spring in the model. The clearance between the teeth and the cutouts ranged from 0.1 to 0.2 mm. To maximize the flexibility of this piece, a grid design was used with thin walls. The thin walls of the grid design were susceptible to significant bending after force was applied to the legs.

![alt text](/assets/img/ElasticPieces.png)

## Design Process

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Centered GIFs</title>
<style>
  .container {
    text-align: center;
  }
</style>
</head>
<body>

<div class="container">
  <img src="/assets/img/Multimaterial Pliers Version 1 - Made with Clipchamp.gif" alt="GIF 1">
  <img src="/assets/img/UpdatedPliers2Motion.gif" alt="GIF 2">
</div>

</body>
</html>

Two models of pliers were built. In both iterations, the design of the jaws and the leg components stayed the same, while the flexible piece changed. In the first model, the depth of the flexible matrix and its border was offset from this piece’s outward extrusions that connected to the jaws and legs. This decision stemmed from the fact that thinner geometries are more flexible and have higher capacity to translate the clamping motion on the legs to the jaws. However, this model was flawed because the depth between the flexible grid and the attachment extrusions was too great. Therefore, when the legs were squeezed with different amounts of force, which occurred when the pliers were operated with one hand, the legs were prone to bending inwards. 

<img src="/assets/img/Multimaterial Pliers Version 1 (failure)- Made with Clipchamp.gif" style="display:flex; margin:auto;">

Nevertheless, the pliers worked very well when used with two hands because the forces on each leg were approximately equivalent. To address this challenge, the next iteration only offset the flexible grid, not its border (see above image of grids). This design also decreased the thickness of the matrix, thereby making the component more flexible. This design worked much better and addressed the imbalance issue. However, this model also had a flaw. Specifically, a different filament was used for this second flexible component. The filament of the first iteration had a much higher Young’s Modulus compared to the filament used for the second model, which also explains why the second design was much more flexible. However, this added flexibility affected the connection between the flexible piece and the legs and pliers. The approximate 0.1 to 0.2 mm clearance between these pieces, which worked very well for this first iteration, was less effective with the more elastic filament. Nevertheless, this added flexibility unlocked a new feature for the pliers. Specifically, this second model of the pliers had the capability to readily open and close, thereby increasing the plier’s jaw capacity (see above motion .GIF). 

<img src="/assets/img/Plier2Failure (1).jpg" style="display:flex; margin:auto;">

## Testing the Pliers

To test the quality of the designs, each plier needed to be able to pick up a through-hole resistor. As the .GIFS below demonstrate, both models of these pliers passed this test.

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Centered GIFs</title>
<style>
  .container {
    text-align: center;
  }
</style>
</head>
<body>

<div class="container">
  <img src="/assets/img/UpdatedPliers1Resistor.gif" alt="GIF 1">
  <img src="/assets/img/UpdatedPliers2Resistor.gif" alt="GIF 2">
</div>

</body>
</html>

## Final Considerations

The legs, pliers, and body were designed as separate bodies in CAD and printed separately using a Voron single extrusion printer. Nevertheless, an assembly file was created that coupled all these bodies together that would allow someone to print these pliers using a dual-extrusion printer. Some notable print settings to control if using a dual-extrusion printer are temperature, speed, and layer height. These parameters ensure that the differences in surface energy, mechanical properties, chemical attributes, and cooling rates are minimized so that proper adhesion between different materials can be ensured.

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e76906e8ae02228d5?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Attributions

All information about multi-material printing is attributed to the lecture material of Dr. David Florian. All images not of the pliers are attributed to the links attached to the images above.

## Gallery

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Four Images</title>
</head>
<style>
  .container {
    text-align: center;
  }
  img {
      margin-bottom: 20px;
  }
</style>
<body>
    <img src="/assets/img/PliersJawsGallery.png" alt="Gallery Image 1" title="Image of Jaws">
    <img src="/assets/img/PlierLegsGallery.png" alt="Gallery Image 2" title="Image of Legs">
    <img src="/assets/img/Plier1Gallery.png" alt="Gallery Image 3" title="Image of First Iteration Pliers">
    <img src="/assets/img/Plier2Gallery.png" alt="Gallery Image 4 title="Image of Second Iteration Pliers">
</body>
</html>
