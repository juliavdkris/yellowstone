---
layout: page
title: Building shape
subtitle: 
---

We will present a few different outputs from the growth algorithm, to illustrate how different weights affect the building shape. Sliders in Houdini are used to change the weights on each of the previously explained four parameters that affect growth: clustering, stacking, flattening, and gravity.

This first output is created from an unweighted scenario -- essentially, there is no bias towards any of the four parameters. This scenario is not structurally feasible, nor does it allow for car parking (in the large middle purple-ish function) or easy circulation throughout the building.
![building shape 1](/assets/img/buildingshape1.png){: .mx-auto.d-block :}

The building shape below has a hiher gravity weight and  makes more sense for our goals. However, there are some strange sections still.
![building shape 2](/assets/img/buildingshape2.png){: .mx-auto.d-block :}

Finally, by increasing the gravity weight even more and setting stacking to be slightly lower than the flattening weight, we achieved a suitable building shape.
![final building shape front](/assets/img/finalbuilding1.png){: .mx-auto.d-block :}![final building shape back](/assets/img/finalbuilding2.png){: .mx-auto.d-block :}

