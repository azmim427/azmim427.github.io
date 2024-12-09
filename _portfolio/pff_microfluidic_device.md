---
title: "Microfluidic Device"
excerpt: "Pinched flow fractionation microfluidic device."
header:
  image: /assets/img/microfluidic_dark.png
  teaser: /assets/img/microfluidic_dark.png
gallery:
  - url: /assets/img/IMG_0450.jpeg
    image_path: assets/img/IMG_0450.jpeg
    alt: "PDMS casted device with glass seal"
  - url: /assets/img/IMG_0653.jpeg
    image_path: assets/img/IMG_0653.jpeg
    alt: "resin printed device mold"
---
###### Designed by Mazyar Azmi

## Project description

* 3D printed flexible needlenose pliers
* Printed out of PLA and TPU
* Meant for picking up small through-hole resistors
* Parts were printed separately then hand pressed together (0.01mm gap)
* Degree of flexibility of TPU core was achieved by altering the slicing/infill patterns of the part and increasing/decreasing its density
* **Print-in-place models:** This part was initially designed to be compatible with a dual-nozzle 3D printer that printed the whole part in one go. Print-in-place describes parts that have mechanisms or other features that can be 3D printed without any further assembly, sometimes making previously impossible geometries possible. [Articulated joints](https://all3dp.com/2/coolest-print-in-place-3d-models/) and multimaterial parts are classic examples of the utility of print-in-place models. Multimaterial parts are especially suited for this process because of the poor adhesion that would normally occur between two very different materials like TPU and PLA. The main reason behind this lack of adhesion between TPU and PLA is due to the differing [surface energies](https://www.tstar.com/blog/bid/33845/surface-energy-of-plastics) of the two polymers. To achieve good adhesion between two plastics in FFF, they must have similar surface energies. Mechanically interlocking the parts using dual-extruder printing where the layers of one part overlap the layers of the other, or by using dovetail (or similar) joints, enables the manufacture of fully functioning multimaterial prints, like these pliers. Common types of mechanical connections in FFF include overlapping joints, encapsulation, or form-fit (e.g. dovetail) joints. Because the joints in this model are all two-dimensional, it is relatively simple to print the parts separately with an interference fit to press them in place. However, if you wanted a TPU part or layer bound to any complex 3D geometry, print-in-place is the only option.

{% include gallery %}

## Design specifications

* Jaw length: ~55mm
* Jaw capacity: ~8mm max
* Materials: 95A TPU, PLA
* Print settings:
  * 95A TPU core
    * Dovetail joint gap: 0.01mm total
    * 25% infill, grid pattern
      * 0 degree angle
    * 0 top or bottom horizontal walls
    * 6 vertical walls
  * PLA components
    * 8 vertical walls
    * 0 top or bottom horizontal walls
    * Gyroid infill, 20%
* Iteration notes:
  * Started with 4mm thick parts, ended with 6mm thick parts: more structurally stable (for the tpu core) which meant less undesired vertical movement of the tips.
  * Initial tpu core had no top or bottom shell walls, which was necessary for proper flex. However, the number of vertical walls and the percentage of infill changed throughout iterations. The earlier versions, which had only 3 vertical walls and ~12% infill, were far too flexible to provide consistent spring force against the compression of the pliers. The final version, with its 6mm thickness, 6 vertical walls, and ~25% infill, provided ample flexibility while also being much easier to use.
  * The original fit of the dovetail joints was too loose at 0.2mm, and the final version used a tighter fit at 0.01mm.
  * The initial design of the plier tips was a bit too wide, and made it slightly cumbersome for picking up small objects. This was fixed in the final version, making the plier more like a traditional needlenose pair.

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a476b64130524d1416?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
