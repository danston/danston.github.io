---
layout: cv
title: WarpIt App
---

# WarpIt App

As a side project during my PhD, I developed a small program for warping 2D images. The approach involves creating a control polygon, referred to as a shell, around the given image. By manipulating the vertices of this polygon, referred to as pulling, you can alter the image. Additionally, providing a new target polygon with the same number of vertices enables the image to deform accordingly.

### Challenges

The primary challenge lies in avoiding excessive fold-overs with the control polygon, a common issue in such scenarios. To mitigate this, I employed new subdividing barycentric coordinates, chosen for their properties that ensure smooth warping effects. The process involves triangulating and subdividing the polygon beneath the image, computing these coordinates, and then utilizing them to warp the image.

### Work With

[Teseo Schneider](https://web.uvic.ca/~teseo/)

### Resources

[`See App here.`](https://github.com/danston/warpit)

[`All visuals can be downloaded here.`](../assets/files/warpit-visuals-anisimov.zip)

<img src="../assets/files/warpitapp-preview.png" alt="WarpIt App" title="WarpIt App" />
