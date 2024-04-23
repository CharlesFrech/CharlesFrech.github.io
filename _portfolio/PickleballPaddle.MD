---
title: "Pickleball Paddle"
excerpt: "A multi-material 3D-printed pickleball paddle optimized for a player who incorporates power and control into their play."
header:
  image: /assets/img/RenderedFullPaddle.png
  teaser: /assets/img/Screenshot 2024-04-21 103038.png
gallery:
  - image_path: assets/img/PaddleFullProfileFlat.jpg
   
---

## The Design

This pickleball paddle was designed in Fusion 360 using a top-down modeling approach because this model had many interconnected components. The total length of the paddle and handle was 33.79 cm, and the maximum width of the paddle was 17.40 cm. These dimensions satisfy the size requirements of a pickle paddle according to Section 2.E.3 of the [USA Pickleball Official Rulebook](https://usapickleball.org/docs/USA-Pickleball-Official-Rulebook-2024-v1.pdf). While this paddle is smaller than standard, this design decision stemmed from intentional efforts to optimize weight distribution in the paddle (see below discussion). Furthermore, the smaller paddle size increased the maneuverability of the paddle. The paddle and handle were both printed out of rigid PLA, and the paddle’s surface is smooth; it contains no delamination, holes, cracks, or indentations. The paddle has two M4 heatset inserts on its base profile. There are also two holes on the handle, which allow the handle to attach to the paddle using two 12 mm M4 hex bolts. 

<img src="/assets/img/RenderedPaddle.png" style="display:flex; margin:auto;">

<img src="/assets/img/ScrewPaddleProfileUpdated.png" style="display:flex; margin:auto;">

## TPU Handle

The pickleball paddle also includes a flexible handle to improve the player’s grip. This element, printed using highly flexible TPU95 from Polymaker, has a curved elliptical pattern of extrusions. This pattern models the exact displacement between my knuckles. 

<img src="/assets/img/PaddleSideProfile.jpg" style="display:flex; margin:auto;"> 

The grip also has three distinct 4 mm circular extrusions. The hole in the center entirely dissects the handle and the TPU to the heat set inserts that attach the paddle to the handle. The two holes adjacent to this center hole run approximately halfway through the TPU grip, and they also allow for two PLA rods to be inserted. Although the TPU insert has no tolerance with the handle, and consequently has an extremely tight fight, these rods provide additional support to ensure the insert remains within the handle.  With further iterations, the TPU guard will be modeled so that it can be removable. With the current design, the only way to remove the guard is to break the PLA rods, which is wasteful and inefficient. 

<img src="/assets/img/RenderedTPUGrip.png" style="display:flex; margin:auto;"> 

## Edge Guard

The paddle also contained a one-piece edge guard to protect the face of the paddle when contact is made with the ground. The edge guard was also printed using highly flexible TPU95 from Polymaker. TPU was used because of its shock absorbing capabilities, its ability to morph when attached to other components, particularly rigid ones, and the need to print this part in one piece. The rigid paddle has eight rectangular inward extrusions along its outside with a 5-degree taper angle. The edge guard has matching outward extrusions, with a 5-degree taper, which inserts directly into the paddle. The edge guard has a 1.5 mm overhang on both sides of the paddle. While this component is very effective, it does not entirely fit into each hole on the paddle. This flaw is likely due to the printer’s inability to print with the precision that was modeled in the CAD file. Furthermore, some irremovable support material obstructed the fit. 

<img src="/assets/img/EdgeGuardDelamination.jpg" style="display:flex; margin:auto;"> 

## Optimizing the Weight of the Paddle

The weight of the paddle was optimized for a player who likes to use power and control in their game. To achieve this desired quality, the paddle was printed with 20% infill with an adjusted five layers of solid layers on the top and bottom of the paddle. When a player hits the ball, the energy from the swing is directly transferred to the ball. However, with sparse infill, much of this energy transfer is lost within the paddle, which consequently limits the player’s capability to return shots with high power. However, with too high an infill percentage, the mass of the paddle becomes too heavy and limits the capability of agile play. Thus, the decision to use a low infill percentage, but a high number of solid layers on the paddle’s perimeter attempted to effectively minimize weight without effecting swing power. The handle was printed with 15% infill, making the handle lighter than the paddle. The TPU elements weighed approximately 20 grams. Thus, the total amount of filament used was approximately 230 grams (8.1 ounces). This weight balance suggests that this paddle is effective for a power-oriented player. However, coupled with its easier maneuverability, due to its smaller size, it is also effective for an agile and controlled player. 

## CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e4483548c63010b6f?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Image of Fully-Assembled Paddle" %}


