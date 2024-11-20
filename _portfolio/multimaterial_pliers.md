---
title: "Multimaterial Pliers"
excerpt: "Fully 3D printed needlenose pliers."
header:
  image: /assets/img/pliers_render_final.png
  teaser: /assets/img/pliers_render_final.png
gallery:
  - url: /assets/img/IMG_0549.jpeg
    image_path: assets/img/IMG_0549.jpeg
    alt: "real life 3D printed needlenose pliers"
  - url: /assets/img/IMG_0558.gif
    image_path: assets/img/IMG_0558.gif
    alt: "gif of pliers working"
  - url: /assets/img/IMG_0566.jpeg
    image_path: assets/img/IMG_0566.jpeg
    alt: "iterations of tpu core"
---
###### Designed by Mazyar Azmi

## Project description

* 3D printed flexible needlenose pliers
* Printed out of PLA and TPU
* Meant for picking up small through-hole resistors
* Parts were printed separately then hand pressed together (0.01mm gap)
* Degree of flexibility of TPU core was achieved by altering the slicing/infill patterns of the part and increasing/decreasing its density
* **Print-in-place models:** This part was initially designed to be compatible with a dual-nozzle 3D printer that printed the whole part in one go. Print-in-place describes parts that have mechanisms or other features that can be 3D printed without any further assembly, sometimes making previously impossible geometries possible. Articulated joints and multimaterial parts are classic examples of the utility of print-in-place models. Multimaterial parts are especially suited for this process because of the poor adhesion that would normally occur between two very different materials like TPU and PLA. Mechanically interlocking the parts using dual-extruder printing where the layers of one part overlap the layers of the other, or by using dovetail (or similar) joints, enables the manufacture of fully functioning multimaterial prints, like these pliers.

{% include gallery %}

## Design specifications

* Jaw length: ~55mm
* Jaw capacity: ~8mm
* Materials: 95A TPU, PLA
* Iteration notes:
  * Started with 4mm thick parts, ended with 6mm thick parts: more structurally stable (for the tpu core)
  * Initial tpu core had no top or bottom shell walls, which was necessary for proper flex. However, the number of vertical walls and the percentage of infill changed throughout iterations. The earlier versions, which had only 3 vertical walls and ~12% infill, were far too flexible to provide consistent spring force against the compression of the pliers. The final version, with its 6mm thickness, 8 vertical walls, and ~25% infill, provided ample flexibility while also being much easier to use.
  * The original fit of the dovetail joints was too loose at 0.2mm, and the final version used a tighter fit at 0.01mm.

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a476b64130524d1416?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
