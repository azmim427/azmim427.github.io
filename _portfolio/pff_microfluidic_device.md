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
mathjax: true
---
###### Designed by Mazyar Azmi

## Project description

* Microfluidic device for pinched flow fractionation
* Mold printed out of clear resin and coated in parylene
* Cast in PDMS and sealed with glass slide
* Meant for separating particles that are 165 microns and 550 microns in size
* **Microfluidic Devices:**
  * Microfluidic devices are tools that manipulate and process small amounts of fluid through narrow channels. They are most commonly used in biomedical and pharmacalogical research, but can be found in any application that requires the transport, mixing, separating, or analysis of small volumes of fluids. The core principle that drives the function of these devices is the interactions between the fluid and the surface of the channels, also known as capillaries. At small volumes, these surface area interactions are very strong and can be utilized to manipulate the fluid in a desired way. One example of these interactions is chaotic advection (different from turbulent flow), or the phenomenon where individual fluid particles deviate from the straight laminar flow lines (fluids in microchambers experience mainly laminar flow if mixing isn't induced) due to underlying microscale disturbances or structures in the flow. Geometries like corners, chevrons, inclined mixers, obstacles, and intersections can all be used to evenly mix two separate fluids if desired. One application that requires such mixing is that of a biological assay where you have one solution of ligands, and one solution of antibodies, and the proper mixing of the two is necessary for them to bind. Another application that can be done entirely using channel geometries is sorting. Geometries for the passive sorting, or separation, of fluids often use sharp corners or narrow passages to accelerate all particles, but especially smaller particles. This varying acceleration allows the particles to sort themselves into different paths that can then lead to different outlets. One final consideration when manufacturing microfluidic devices is the fact that uncured resin monomers can leach out of the printed mold and interfere with the PDMS. This was prevented by coating the molds in a thin layer of parylene polymer to act as a barrier between the two materials.
* **Pinched flow fractionation:** This device works by the mechanism known as pinched flow fractionation, or PFF, to separate out particles of different sizes from a mixture. PFF allows for the continuous separation of varying size particles by bringing them through a narrow "pinched" channel and then out into a much wider channel, where the transition between the two results in smaller particles hugging the corner tighter than large particles, resulting in the two size particles sorting themselves into two different lanes in the wider channel, where they can then be separated and stored. There are some formulas available online that describe ideal input velocities, pinched channel widths, outlet channel widths, and final distance from the outlet channel wall that can be calculated using the particle diameters that you're interested in separating, which were 165 and 550 microns in this case. Unfortunately, the numbers I used must have been wrong because the final product doesn't actually separate the particles, but you can still see the forces involved in the video below.
* **Instructions to build:**
  * Start by resin printing the mold. This should be printed flat, i.e. the bottom surface should be parallel to the build plate so there are no layer lines on the surface.
  * Next, post process the mold while being careful not to touch or disturb the inside surface. Remove support material after 60 second cure.
  * Next, coat the print with 2 grams of parylene-C.
  * Pour PDMS into mold, degas in vacuum, and cure in oven before demolding.
  * Finally, bond PDMS device to glass microscope slide.

{% include video id="Y6jHMoRPzXk" provider="youtube" %}

{% include gallery %}

## Design specifications

* **Materials:**
  * Clear resin mold
  * Polydimethylsiloxane (PDMS) cast
  * Glass microscope slide
* **Geometry calculations:**
  * The widths of the pinched section and the outlet section were calculated using this formula:
  * $`Y_{0} = \left( {w_{\text{p}} - \frac{D}{2}} \right)\frac{{w_{0} }}{{w_{\text{p}} }}`$
  * $`Y_{0}`$ is the position of the particle in the outlet section (distance from wall)
  * $`{{w_{\text{p}} }}`$ is the width of the pinched section
  * $`{{w_{0} }}`$ is the width of the outlet section
  * $`D`$ is the diameter of the particle
 
$$
\begin{aligned} 
a^2 + b^2 &= c^2 \\ 
E &= M \cdot C^2 \\ 
&= xy + \mathbb{E} 
\end{aligned}
$$


## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a49618cb5b9c3e2d54?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
