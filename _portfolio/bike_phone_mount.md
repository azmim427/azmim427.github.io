---
title: "Bicycle Phone Mount"
excerpt: "Bicycle phone mount for iPhone 13 mini."
header:
  image: /assets/img/bike_phone_mount_render.png
  teaser: /assets/img/bike_phone_mount_render.png
gallery:
  - url: /assets/img/IMG_0636.jpeg
    image_path: assets/img/IMG_0636.jpeg
    alt: "IRL phone mount (portrait)"
  - url: /assets/img/IMG_0937.jpeg
    image_path: assets/img/IMG_0937.jpeg
    alt: "Phone mount with phone attached"
  - url: /assets/img/IMG_0648.jpeg
    image_path: assets/img/IMG_0648.jpeg
    alt: "IRL phone mount (landscape)"
---
###### Designed by Mazyar Azmi

## Project description

* SLS 3D printed bicycle phone mount for iPhone 13 mini
* Printed out of Nylon 12 powder on Formlabs Fuse
* Meant for 23-25mm diameter bicycle handlebars
* Ball joint allows for switching between landscape/portrait orientation
* **Top-down modeling:** The top-down design method of assembly is the easiest way to assemble multiple components into one assembly file in Fusion 360. Unlike the traditional method of making each component separately and then inserting them into an assembly design where each part has to be joined to the next, top-down modeling allows for every single component to be started and finished inside the same file, which permits the use of projections to other parts and skips the lengthy joining process. 
* **Assembly instructions:**
  * First, insert the four short heat-set inserts into the holes in the front half of the clamp.
  * Next, place the ball joint in its socket and tighten it down.
  * Next, insert the longer heat-set insert into the hole in the ball joint.
  * Finally, screw the phone grips to the ball joint and clamp the mount to the handlebars.
* **Design Rationale:** I wanted this design to be as small as possible with no more moving parts than necessary. Therefore, I chose a four armed gripper geometry for the part of the mount that interfaces with the phone, which provides a very sturdy yet simple solution to the problem. The ball joint can be tightened down or loosened depending on whether or not you need to adjust the angle of the phone, and it always allows for some play regardless of how tight it is (but it doesn't flop around). The clamp is very adjustable and can be secured to various diameter handlebars, even over 25mm.
* **Material Choice:** Nylon 12 powder printing allows for much more robust and durable parts than traditional FFF printing, which is necessary for the phone grip geometry I chose, which relies on mechanical force rather than moving parts to secure the phone. Because of the layer lines and delamination associated with FFF printing, it wouldn't be as viable long term under daily use while mounting and unmounting the phone. Additionally, because I wanted the assembly to be as small as possible, I needed the parts to be strong without being bulky, which SLS excels at.
* **Off-the-shelf parts required:**
  * 1x M4 10mm socket screw (McMaster 91290A144)
  * 4x M4 12mm socket screws (McMaster 91290A144)
  * 1x M4 long heat set insert (McMaster 94180A353)
  * 4x M4 short heat set inserts (McMaster 94180A351)

{% include gallery %}

## CAD Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH286ddQT78850c0d8a42310f7aee96e8ebd?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
