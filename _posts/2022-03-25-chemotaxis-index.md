---
layout: post
title: Rapid assesment of the chemotaxis index (CI)
subtitle: See how I used Python to speed up phenotyping
gh-repo: AndersenLab/chemotaxis-cli
gh-badge: [star, fork, follow]
tags: [Phenotyping, python]
comments: true
---

### Background
Wild nematodes can sense and react to all sorts of chemical cues in their natural environment. When a nematode moves towards a particular cue, it’s displaying a behavior known as chemotaxis. One of the most common ways to study chemotaxis in the lab is to use a Chemotaxis Assay. In these assays, researchers transfer many nematodes to the center (origin) of a circular agar plate then observe how the nematodes respond to a chemical located on periphery of the plate. The test compound is spotted on the plate a set distance away from the origin in two of four quadrants on the plate, the other quadrants are spotted with a control solution (diluent only). After the animals react to the cues, researchers calculate the chemotaxis index (CI), which describes the behavioral response as a range from 1 (maximum attraction) to -1 (maximum avoidance). 

**The problem** is that traditional chemotaxis assays have low throughput because researchers must manually setup experimental populations and score CIs.

**To fix this issue**, my collaborators and I came up with an automated methodology that uses liquid-handling robots to transfer nematodes to plates and a custom image analysis package, `ct`, to automate the scoring of CIs from plate images. You can see our workflow in the figure below.  

![](/assets/img/chemotaxis_workflow.png)

To see more detail checkout our recent [manuscript](https://www.biorxiv.org/content/10.1101/2022.04.30.490142v1) and the [GitHub repo](https://github.com/AndersenLab/chemotaxis-cli).
