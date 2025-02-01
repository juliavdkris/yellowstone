---
layout: page
title: Choice of facade tiles
subtitle: 
---

## Facade types
The facade tiles will be made of oak slats, glass, and concrete.

For the windows, there are four tile types: full window, half window / half wood slats, window with slanted wood slats, and full wood slats (the only option with no window).

The balconies consist of two presets, both made with smooth curves.

Below are the four window facades and the two balcony presets, in both normal and wireframe view on Houdini.
![facade wireframe](/assets/img/facade_wire.png){: .mx-auto.d-block :}
![facade](/assets/img/facade.png){: .mx-auto.d-block :}

Lastly, to create an organically shaped building, we created three types of curved corner tiles that would be placed at every corner. The three types are shown below.
![corners](/assets/img/corners.png){: .mx-auto.d-block :}

## Facade placement
The placement procedure depends between windows and balconies, as well as between residential and public functions.



The placement of windows for residential units is determined by each voxel's exposure to sunlight. The facade placement algorithm loops through each voxel in the building, looking at the amount of sunlight a voxel gets, and placing the appropriate facade type. For voxels exposed to high sunlight, for example, they will have a half-window facade or a window with slanted slats over it. For a voxel with low sunlight, it will receive a full window.