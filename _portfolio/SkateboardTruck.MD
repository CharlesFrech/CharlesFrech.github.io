---
title: "Skateboard Truck Hanger"
excerpt: "A skateboard truck hanger created using generative design and manufactured using an SLS printer with Nylon 12 powder."
header:
  image: /assets/img/Screenshot 2024-04-21 150427.png
  teaser: /assets/img/IMG_3042.jpg
   
---

## Introduction to Generative Design and Powder Bed Fusion 

Powder bed fusion (also known as powder-based selective laser sintering, or pSLS) is an additive manufacturing process in which granular polymer powder is heated just below its melting point by a laser that traverses over its surface. The laser produces a small amount of energy that melts the powder into the desired geometry. For each successive layer, a thin layer of unfused powder is spread on top of the part. Moreover, generative design is an iterative design process that uses artificial intelligence to create a singular, lightweight geometry based on the constraints that a manufacturer assigns to the model. In this project, SLS and generative design were harnessed to create a truck hanger for an electric skateboard. The truck also incorporated a motor mount for an electric DC motor.

<img src="/assets/img/SLSPritners.jpg" alt="Image 3" style="display:flex; margin:auto;">

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Center Text</title>
<style>
  .center {
    text-align: center;
  }
</style>
</head>
<body>

<div class="center">
  <p><a href="https://alleghenyedusys.com/product/formlabs-fuse-1-3d-printer">Formlabs Fuse 1+ SLS printer</a></p>
</div>

</body>
</html>

## Pairing Powder Bed Fusion and Generative Design

The unique benefits of the SLS manufacturing process and the generative design modeling method can directly benefit one another. 

* **Benefit 1:** Firstly, generative design's ability to explore unconventional solutions and develop complex geometries that satisfy given constraints aligns with SLS’s capability to manufacture sophisticated shapes with high precision. This combination unlocks new design possibilities that were previously unattainable using conventional manufacturing methods like FFF or resin printing. This benefit is very relevant in aerospace and automotive applications. For example, many components of cars and planes need to be lightweight to optimize fuel efficiency. Thus, a manufacturer in one of these industries can use generative design to create complex geometries for these parts. Then, they can subsequently leverage the high precision manufacturing capabilities of SLS to manufacture the design. 

<img src="/assets/img/Screenshot 2024-04-21 195813.png" alt="Image 3" style="display:flex; margin:auto;">

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Center Text</title>
<style>
  .center {
    text-align: center;
  }
</style>
</head>
<body>

<div class="center">
  <p><a href="https://3dprintingindustry.com/news/hexcel-makes-boeings-qualified-provider-list-for-3d-printed-aircraft-components-160887/">Examples of SLS-printed aircraft parts with complex geometries</a></p>
</div>

</body>
</html>

* **Benefit 2:** Moreover, pairing SLS and generative design has the potential to minimize material waste. The Fusion 360 generative design feature has a specific option that  directs the algorithm to minimize material usage. If a manufacturer wants to minimize material usage, SLS is an ideal additive manufacturing technique to utilize because it does not require support material for overhangs. Rather, the loose powder in the powder bed is sufficient to hold the growing part.  In aviation and automation, designing intricate components like turbines is an example of coupling these tools together. In 2017, Siemens, a manufacturing company, developed a turbine engine, manufactured entirely using SLS. There are many parts in this device with unique shapes and structures that would typically require support material if manufactured with other 3D-printing techniques. However, with SLS, this model required no support material.

<img src="/assets/img/Screenshot 2024-04-21 203736.png" alt="Image 3" style="display:flex; margin:auto;">

<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Center Text</title>
<style>
  .center {
    text-align: center;
  }
</style>
</head>
<body>

<div class="center">
  <p><a href="https://www.3yourmind.com/news/functional-motorized-3d-printed-turbine-model-for-siemens">Siemiens turbine engine</a></p>
</div>

</body>
</html>


* **Benefit 3:** Furthermore, a manufacturer can apply many different materials to a single generative design process. Thus, many parts made from different materials can be generated under the same loading conditions. This particular advantage of generative design was leveraged in this skateboard truck project. Specifically, two trucks were ultimately digitally generated: one made from Nylon 12 (see first photo below) and one from ALSi10Mg (see second photo below). SLS, as a manufacturing method, is compatible with a wide variety of materials with diverse mechanical properties. Thus, the capability to design with different materials and produce models with different materials manifests a further reason why these technologies can be paired. In the automotive and aeronautical industries, manufacturers must test a wide variety of materials when designing exterior components to optimize impact resistance, energy absorption, rigidity, and deformation characteristics.

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
      <img src="/assets/img/Screenshot 2024-04-21 152504.png" alt="Image 1">
      <img src="/assets/img/Screenshot 2024-04-21 152306.png" alt="Image 2">
</div>

</body>
</html>

* **Benefit 4:** Finally, a fourth benefit that directly couples these two technologies is the opportunity to maximize manufacturing productivity. Generative design finds creative solutions to problems humans might otherwise overlook, which can save time and resources during the creative process. Furthermore, SLS is particularly advantageous compared to other additive manufacturing techniques because manufacturing time does not scale with print volume. Because SLS is an iterative process that manufactures parts on a layer-by-layer basis, it is suitable for batch processing, and it is the fastest 3D-pritning technology when the build volume is packed appropriately. Thus, the coupling of this software and hardware can directly optimize manufacturing processes. 

<img src="/assets/img/Screenshot 2024-04-21 195941.png" alt="Image 3" style="display:flex; margin:auto;">


<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Center Text</title>
<style>
  .center {
    text-align: center;
  }
</style>
</head>
<body>

<div class="center">
    <p><a href="https://3dprintingindustry.com/news/materialise-and-eos-become-first-to-3d-print-flight-ready-sls-parts-for-airbus-190816/">SLS Airplane Parts Printer Factory</a></p>
</div>

</body>
</html>

## Reflection on Generative Design

The generative design process is most useful in applications where multiple complex solutions to a problem that satisfy various loading constraints are required. Therefore, when coupled with additive manufacturing techniques like SLS, generative design can be particularly useful in the automotive and aeronautical industries (see above discussion). As a biomedical engineer, I am curious how this technology will grow concurrently with novel methods additive tissue engineering. I predict that in the future, generative design will be able to generate sophisticated tissue geometries that can be subsequently manufactured with novel additive manufacturing techniques. Nevertheless, generative design does have flaws. Firstly, it is very complex and requires a lot of practice to fully grasp. When designing the skateboard truck mount, I was initially very confused about how to leverage different obstacles and preserve geometry features to direct the AI into building my final part. However, through extensive practice during this project, I learned how to effectively design obstacles (red structures in the below images) and preserve gemotries (green structures) to guide the algorithm into building a part that satisfied the constraints of the truck hanger. 

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
      <img src="/assets/img/Screenshot 2024-04-21 150721.png" alt="Image 1">
      <img src="/assets/img/Screenshot 2024-04-21 150704.png" alt="Image 2">
</div>

</body>
</html>

Additionally, the generative design model required a strong fundamental understanding of forces and loading constraints, which might be a challenge for many engineers. In my final model, I used the following loading conditions:

| Forces/Moments           | Magnitude | Direction                       |
| ----------------|:---------:|--------------------------------:|
| Weight Force of Rider | 880 N     | Downwards (direction of gravity)|
| Shear Forces Pair 1 | 200 N     | Orthogonal to weight force|
| Shear Force Pair 2 | 200 N     | Upwards and downwards     |
| Pulley Tension Force | 200 N     | Orthogonal to wight force towards rod |
| Motor Mount Moment 1 | 8 Nm | Resisitve to side-to-side motion of mount |
| Motor Mount Moment 2 | 8 Nm | Motor spinning direction/resistive to up-and-down motion of mount |

Finally, the generative design process was often slow to produce models. Thus, I think there is little benefit of generative design to individual projects that can be solved using traditional CAD practices. However, for individuals or companies that are manufacturing sophisticated or interconnected parts, I appreciate the power of leveraging this technology. 

## CAD Models
* **Aluminum Truck**
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6ee8f8ee9f2c9f51c9?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

* **Nylon 12 Truck**
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e857fb08e66e8bf80?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Attributions

All information about generative design and SLS printing is attributed to the lecture material of Dr. David Florian. All images not of the model are attributed to the links attached to the image.

## Gallery

<img src="/assets/img/Screenshot 2024-04-21 193419.png" alt="Image 3" style="display:flex; margin:auto;">

<img src="/assets/img/Screenshot 2024-04-21 150427.png" alt="Image 3" style="display:flex; margin:auto;">

<img src="/assets/img/IMG_3044.jpg" alt="Image 3" style="display:flex; margin:auto;">

<img src="/assets/img/IMG_3043.jpg" alt="Image 3" style="display:flex; margin:auto;">

<img src="/assets/img/IMG_3042.jpg" alt="Image 3" style="display:flex; margin:auto;">
