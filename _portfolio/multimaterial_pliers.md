---
title: "Multimaterial Pliers"
excerpt: "Fully 3D printed needlenose pliers."
header:
  image: /assets/img/pliers_render_final.png
  teaser: /assets/img/pliers_render_final.png
gallery:
  - url: /assets/img/syringe_pump_photo.jpg
    image_path: assets/img/syringe_pump_photo.jpg
    alt: "real life assembly of the syringe pump"
    title: "title"
  - url: /assets/img/syringe_pump_drawing.png
    image_path: assets/img/syringe_pump_drawing.png
    alt: "drawing of the syringe pump body"
    title: "title"
  - url: /assets/img/syringe_pump_circuit.jpg
    image_path: assets/img/syringe_pump_circuit.jpg
    alt: "diagram of the syringe pump's wiring circuit"
    title: "title"
---
##### Designed by Mazyar Azmi

## Project description

* **Capable of a wide range of flow rates from 1-100 mL/min.** Using arduino controlled stepper motor coupled to 8mm lead screw.
* **3 modes of operation to choose from.** Choose between entering your desired flow rate in mL/min, entering your desired volume in mL, or controlling the motor manually using the buttons.
* **Swappable syringe sizes.** Choose to pump from either a 10 or 20 mL syringe.
* **LCD Display.** Informs the user about the device’s current state.
* **Limit switch.** Automatically stops motor when syringe is out of fluid.
* **3D printed enclosure.** To protect electronic components from spills.

Blurb about print-in-place models

{% include gallery %}

## Off-the-shelf parts required

| Part Name | Quantity |
|-----------|----------|
| 250 mm lead screw with 2 mm pitch and 2 mm lead | 1 |
| 250 mm lead screw with 2 mm pitch and 8 mm lead | 1 |
| 1/4" x 8mm Flexible Coupling | 1 |
| 200 mm linear rod with 8 mm diameter | 2 |
| LM8UU Linear bearing for 8 mm diameter rod | 2 |
| 2040 Aluminum Extrusion 1' Length | 1 |
| Nema 17 Stepper Motor | 1 |
| MEAN WELL RQ-65D AC-DC Power Supply Quad Output 5V 12V 24V 12V 4 Amp | 1 |
| Arduino Uno | 1 |
| A4988 Stepper Driver | 1 |
| Small Breadboard | 1 |
| Panel Mount Latching Push Buttons (On/Off) | 1 |
| Panel Mount Momentary Push Buttons | 2 |
| Limit Switch | 1 |
| Rotary Encoder | 1 |
| RGB Common Cathode LED | 1 |

## 3D printed parts required

| Part Name | Quantity |
|-----------|----------|
| Motor Mount| 1 |
| Back Barrel Stabilizer | 1 |
| Plunger Presser | 1 |
| Front Barrel Stabilizer | 1 |
| End Support | 1 |
| Enclosure | 1 |
| Enclosure Lid | 1 |


## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a476b64130524d1416?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Instructions

1. Use the two momentary buttons to move the plunger presser far back enough for the length of the syringe with its plunger extended. Put the back part of the syringe in the slot on the back barrel stabilizer. Adjust the presser with the momentary buttons as needed.
2. Advance the plunger presser until it makes contact with the syringe using the forwards and backwards buttons.
3. Press both buttons simultaneously to slowly advance the plunger. 
4. Use the knob and button on the screen to set syringe size and select operation mode. There are two options for operation mode. If “ml/min” is selected, a flow rate can be specified and the toggle switch can be clicked once to start pumping and again to stop. If “ml” is selected, the amount to pump in ml can be specified and the rotary encoder button can be pressed to start pumping. The pump will stop automatically once the required volume of liquid is pumped. If the limit switch is pressed during operation, the pump will warn the user that they have run out of space. The machine will then proceed to move backward into a safe position and reset itself. There is also a small reset button on the screen that resets the program if the syringe size needs to be changed out.
5. Switch out the syringe as desired.

## [Arduino Code](/assets/img/syringe_pump_code.ino)

