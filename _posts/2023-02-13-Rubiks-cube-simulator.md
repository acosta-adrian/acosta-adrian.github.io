---
layout: post
title:  "Rubik's cube simulator in excel"
date:   2023-02-13 13:01:40
blurb: "Rubik's cube simulator in excel"
og_image: /assets/img/image.png
---

<img src="{{ "/assets/img/image.png" | absolute_url }}" alt="screenshot of rubiks cube simulator in excel" class="post-pic"/>


Back in high school, I was obsessed with solving Rubik's cube. I probably solved many thousands to the point that I could solve any scramble in ~11 seconds on average.

At one point I actually took it as challenge to solve the worlds biggest rubik's cube (with dimensions of 121x121x121), which took me ~89h across several months. [You can read my blog post here about it from nearly a decade ago](https://www.speedsolving.com/threads/uwr-121x121x121-largest-solve-ever.44193). Such a large rubik's cube can't even really be practically built, so it's all done in a simulator. 

Naturally I'm often compelled to do things just for the challenge of it -- simulating a rubik's cube in excel is really inefficient and unecessary but it was fun to do it just for the challenge. 

The buttons in the spreadsheet are linked to a macro written in VBA for Excel. In the subroutines, the calculations are done with arrays that update the colors in the spreadsheet for the visualization of the faces.

There is both an unfolded visualization of the 6 faces of the rubiks cube as well as a 3d visualization that can be rotated to see the 'hidden' sides, since you can only see three faces of the cube at a time. It also has a timer and automatic scrambler.

For the 3d visualization...there is no 3d modelling :p rather I took a creative approach to just place shapes constructed by shapes that don't move but whose individual color updates with each turn.

The excel file is uploaded at this [Dropbox link](https://www.dropbox.com/scl/fi/nnwb1gjeoduzayam84jur/Rubiks-Cube-Simulator.xlsm?dl=0&rlkey=lqtn6azjisgf35uobv07towu2).
