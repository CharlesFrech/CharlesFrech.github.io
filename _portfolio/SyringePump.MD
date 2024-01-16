---
title: "Syringe Pump"
excerpt: "A stepper motor driven syringe pump primarily made of 3D printed parts with a precise flow rate and compatiblity with syringes of ranging volumes."
header:
  image: /assets/img/Screenshot 2024-01-14 124656.png
  teaser: /assets/img/FromAfarSP.jpg
gallery:
  - image_path: assets/img/FromAfarSP.jpg
  - image_path: assets/img/ElectricalSP.jpg
  - image_path: assets/img/AerialSP.jpg
  - image_path: assets/img/Screenshot 2024-01-15 173428.png
   
---

# Features/Design Elements

* **Custom Parts:** The final device had many custom components. Firstly, three custom mounts were manufactured to hold the syringe's body, plunger, and tip. These components were dimensioned with respect to a large 20 mL syringe with zero tolerance to provide a tight fit that would eliminate any chance of wobbling and rotating in the yaw or pitch direction. A separate custom end support was constructed to limit the carriage's backward motion to prevent it from interfering with the flexible coupler. Moreover, to protect the model's electronics from water and finger intrusion, the model also had an electronic enclosure. The enclosure was precisely dimensioned to fit the breadboard, Arduino, power supply box, and all the wiring. Finally, a motor mount was designed to attach a NEMA 17 stepper motor to the model. All these custom parts were designed in Fusion 360. The syringe mounts, electronic enclosure, and end supports were 3D printed out of PLA. The motor mounting plate was printed out of ABS because of its ability to resist significant softening. This precaution was necessary because the motor generated heat. 
* **Electrical Components:** In addition to the breadboard, Arduino, and power supply box, the syringe pump contained one latching push button, two non-latching push buttons, one multicolored LED, and one limit switch. When the latching push button was pressed, the LED became green, and the carriage holding the syringe's plunger traversed away from the motor. When the latching push button was unpressed, the LED turned yellow, and the carriage stopped moving. When the syringe was fully emptied, the carriage was designed to press the limit switch. As a result of this contact, the motion of the motor stopped, and the LED turned red. Finally, when the left push button was pressed, the syringe moved backwards to the starting position. Once far enough back, a newly loaded syringe could be set into the device. When the right push button was held, the syringe moved away from the motor, in the forward direction, at a constant rate. These buttons allowed for quick and easy adjustment of the carriage's position before starting the pump.
* **Programming:** The syringe was programmed using the Arduino IDE. The program first initialized variables for the motor, flow rate, speed, syringe diameter, lead screw pitch, button inputs (including the limit switch), and LED inputs. The setup function initially received an input max speed and subsequently set a fixed speed based on the user's desired flow rate. In the loop of the function, the base color values of the LED were preset to be zero so that they could be updated later. Then, the start/stop button was checked. If the latching button was pressed, then the speed was set using a function that converted flow rate to speed. The LED also changed to green. If the latching button was not pressed, the program set the speed to 0, and the LED values were updated to a yellow color to signify that the motor was paused. Next, the program checked if the counterclockwise non-latching button was pressed; if so, the speed was set to a negative constant so that the syringe moved backwards. Then, the limit switch was checked. If the limit switch was pressed, the speed was set to 0, and the LED values were assigned to red color values. The limit switch was checked after the counterclockwise button so the syringe could move backwards even if the limit switch was pressed. Finally, the program checked if the clockwise button was pressed. If so, the speed was set to a constant. This button was checked after the limit switch so the carriage would not run into other components on the model. Lastly, the final LED values were translated to the LED pins, and the run speeds were sent to the stepper motor. The complete code for the code can be found [here](https://github.com/CharlesFrech/SyringePump/blob/master/main/main.ino).


# Off the Shelf Parts

|      Part                                                            |     Quantity            |
| ---------------------------------------------------------------------|:--------------------------:|
| [250 mm lead screw with 2 mm pitch and 8 mm lead](https://amzn.to/3infwI0)                      | 1 |
| [1/4" x 8 mm flexible coupler](https://openbuildspartstore.com/1-4-x-8mm-flexible-coupling/)                                         | 1                   |
| [200 mm linear rod with 8 mm diameter](https://www.amazon.com/dp/B07MPGWJMS/ref=cm_sw_em_r_mt_dp_X5AQS0ES7JH8JG83AAZ3)                                 | 1                   |  
| [LMUU linear bearing for 8 mm diameter rod](https://www.amazon.com/gp/product/B087WPGQ8T/ref=ppx_yo_dt_b_asin_image_o00_s00?ie=UTF8&psc=1)                             | 1                   | 
| [20 x 40 V-Slot aluminum linear rail](https://openbuildspartstore.com/v-slot-20x40-linear-rail/)                                  | 1                   | 
| [NEMA 17 stepper motor](https://www.amazon.com/gp/product/B07LF898KN/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&th=1)                                                | 1                   | 
| [MEAN WELL RQ-65D AC-DC quad output power supply](https://www.amazon.com/dp/B005T9HGLI/ref=cm_sw_em_r_mt_dp_A8CZ056TM52EJGZTGZGR?_encoding=UTF8&psc=1) | 1                 | 
| [Arduino Uno](https://www.amazon.com/dp/B007R9TUJE/ref=cm_sw_em_r_mt_dp_TY8JGK0CJD1JEJM4BNNJ)                                                          | 1                   | 
| [A4988 stepper driver](https://www.amazon.com/dp/B01FFGAKK8/ref=cm_sw_em_r_mt_dp_V0YKTYKDWMR8WHTKA53T?_encoding=UTF8&psc=1)                                                 | 1                   | 
| [REXQualist 400-point breadboard](https://www.amazon.com/dp/B082VYXDF1/ref=cm_sw_em_r_mt_dp_N6Q28CAGPAYCKCSJKDDC?_encoding=UTF8&psc=1)                                      | 1                   | 
| [Panel mount latching push buttons](https://amzn.to/3VxQ29h)                                    | 1                   | 
| [Panel mount non-latching push buttons](https://www.amazon.com/Non-Latching-Momentary-Non-Locking-Normally-oorbell/dp/B0B63PT9PB/ref=sr_1_3adgrpid=1331510951630385&dib=eyJ2IjoiMSJ9.LrB4lPX7ZtipmPMcUgqllMQjLafqyAYwHec6e_WH49-H3N4f4GCO6cAlj_O5UEgP8XDJW64eJnWlgiH6OH6Rz9IQxmqY-zIuQ2hYwyNc7u0-PdK3c4xwU38_j_ZPFE4a3ki6KGEwp3HCvmGGg1e_iA.WlLBeu58unGL-fJ_7WYOiImrYylo8l2mhe_YpN0LTEo&dib_tag=se&hvadid=83219689318242&hvbmt=bp&hvdev=c&hvlocphy=83973&hvnetw=o&hvqmt=p&hvtargid=kwd-83220462151988%3Aloc-190&hydadcr=7664_13467799&keywords=non+latching+push+button&qid=1705252826&sr=8-3)                                    | 2            | 
| [Limit switch](https://www.amazon.com/gp/product/B073TYWX86/ref=ppx_yo_dt_b_asin_image_o01_s00?ie=UTF8&psc=1)                                                         | 1                  | 
| [RGB common cathode LED](https://www.amazon.com/dp/B0194Y6MW2/ref=cm_sw_em_r_mt_dp_FW3CFQT7ZGFQ2R04N6G3?_encoding=UTF8&psc=1)                                               | 1                   | 
| [F688ZZ flange ball bearing](https://www.amazon.com/uxcell-Bearing-8x16x5mm-Shielded-Bearings/dp/B07RVHTY3V/ref=sr_1_4?crid=17UOU208N0O6F&dib=eyJ2IjoiMSJ9.HOTRTml3NQ0GPksGnan0AGR_ZrBvAsHZDZIoFXeNkJUnm-Y7qAfxgFtQRODDs4BHl3lyCcqZF6tDDubJQ_6YcuOlp6or0hGFGhEKgltzqkSTSrqXSLjCqh4yMK2-ASnS2JMq0S9UtflWCBr-DovT6A.FHSc0qN8xVYI7WmieDQ8KQicMlXriLO6b6dwLTyHBIA&dib_tag=se&keywords=f688zz%2Bflanged%2Bbearings&qid=1705259259&sprefix=f688zz%2Bflanged%2Bbearings%2Caps%2C78&sr=8-4&th=1)                                               | 2                   | 
| [Closed lock collar for lead screw](https://www.amazon.com/Befenybay-Collar-Shaft-Screw-Printer/dp/B07V41FRZS/ref=sr_1_7_sspa?adgrpid=1334808468938516&dib=eyJ2IjoiMSJ9.BGJaFDPaBWdW9TI9SqbWf_WtLOCunnxYj6tvXCLaQT62a6CAMWn0zdnSrJWk8Xg8SvCvqtA87HpjbQA5txjOd7T32sKzA2Fp2_DX0dBiK9DOiPCxlMhDKF6SoNI67epE-LNRK7AQraAwQ_hO2zZcsw.SP_wFTwcTRiAT3X_LD_eFoZMRUn1veldQxwBD3J61OA&dib_tag=se&hvadid=83425722910178&hvbmt=be&hvdev=c&hvlocphy=83973&hvnetw=o&hvqmt=e&hvtargid=kwd-83426418357563%3Aloc-190&hydadcr=951_1014987053&keywords=8mm%2Block%2Bcollar&qid=1705259520&s=industrial&sr=1-7-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9tdGY&th=1)                                               | 2                   | 
| [Open lock collar for linear rod](https://www.amazon.com/10PCS-Shaft-Collar-Aluminum-Linear/dp/B0C46G8G1R/ref=sr_1_4?crid=1UHY2GPNTBI60&dib=eyJ2IjoiMSJ9.Z4VFK7TCNkQVh6ZSSoBEDDt7yQi93S6YVeA6kHIQea_7zQ7Ttgalkgt18mbeFgWAJdnhIjSctNspfIGbRoHQDfqUTvkUShsk2fWDLT8ww9f0m5QixwMSYwthMgkI-5DOqpEXEJgBaAmqAoVO0m1qfw.9o3Ft8QwFqLbCMHWCr7MB9d6XibN7guKKHFYlRWI4xY&dib_tag=se&keywords=8mm%2Block%2Bcollar%2Blinear%2Brod&qid=1705259641&s=industrial&sprefix=8mm%2Block%2Bcollar%2Blinear%2Bro%2Cindustrial%2C87&sr=1-4&th=1)    | 2                   | 
| [Tr8x8 brass nut](https://www.amazon.com/2-Pack-Thread-Starts-Printer-Machine/dp/B09F2WGTH7/ref=sr_1_62?asc_source=01HFY6QA7Q8N1TT2Z879WGSZ46&tag=snx79-20&th=1)                                                 | 1                   | 
| M3 x 8 mm thread forming screws                                                 | 4          | 
| M3 x 10 mm bolt                                               | 4                   | 
| M5 Tee-Nut                                             | 8                   | 
| M5 x 8 mm bolt                                                 | 8                | 
| Electrical components including wires and resistors                  | Varies depending on wiring schematic                 | 

# Custom Designed Parts

|      Custom Part                                                     |      
| ---------------------------------------------------------------------|
| [Carriage (Syringe Plunger Support)](https://a360.co/47Aw03m)        |
| [Syringe Tip End Support](https://a360.co/3tYjexW)                   | 
| [LED Mount](https://a360.co/48zgJBd)                                 | 
| [Syringe Body Middle Mounting Plate](https://a360.co/3tZfLz9)        |
| [NEMA 17 Motor Mounting Plate](https://a360.co/421cKeA)              | 
| [Left End Mount](https://a360.co/3vHa9tQ)                            | 
| [Electronics Enclosure Lid](https://a360.co/3U2tiRc)                 | 
| [Electronics Enclosure Box](https://a360.co/3vtpgqM)                 | 

# Instructions for Operation

To operate the pump, the user first loaded the syringe. The outward extrusions on the syringe (i.e. the holders designed for human fingers) fit into the middle support. The tip of the syringe was rested on the end support, facing away from the motor. Finally, the end part of the syringe's plunger was placed in the extrusion located near the top edge of the carriage. Then, the person operating the device was safely able to plug it in to turn it on. The user could press the latching button, which serves as a start/stop button, to start the syringe pump. The LED would turn green, and the device would begin dispensing liquid. If the user pressed the latching button again, the motor would stop moving, and the LED would turn yellow. Finally, when the carriage holding the syringe hit the limit switch on the middle mount, the motor stopped, and the LED turned red. This outcome occured when the syringe was empty. The design also contained two additional buttons that changed the direction of the motor’s rotation. Because the motor cpuld rotate clockwise and counterclockwise, the syringe could partially fill and expel liquids using these buttons at a constant rate. A user operated this multi-directional pump feature by simply holding one of the two buttons. A video of the operational syringe pump can be found [here](https://drive.google.com/drive/folders/1s0FM1NEmiLGKT7h9kciig2gYD0h-9A-2?usp=sharing).

# CAD Model
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e10515e96ce3f04fe?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="3D-Printed Syringe Pump" %}

