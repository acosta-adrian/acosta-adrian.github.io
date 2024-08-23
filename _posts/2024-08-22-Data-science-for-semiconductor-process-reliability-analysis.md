---
layout: post
title:  "Data science for semiconductor process reliability"
date:   2024-08-22 07:13:54
blurb: "Data science for semiconductor process reliability"
og_image: /assets/img/image.png
---

Link to Kaggle notebook for this project: [https://www.kaggle.com/code/adrianacosta0/data-science-for-semiconductor-process-reliability](https://www.kaggle.com/code/adrianacosta0/data-science-for-semiconductor-process-reliability)

I set up this mini-tutorial to demonstrate:

1) Sets up a CVD reactor model for the growth of SiO2 in a process chamber.

The growth is affected by several key input parameters which have a corresponding sensor that monitors these inputs.

As part of the exercise, we introduce variation in the process conditions to simulate chamber-to-chamber mismatch

2) This sets us up to analyze sensor data from semiconductor deposition chambers to get to root causes of variations in wafer dep growth rates

Utilizing techniques like Principal Component Analysis (PCA) helps us visualize and understand the underlying patterns in the data, while regression models enabled us to pinpoint the most influential factors impacting film thickness.

3) Building on these insights, we introduced controlled systematic drifts to mimic real-world equipment issues, such as gradual clogging, and assessed their effects on the deposition process using regression.
