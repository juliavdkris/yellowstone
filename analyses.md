---
layout: page
title: Analyses
subtitle: Sun, sky view, hotspot, and noise
---
Five analyses were performed on the voxel cloud that was created previously, with scores being assigned to the voxels for each analysis. First, we performed analyses regarding sun: 1) voxels shaded surrounding buildings, and 2) voxels that were shaded by surrounded buildings. Then, a sky view analysis was performed, which determines the view quality for each voxel. The hotspot analysis looked at the visibility of five prominent architectural hotspots in Rotterdam, and the noise analysis found which parts of the building were most impacted by the sounds of the surrounding environment.

Below is a flowchart showing the general process for the sun, sky view, and hotspot analyses (not noise):

![sun skyview hotspot flowchart](/assets/img/sun_view_hotspot_flow.png){: .mx-auto.d-block :}

## Sun analysis (shading others and being shaded)
The sun analysis was performed using 2019 sun path data obtained from sunearthtools.com. City data was from 3D BAG. Then, raycasting was used and the intersection of voxels with the rays determnied how much sun they were blocking and how much sun was being blocked from reaching them. The image below showsthe output of the sun analysis.

![sun](/assets/img/sun.png){: .mx-auto.d-block :}
![shadow](/assets/img/shadow.png){: .mx-auto.d-block :}

## Sky view analysis
A similar method was used for the sky view analysis as for the sun analysis, except this analysis checks if the voxels intercept the "skydome" that was created in a 200m sphere around the building.

![sky view](/assets/img/skydome.png){: .mx-auto.d-block :}

## Hotspot analysis
The hotspot analysis checks the visibility of the following five hotspots: Rotterdam Centraal Station, Stadhuis Rotterdam, Euromast, Erasmus Brug, and Kralingse Plas. In the end, however, this analysis was not incorporated into the facade placement because it limited in its execution: it does not take into account that the building blocks itself from certain views. 
The below image displays the visibility of the Erasmus Brug hotspot. There are four others for the four other hotspots.

![erasmus brug](/assets/img/erasmus.png){: .mx-auto.d-block :}

## Noise analysis
We performed the noise analysis using a soundmap from atlasleefomgeving.nl (Atlas of The Living Environment). The analysis calculates how noise travels through the space by assigning values to points based on their distance from noise sources. Then these values are weighed and normalized to create the final acoustic analysis.

![noise flowchart](/assets/img/sun_view_hotspot_flow.png){: .mx-auto.d-block :}
![noise](/assets/img/noise.png){: .mx-auto.d-block :}