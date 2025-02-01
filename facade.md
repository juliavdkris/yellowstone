---
layout: page
title: Facade
subtitle: 
---

## Facade types
The facade tiles will be made of oak slats, glass, and concrete.

For the windows, there are four tile types: full window, half window / half wood slats, window with slanted wood slats, and full wood slats (the only option with no window). Designing the window tiles this way allows for the parametric placement of the facade to be made visual.

The balconies were designed to be made from four separate pieces that fit together in different combinations. However, due to the time constraint on this project, the final balcony options consist of two presets, both made with smooth curves.

Below are the four window facades and the two balcony presets, in both normal and wireframe view on Houdini.

![facade wireframe](/assets/img/facade_wire.png){: .mx-auto.d-block :}
![facade](/assets/img/facade.png){: .mx-auto.d-block :}

Lastly, to create an organically shaped building, we created three types of curved corner tiles that would be placed at every corner. The three types are shown below. These curved corners were another element of Yellowstone that was not captured in the final building design, due to the combination of curved corners and multi-voxel balconies creating a very complex facade placement.

![corners](/assets/img/corners.png){: .mx-auto.d-block :}

## Facade placement
The placement procedure depends between windows and balconies, as well as between residential and public functions.

The probability of a window being placed (as opposed to the fourth, closed off tile) is configured per unit type. So, parking does not have any windows, whereas some other public functions have a 50% probability of a window being placed. 

In addition to this window probability per unit type, the placement of windows is determined by each voxel's exposure to sunlight. The facade placement algorithm loops through each voxel in the building, looking at 1) if that voxel will get a window. 2) If the voxel will get a window, the algorithm will also look at the amount of sunlight a voxel gets, and from that, placing the appropriate facade type. For voxels exposed to high sunlight, for example, they will have a half-window facade or a window with slanted slats over it. For a voxel with low sunlight, it will receive a full window.

Balconies were only placed on residential units. The placement algorithm we used works based on a set probability of a balcony being placed -- it does not rely on exposure to sunlight. The balcony placement algorithm holds a higher level of complexity since the balcony presets are three voxels wide (9 meters) rather than one voxel wide (3 meters). The algorithm thus accounts for the balcony size and makes sure that the balconies do not overlap with each other or extend over the edge of the building.