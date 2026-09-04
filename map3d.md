---
layout: cv
title: 3D Map Engine
---

# 3D Map Engine

While working in Zenly, I was involved in many backend geometry-related tasks. Below, you can see some of this work. 
Note that the look and feel, and how the final result appears on the phone screen is not my work but of many other talented people in the team, 
who did an awesome job to optimize and support my geometries even on the old phones with very limited power. I did not work either on things like trees, 
fountains, grass, and a few others. My work involves only buildings, bridges, partially roads, terrain, and rivers. In addition, 
I contributed to creating road networks with multiple lanes and simulated traffic.

### Challenges

A significant challenge was ensuring the functionality across thousands of tiles constituting the complete world map. Dealing with boundaries 
posed a major issue, as many geometric objects were fragmented by tile borders. We needed to devise a method to create a seamless triangle mesh, 
avoiding visual glitches along the boundaries while still supporting global tiling. Another hurdle was managing the size of the final meshes generated. 
To optimize performance on phones with limited processing power, extensive optimizations were implemented on both the backend and rendering aspects.

All 3D objects were automatically generated from simple input data. For instance, bridges were crafted from a set of 3D polylines without any known bridge heights. 
Buildings were extruded from 3D flat footprint polygons. All urban objects then have been properly embedded in the ground represented as a triangle mesh. 
Roads, lanes, and traffic simulations were generated from sets of 3D polylines with designated road directions only.

### Work With

[Charly Delaroche](https://www.linkedin.com/in/charly-delaroche-949a2391/), [Matt Amos](https://www.linkedin.com/in/matt-amos-94175ba0/), 
[Hannes Janetzek](https://www.linkedin.com/in/hannes-janetzek-399340115/), et al.

### Resources

[`All visuals can be downloaded here.`](../assets/files/map3d-visuals-anisimov.zip)

<img src="../assets/files/map3d-preview.jpeg" alt="3D Map Engine" title="3D Map Engine" />
