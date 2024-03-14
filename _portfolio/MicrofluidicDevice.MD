---
title: "Microfluidic Device"
excerpt: "A plasma bonded microfluidic device made out of PDMS that was casted from a resin printed mold."
header:
  image: /assets/img/20240307_080959.jpg
  teaser: /assets/img/PDMuFluidicDevice.jpg
gallery:
  - image_path: assets/img/ResinMoldUFluidic.jpg
  - image_path: assets/img/PDMuFluidicDevice.jpg
  - image_path: assets/img/SideBySide.jpg
   
---

# Introduction to Microfluidic Devices

Microfluidic devices are systems that use small channels, with widths as small as 60 micrometers, to transport and mix various reagents together. The high surface to volume ratio of these devices generates surface tension that drives capillary action within the device induces the mixing process. Microfluidic devices are particularly relevant in medical diagnostics, DNA sequencing, tissue engineering, and environmental testing in which the microscale homogeneous mixing of reagents is critical.  



# Logic of Designing Microfluidic Devices

There are two principal ways to enhance mixing in microfluidic devices. Firstly, it is possible to increase surface area of the fluid’s path. On a microscopic scale, the flow of the fluids in these devices is laminar (smooth). In laminar flow some mixing occurs through molecular diffusion, which is inherently slow because it relies on the random movement of molecules over short distances. Thus, increasing cross-sectional area will increase the rate of diffusion. In these small devices, cross-sectional area can be optimized by increasing path length and splitting the fluidic flow into many subsections. Moreover, another way to optimize mixing in microfluidic devices, is to increase chaotic advection. Because the flow of fluids in these devices is laminar, to increase the fluid’s chaotic flow, designs can attempt to create microscale disturbances or structures in the flow. An important distinction to note is that turbulent mixing is a high-energy, large-scale phenomenon that does not occur in microfluidics, while chaotic advection also can induce chaotic flow, but on a smaller scale that is suitable for the small channels in the microfluidic device. Some of the decisions regarding the dimensions of the size of the geometries I used to create chaotic advection relied on the size constraints of the device. Specifically, the resolution of the printer was limited to 25 microns, there had to be two primary mixing sections in the device (by each team member), the aspect ratio had to be less that 4:1, and all geometries had to be at least 4 mm form the edge of the device. Nevertheless, my device utilizes multiple unique geometries to maximize surface area and chaotic advection of the fluid. 

![HI](/assets/img/SideBySide.jpg)

The first geometry I designed is an inclined twisting geometry. This geometry works in three dimensions and consequently causes the fluid to simultaneously flow from side-to-side and up-to-down as it travels forward throughout the device. This multiaxial motion induces chaotic mixing of the fluid. This geometry then diverts into the major two-part mixing section of the device. One piece of this primary mixing section utilizes intersecting channels. The intersecting channels geometry splits, rearranges, and recombines component streams. The design has a 1 mm thick rectangular boundary with small 0.25 mm parallel channels orthogonally dissecting it. Most of the fluid traverses the wider rectangular border path; however, small portions of it travel through the orthogonal channels, thereby enhancing chaotic advection. On the other side of this primary mixing section, the device uses an obstacle-based geometry. Specifically, wide extrusions that disrupt smooth forward flow greatly slow the mixing process and force the fluid to move through channels of varying widths. Finally, the ultimate mixing geometry of this side of the device is a simple zig-zag pattern, which is a common passive geometry in microfluidic devices due to its efficiency and simplicity. For this geometry the ration between the width and step size of the pattern determines the mixing efficiency. An optimal ratio of 4:1 between these parameters maximizes mixing efficiency. 

# Making the Device

* **Step 1 - Printing and Curing Resin Mold:** Stereolithography is a simple and rapid way to fabricate molds for microfluidic devices. Therefore, the mold for this microfluidic device was designed in CAD and printed using a Formlabs Fuse 3 SLA printer using high temperature resin. After printing the mold, the part was washed for 10 minutes in varying orientations to remove external clumps of uncured resin. The device was left to dry for 30 minutes, and once the mold had a homogeneous sheen, it was cured for five seconds without heat. This short cure time prevented the part from warping, which would inhibit the high resolution of the device’s design (which is a significant advantage of SLA) and subsequent steps in fabricating the microfluidic device.  
* **Step 2 - Parylene Deposition:** Many resins are not suitable for biomedical applications because uncured resin can leak out of the part and consequently change the composition of solutions and kill cells. Furthermore, resin printed parts are not suitable for elastomer polymerization because it inhibits curing, which impedes using resin in applications where fabricating flexible parts from polymers like PDMS is necessary. The most effective way to prevent these major limitations of resin printed parts is to deposit a thin layer of parylene along the surface of the model. This process enhances the biocompatibility of resin-based prints and allows them to be used as molds for elastomeric devices. 
* **Step 3 - Casting in PDMS:** Once this mold was casted in parylene to inhibit its cytotoxic qualities, the structures of the device was transferred to PDMS (an elastomeric, nonfragile, and transparent polymer) through casting. Specifically, to create this new PDMS mold, a PDMS-based solution was poured into the parylene coated mold and exposed to UV light to induce curing. The new PDMS mold was then removed from the resin mold. This process PDMS requires special care because, as previously mentioned, resin inhibits proper curing of PDMS. Leaching chemicals in the resin can destroy the catalysts responsible for inducing curing in PDMS.
* **Step 4 - Plasma Bonding PDMS Molds:** To close the new PDMS mold, the activated PDMS is irreversibly bonded to silicon-based materials like glass or silicon through surface activation by oxygen plasma treatment. The general principal of surface activation requires removing contaminants and generating reactive chemical species to induce covalent bonding. Specifically, plasma exposure causes the terminal methyl groups in PDMS can be replaced by silanol groups to form covalent silane bonds with adjacent molecules. 
In short, the process to make the functioning microfluidic device started with designing and manufacturing a mold using stereolithography. This mold was then covered in parylene. The coated mold was then casted in PDMS. Finally, this elastomeric form of the device was filled using oxygen plasma-based surface activation.



# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e4cdffd816f228146?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="Microfluidic Device" %}

