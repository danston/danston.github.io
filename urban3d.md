---
layout: cv
title: 3D Urban Reconstruction
---

# 3D Urban Reconstruction

While being at Inria, working as a research and developer engineer, I undertook the ambitious project of developing a fully automated pipeline. This pipeline aimed to take a raw point cloud, containing only x, y, z coordinates, and reconstruct the urban environment with varying levels of detail (LODs). The primary objects addressed in this pipeline were ground, buildings, and trees, with potential plans to incorporate additional objects later on. The levels of detail included LOD0, representing only flat footprints of objects (polygons for buildings and circles for trees) with a flat ground polygon; LOD1, featuring shoe boxes for buildings and cylinders for tree trunks with a ground triangle mesh; and LOD2, incorporating buildings with detected roofs and walls, trees with trunks and crowns detected, and a ground triangle mesh. Notably, in LOD1 and LOD2, buildings and trees were accurately embedded into the ground, respecting the local surface characteristics.

### Challenges

This task presented a multitude of challenges, including the difficulty of distinguishing between points representing trees and buildings when they are in close proximity. Even when correctly identified, removing points of one class can create substantial gaps in objects of the other class, making it challenging to determine the accurate shape of the object and reconstruct it afterwards. Managing the size of the point cloud was another hurdle, requiring segmentation into parts and subsequent merging, which is not always straightforward. As the levels of detail increase, especially from LOD1, complications arise in fitting precise roof shapes to building boundaries from a point cloud. The slopes and other roof parameters become quite unstable. 
Finally, the error accumulation does not make the life easier. Making a small error at LOD0 can lead to a disaster at LOD2 due to the cumulative effect.

### Work With

[Pierre Alliez](https://team.inria.fr/titane/pierre-alliez/), [Simon Giraudot aka Gee](https://ptilouk.net/), 
[Florent Lafarge](https://www-sop.inria.fr/members/Florent.Lafarge/), and [Andreas Fabri](https://geometryfactory.com/who-we-are/).

### Resources

[`All visuals can be downloaded here.`](../assets/files/urban3d-visuals-anisimov.zip)

<img src="../assets/files/urban3d-preview.jpg" alt="3D Urban Reconstruction with LODs" title="3D Urban Reconstruction with LODs" />
