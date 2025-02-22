---
layout: page
title: Building shape
subtitle: 
---

## Building shape scenarios
We will present a few different outputs from the growth algorithm, to illustrate how different weights affect the building shape. Sliders in Houdini are used to change the weights on each of the previously explained four parameters that affect growth: clustering, stacking, flattening, and gravity.

This first output is created from an unweighted scenario -- essentially, there is no bias towards any of the four parameters. This scenario is not structurally feasible, nor does it allow for car parking (in the large middle purple-ish function) or easy circulation throughout the building. At the bottom of this page there is a color code for what color represents each function.

![building shape 1](/assets/img/buildingshape1.jpg){: .mx-auto.d-block :}

The building shape below has a higher gravity weight and  makes more sense for our goals. However, there are some strange sections still.

![building shape 2](/assets/img/buildingshape2.jpg){: .mx-auto.d-block :}

## Final building shape

Finally, by increasing the gravity weight even more and setting stacking to be slightly lower than the flattening weight, we achieved a suitable building shape.

![final building shape front](/assets/img/finalbuildingshape1.png){: .mx-auto.d-block :}![final building shape back](/assets/img/finalbuildingshape2.png){: .mx-auto.d-block :}

The color code for the functions:
![function color code](/assets/img/function_key.png){: .mx-auto.d-block :}
("small" means that there were two functions with very similar colors, so it is the smaller of the two.)