---
title: "Microfluidic Device"
excerpt: "A plasma bonded microfluidic device made out of PDMS that was casted from a resin printed mold."
header:
  image: /assets/img/20240307_080959.jpg
  teaser: /assets/img/PDMuFluidicDevice.jpg
gallery:
  - image_path: assets/img/SideBySide.jpg
   
---

# Introduction to Microfluidic Devices

Microfluidic devices are systems that use small channels, with widths as small as 60 micrometers, to transport and mix various reagents together. Microfluidic devices are particularly relevant in medical diagnostics, DNA sequencing, tissue engineering, and environmental testing in which the microscale homogeneous mixing of reagents and direct manipulation of cellular spatial organization are critical. Furthermore, these devices can also be used to generate droplets (which is relevant in single cell analysis). A major challenge of mixing in microfluidics results from the microscale mechanisms within the devices. Fluids behave very differently in microscale systems than macroscale ones. Therefore, these devices require creative and complex design elements to optimize mixing.  

# Logic of Designing Microfluidic Devices

There are two principal ways to enhance microscale mixing in microfluidic devices. Firstly, it is possible to increase diffusion. The flow of the fluids in microfluidic devices is laminar (smooth). In laminar flow some mixing occurs through molecular diffusion, which is inherently slow because it relies on the random movement of molecules over short distances. Thus, increasing cross-sectional area will increase the rate of diffusion. In these small devices, diffusion (and consequently mixing) can be enhanced by increasing cross-sectional area. This parameter can be directly optimized by increasing path length and splitting the fluidic flow into many subsections. 

![alt text](/assets/img/Screenshot 2024-03-19 201747.png "Strategies to Increase Diffusion")

Moreover, another way to optimize mixing in microfluidic devices, is to increase chaotic advection. Because the flow of fluids in these devices is laminar, mixing can be enhanced by creating microscale disturbances in the flow. An important distinction to note regarding microscale mixing is that turbulent mixing is a high-energy, large-scale phenomenon that does not occur in microfluidics. Chaotic advection also can induce chaotic flow, but on a smaller scale that is suitable for the small channels in the microfluidic device. 

![alt text](/assets/img/Screenshot 2024-03-19 201821.png "Methods to Increase Chaortic Advection")

Some of the decisions regarding the dimensions of the geometries we used in the device to enhance diffusion and chaotic advection relied on the constraints of the manufacturing process. Specifically, the resolution of the printer was limited to 25 micrometers, there had to be two primary mixing sections in the device (one by each team member), the aspect ratio had to be less than 4:1, and all geometries had to be at least 4 mm from the edge of the device. Nevertheless, through creative design techniques, this device also utilizes multiple unique geometries that maximize diffusion and chaotic advection of the fluid.

# The Device

The first section of this microfluidic device utilizes four primary design choices: branched paths, obstacles, paths with ridges, and sharp corners. These four geometries augment diffusion and chaotic advection in the device, thereby inducing mixing. Referencing the image below, this first part of the device starts with a serpentine path followed by a branched structure that splits into eight roads. These roads vary in width, which, as previously noted, increases the cross-sectional area of the path and consequently increases the greater rate of diffusion. The serpentine path also includes ridged channels with a height of 250 micrometers to induce chaotic flow. This large width heightens the rate of diffusion, and the ridged channels allow for the fluid to split up and subsequently rejoin, thereby directly fostering mixing. The next primary geometry in this first mixing section includes obstacles. The approximate 20 obstacles in each of the aforementioned eight roads further induces chaotic flow by disrupting the fluid's forward smooth flow. It is important to note that this section of the device had a couple flaws. Specifically, because this section of the device had an overabundance of roads, not all of the paths were utilized for mixing, leading to dead zones. Nevertheless, for the fluid that did travel along the obstacle path, mixing was augmented effectively.

![alt text](/assets/img/Screenshot 2024-03-17 031522.png "Geometries on First Half of Device")

Moreover, the first geometry the second section of the mixing device contains is an inclined twisting geometry. This geometry works in three dimensions and consequently causes the fluid to simultaneously flow from side-to-side and up-to-down as it travels forward throughout the device. This multiaxial motion fosters chaotic advection. This geometry then diverts into the major two-part mixing section of this side of the device. One piece of this primary mixing section utilizes intersecting channels. This intersecting channel geometry splits, rearranges, and recombines component streams. The design has a 1 mm thick rectangular boundary with small 0.25 mm parallel channels orthogonally dissecting it. Most of the fluid traverses the wider rectangular border path; however, small portions of it travel through the orthogonal channels, thereby facilitating mixing through diffusion. The amount of mixing is directly related to the number of intersecting channels and the thickness of these channels. On the other side of this primary mixing section, the device uses an obstacle-based geometry. Specifically, wide extrusions that disrupt smooth forward flow greatly slow the mixing process and force the fluid to move through channels of varying widths. The final mixing geometry of this part of the device is a simple zig-zag pattern, which is a common passive geometry in microfluidic devices due to its efficiency and simplicity. For this geometry the ratio between the width and step size of the pattern determines the mixing efficiency. 

![alt text](/assets/img/Screenshot 2024-03-14 171945.png "Geometries on Second Half of Device")

# Making the Device

* **Step 1 - Printing and Curing Resin Mold:** Stereolithography is a simple and rapid way to fabricate molds for microfluidic devices. Therefore, the mold for this microfluidic device was designed in CAD and printed using a Formlabs Form 3 SLA printer using high temperature resin (see image below). After printing the mold, the part was washed for 10 minutes in varying orientations to remove external clumps of uncured resin. The device was left to dry for 30 minutes, and once the mold had a homogeneous sheen, it was cured for five seconds without heat. This short cure time prevented the part from warping, which would inhibit the high resolution of the device’s design (which is a significant advantage of SLA) and hinder subsequent sealing steps during the fabrication process.  

![alt text](/assets/img/ResinMoldUFluidic.jpg "Resin Mold")

* **Step 2 - Parylene Deposition:** Many resins are not suitable for biomedical applications because uncured resin can leak out of the part and consequently change the composition of solutions and kill cells. Furthermore, resin printed parts are not suitable for elastomer polymerization because it inhibits curing, which impedes using resin in applications where fabricating flexible parts from polymers like PDMS is necessary. A simple and effective way to prevent these major limitations of resin printed parts is to deposit a thin layer of parylene along the surface of the model. This process enhances the cytocompatibility of resin-based prints and allows them to be used as molds for elastomeric casting. 
* **Step 3 - Casting in PDMS:** Once this mold was casted in parylene to inhibit its cytotoxic qualities, the device's features were transferred to a PDMS mold (an elastomeric, nonfragile, and transparent polymer) through casting. Specifically, to create this new PDMS mold, a PDMS-based solution was poured onto the parylene coated mold and cured. The new PDMS mold was then removed from the resin mold.
* **Step 4 - Plasma Bonding PDMS Molds:** To seal the new PDMS mold, the activated PDMS can be irreversibly bonded to silicon-based materials like glass or silicon through surface activation by oxygen plasma treatment. Specifically, surface activation requires removing contaminants and generating reactive chemical species to induce covalent bonding. Specifically, plasma exposure causes the terminal methyl groups in PDMS to be replaced by silanol groups to form covalent silane bonds with adjacent molecules. The final, sealed PDMS device is shown below.

![alt text](/assets/img/PDMuFluidicDevice.jpg "Final PDMS Device")

# Video

[Here](https://youtu.be/6WT70_s9AQU) is a video of the functioning final microfluidic device at the volumetric flow rate of approximately 1 mL/min. For the sake of speed and efficiency, at the timestamp 1:45, the volumetric flow rate was increased.

# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e4cdffd816f228146?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

#Attributions

All images not of the device are attributed to the lecture material of Dr. David Florian. Information regarding the device fabrication process was primarily drawn from the scientifc paper "Lab on a Chip: Rapid prototyping of cell culture microdevices using parylene-coated 3D prints." This paper can be accessed at this [link](https://doi.org/10.1039/D1LC00744K).

{% include gallery caption="Side-By-Side Comparison of Resin and PDMS Molds" %}

