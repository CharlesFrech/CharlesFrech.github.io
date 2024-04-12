---
title: "Bike Phone Holder"
excerpt: "A multi-material and multi-component phone holder for a bike with a handlebar diameter ranging from 23 to 25 mm."
header:
  image: /assets/img/ScreenShotmoldRendering.png
  teaser: /assets/img/IMG_5274 (2).jpg
   
---

## Introduction to Top-Down Modeling

Top-down modeling is a design strategy in which the manufacturer first creates the overall assembly file and subsequently makes each component in this singular file. This approach is different compared to bottom-up modeling, in which the sub-components are first designed separately and subsequently compiled in a single parent assembly file. This secondary strategy was used in the [multi-material pliers](https://charlesfrech.github.io/portfolio/MultiMaterialPliers/) and [syringe pump](https://charlesfrech.github.io/portfolio/SyringePump/) CAD modeling processes. The traditional bottom-up process is desirable for smaller models with few components. However, top-down modeling should be leveraged with highly complex designs with many components. It allows manufacturers to create and modify certain parts with respect to other ones in one file instead of having to analyze multiple separate files. Furthermore, top-down modeling also allows for easy parametrization of dimensions, which can optimize the speed and efficiency of the fabrication process.

<img src="/assets/img/TopdownSchematic.png" style="display:flex; margin:auto;">
<span class="image-title">[Schematic of Top-Down vs. Bottom-Up Designing](https://mungfali.com/post/791E71B031352D66F4C66ADE9CE802C28A96754E)</span>

## Rationale Behind the Design

Top-down modeling was used when designing this bike-specific phone holder because many separate, connecting components were needed to make this assembly. The first step of the design process was to create a makeshift representation of the handlebars (a simple cylinder with a 24 mm diameter) and to import a model of a phone (an iPhone 15 Pro was used in this model). Next, these two bodies were oriented to mimic how the final, physical device would function and look. With these two objects, the four major components of the model were designed.  

## The Device

* Part 1: To attach the phone holder to the handlebars, a cylindrical base was first designed. This base had a 0.1 mm tolerance with the handlebar, which had a diameter of 24 mm. Furthermore, this piece had two extrusions. One side of the model had a rectangular extrusion with two holes that matched the diameter of M5 bolts. The extrusion was orthogonal to the model and was split into two sections. The total length of the upper and lower blocks (including the gap between) was 16 mm, thereby demonstrating this model was compatible with a 16 mm M5 bolt. The M5 bolts were locked with two M5 nuts. This adjustable extrusion allowed for this handlebar connector to be suitable with a variety of handlebar sizes. A major issue with this part was its obscure geometry, which required excessive support material during the 3D printing process. Therefore, the final surface of the part was rough and stringy. Nevertheless, its functionality was not hindered. Future iterations of this model will break up this obscure piece into more simplistic components to minimize the probability of a print failure and enhance the surface finish of the final model.
<img src="/assets/img/HandleBarSideProfile.png" style="display:flex; margin:auto;">

The second extrusion of this handlebar connector was a rectangular prism with a 10-degree taper (thereby making it trapezoidal). This extrusion was angled at 45 degrees from the screw holes, which was determined to be an optimal angle for the phone’s visibility to the biker. This trapezoidal extrusion had two bumps at its end to enhance the phone case’s connection to this piece. This piece was printed out of PLA because of its necessary tensile strength and impact resistance. Additionally, the PLA material choice allows for a user to input M5 heat set inserts as an alternative mechanism to adjust the diameter of the connector (TPU is not compatible with heat set inserts).

<img src="/assets/img/HandlebarConnectorNubFaceProfile.png" style="display:flex; margin:auto;">

* Part 2: The second piece of this assembly was a phone case. On the backside of the case, which had a thickness of 2 mm, there was a tapered rectangular extrusion to connect to the angled extrusion on the handlebars. This tapered design optimized the attachment between the male and female connections of the handlebar connector and the phone case. The female connection on the phone case had outward cutouts that match the bumps on the male connector. The motivation behind this outward extrusion design is its simplicity. Compared to a ball-and-socket or screw mechanism, this push-and-pull mechanism is suitable for imprecision in 3D printing, and it allows a biker to quickly adjust the orientation of their phone. The phone case also had slits at each of its ends, in which the lid components were inserted.

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Images Side by Side</title>
<style>
    .image-container {
        display: flex;
        justify-content: center;
    }
    .image-container img {
        width: 50%; /* Adjust as needed */
        height: auto;
        margin: 0 10px;
    }
</style>
</head>
<body>

<div class="image-container">
      <img src="/assets/img/LidInsertProfile.png" alt="Image 1">
      <img src="/assets/img/CaseOutsideFaceProfile.png" alt="Image 2">
</div>

</body>
</html>

<img src="/assets/img/CaseSideProfile.png" alt="Image 3" style="display:flex; margin:auto;">

This component was printed out of TPU because this elastic material is more susceptible to morphing. This capacity was necessary because it enhanced the case’s connection to the tapered PLA insert, the fit of the phone in the case, and the case's link with the lids.

* Parts 3/4: The final two components of this assembly were the lids, which were inserted into the aforementioned top and bottom slits of the phone case. These pieces enhanced the phone’s security in the case because they were printed out of PLA, which is rigid and has minimal deformation under low stresses. 

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Images Side by Side</title>
<style>
    .image-container {
        display: flex;
        justify-content: center;
    }
    .image-container img {
        width: 50%; /* Adjust as needed */
        height: auto;
        margin: 0 10px;
    }
</style>
</head>
<body>

<div class="image-container">
    <img src="/assets/img/LidsFaceProfile.png" alt="Image 1">
    <img src="/assets/img/LidsOutwardProfile.png" alt="Image 2">
</div>

</body>
</html>

## Assembilng the Device

To assemble the model, the user first slides the connector onto the handlebar and locks the M5 with two compatible M5 nuts. The biker will next attach the case to the angled extrusion on the handlebar connector in the desired orientation. They finally set the phone in the case and ensure its stability by inserting the lids. 

## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e40ad6560210ab50b?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Attributions

The CAD model of the iPhone 15 Pro is attributed to Travis Llado and can be found [here](https://grabcad.com/library/iphone-15-pro-1). All images not of the model are attributed to the links attached to the image.

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
    <img src="/assets/img/FullAsseblyUpwardsSide.png" alt="Gallery Image 1" title="Image of Assembly Side (Vertical)">
    <img src="/assets/img/FullAssemblyLandscapeBack.png" alt="Gallery Image 2" title="Image of Assembly Back (Horizontal)">
    <img src="/assets/img/FullAssemblyLandscapeSide.png" alt="Gallery Image 3" title="Image of Assembly Side (Horizontal)">
    <img src="/assets/img/FullyAssemblyUpwardsFront.png" alt="Image of Assembly Front (Vertical)">
    <img src="/assets/img/FullAssemblyUpwardsBack.png" alt="Gallery Image 4" title="Image of Assembly Back (Vertical)">
    <img src="/assets/img/IMG_5277.jpg" alt="Assembly on Bike 1">
    <img src="/assets/img/IMG_5275.jpg" alt="Assembly on Bike 2">
    <img src="/assets/img/IMG_5278.jpg" alt="Assembly on Bike 3">
</body>
</html>
