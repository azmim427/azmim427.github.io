---
title: "Generative Skateboard Truck"
excerpt: "Motorized skateboard truck designed with generative AI."
header:
  image: /assets/img/skateboard_assembly.png
  teaser: /assets/img/skateboard_assembly.png
gallery:
  - url: /assets/img/IMG_0688.jpeg
    image_path: assets/img/IMG_0688.jpeg
    alt: "irl truck on skateboard"
---
###### Designed by Mazyar Azmi

## Project description

* SLS 3D printed motorized skateboard truck designed with generative AI
* Printed out of Nylon 12 powder on Formlabs Fuse

{% include gallery %}

* **Generative design:** Generative design is the use of powerful computer algorithms to optimize the structure of a part, allowing for lighter weight, less components, and lower cost. Using simulations that take force scenarios as inputs, generative design can output new design concepts that surpass all other designs in balancing strength and weight, but the drawback is that these designs are impossible to machine by traditional methods due to their flowing and organic topology. Instead, the ideal way to manufacture these parts is through additive manufacturing processes like powder bed fusion, or SLS. PBF is an additive manufacturing techinique that uses a laser or electron beam to selectively fuse powdered material to form a component layer by layer. Because PBF doesn't require additional supports or tooling, combining it with generative design allows for an almost perfectly optimized manufacturing pipeline with minimal waste. PBF can work with high-strength materials like nylon 12 or metal alloys, allowing for almost any strength part to be manufactured. This is most useful in aerospace and automotive applications where any extra weight savings can cut costs by a fortune. My favorite example is the [Czinger 21C](https://czinger.com/revolutionary-technology), a hybrid hypercar with truly astonishing performance thanks to generative optimization of its components.
* **Load case rationale:** Load cases are the force scenarios that you feed into the generative algorithm before it can return a design. If you know the magnitude and direction of a force you need the part to withstand, you can simply input it on the surface that it will be acting on. The generative design process involves simulations of these forces against the mechanical properties of the material you chose, and requires several cycles of iteration before the final product. The load cases I chose were all based around a fixed constraint on the pivot joint. This isn't necessarily ideal because, in reality, the part is supposed to move, which means that the clearances for the turning of the truck needed to be set by hand. ChatGPT helped me come up with these values and magnitudes, but it took a lot of tweaking to get right. I started with a downward load of 1000N on the pivot joint face, kingpin hole, and axle to simulate the static load of a rider, as well as a 20N downward force and a 20N moment on the motor mounting plate to simulate its weight as well. Next, I added a 2000N upward force on the pivot joint face, kingpin hole, and axle to simulate the force of a bump or impact. Next, I added one 500N moment on the kingpin hole faces for turning in both directions, to simulate the force of the bushings on the truck. Next, I added an asymmetrical 1000N upward force on each end of the axle separately, to simulate the force of a bump on only one wheel. Next, I calculated the torque of the motor, and added a force of 250N in both directions of the direction of travel of the pulley to simulate this. Next, I added forward and backward forces of 300N on the pivot joint and kingpin hole. Finally, I added left and right turning forces of 200N on the pivot joint and kingpin hole. To simulate the forces that the motor exterts on the motor plate during turning, I added a 50N moment in each direction.
* **Comparing nylon and aluminum models:** For this design, Fusion 360 outputted generative models in both nylon 12 (pSLS) and ALSi10Mg (mSLS). With the forces I provided, the nylon version ended up very bulky but the aluminum version always came out pretty small. For example, the material connecting the nylon motor mount to the rest of the truck is so large that it wraps around half of the motor, but for the aluminum it only needed about a finger's width worth of material.
* **A critique of generative design:** Personally, I am very impressed by the technology. While it could have been easier to use, ease of use really isn't the point. The purpose of generative design is to make stronger and lighter parts that serve the same purpose, so it's okay if it takes a little more iteration to get the design right. As someone who has almost no experience with forces, load cases, or manufacturing, I struggled a little bit with brainstorming what kind of forces I needed this part to survive, but I think I got there in the end (with more than a little help from ChatGPT). I think if I were to use this technology again, I would spend significantly more time setting up the obstacle geometry at the beginning. I incorrectly assumed that the software would be more lenient with this, but it turns out it tries to use every millimeter of available space. Whether or not I correctly inputted the forces is yet to be seen, but I don't think that makes generative design an inviable solution, just a little bit of a slower one that requires some real world trial and error.

## CAD Models

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a43c7f44200515f9c3?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a47351caef4adb1351?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
