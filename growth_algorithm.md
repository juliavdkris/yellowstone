---
layout: page
title: Growth algorithm
subtitle: 
---
The placed function seeds look like this:
![function seeds](/assets/img/seeds.png){: .mx-auto.d-block :}

Now that we have the function seeds placed, we can grow our building shape. We chose four parameters for the growth algorithm, each of which has a different effect on the growth itself. They are as follows:

1) Clustering: this parameter makes functions want to be close to each other, or to "cluster". We wanted our functions to grow in a clustered manner, rather than spread out too far, as it makes for unit shapes that are easier to work with down the line. Clustering essentially creates self-organizing housing units.

![clustering](/assets/img/clustering.png){: .mx-auto.d-block :}

2) Gravity: gravity makes functions want to grow down, and is useful to prevent a building structure that is not structurally sound or feasible. Our design principles outlined that we wanted a building with a roof park and two small "towers" on either side with residential functions. So, this parameter was necessary to make that happen.

![gravity](/assets/img/gravity.png){: .mx-auto.d-block :}

3) Flattening: Especially for the roof park, and for easy installment of solar panels, having functions grow in a flat way helps us reach our design goals. This parameter also can be thought of as the horizontal growth parameter -- on the other hand, gravity and stacking both control the vertical growth.

![flattening](/assets/img/flattening.png){: .mx-auto.d-block :}

4) Stacking: this parameter makes functions want to grow upwards, on top of each other. It encouraged a building strucutre that has clear separation between levels, and helps to maximize height while maintaining relative order.

![stacking](/assets/img/stacking.png){: .mx-auto.d-block :}