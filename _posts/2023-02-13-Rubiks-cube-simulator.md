---
layout: post
title:  "Rubik's cube simulator in excel"
date:   2023-02-13 13:01:40
blurb: "Rubik's cube simulator in excel"
og_image: /assets/img/image.png
---

<img src="{{ "/assets/img/image.png" | absolute_url }}" alt="screenshot of rubiks cube simulator in excel" class="post-pic"/>


I used to be obsessed with Rubik's cubes back in high school. I was never world class :p but after probably solving many thousands of Rubik's cubes I did get close to solving any scramble in ~11 seconds on average.

At one point I actually took it as challenge to solve the worlds biggest rubik's cube (with dimensions of 121x121x121), which took me ~89h across several months. [You can read my blog post here about it from nearly a decade ago](https://www.speedsolving.com/threads/uwr-121x121x121-largest-solve-ever.44193). Such a large rubik's cube can't even really be practically built, so it's all done in a simulator. 

You can probably tell that I'm often compelled to do things just for the challenge of it -- simulating a rubik's cube in excel is also really inefficient but it was fun to do just for the challenge.

The buttons in the spreadsheet are linked to a macro written in VBA for Excel. In the subroutines, the calculations are done with arrays before outputting the values to the excel sheet.

There is both an unfolded visualization of the 6 faces of the rubiks cube as well as a 3d visualization that can be rotated to see the 'hidden' sides, since you can only see three faces of the cube at a time. It also has a timer and automatic scrambler.

The 3d visualization took some creativity -- there is no 3d modelling :p rather the cube is constructed by shapes whose individual color updates with each turn.

The excel file is uploaded at this [Dropbox link](https://www.dropbox.com/scl/fi/nnwb1gjeoduzayam84jur/Rubiks-Cube-Simulator.xlsm?dl=0&rlkey=lqtn6azjisgf35uobv07towu2).
