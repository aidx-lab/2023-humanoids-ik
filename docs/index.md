---
layout: page
title:
---

This site complements the paper [**Efficient Learning of Fast Inverse Kinematics with Collision Avoidance**](https://ieeexplore.ieee.org/document/10375143) by
[Johannes Tenhumberg](https://scholar.google.com/citations?user=2RZuYZMAAAAJ), [Arman Milke](https://scholar.google.com), and [Berthold Bäuml](https://scholar.google.com/citations?user=fjvpDsEAAAAJ)
presented at the _2023 IEEE-RAS International Conference on Humanoid Robots_, in Austin, USA.


![Agile Justin in front of a shelf](/assets/imgs/justin_shelf2.jpg){:.this
style="width: 600px;
display: block;
margin-left: auto;
margin-right: auto"}


# Abstract
---
Fast inverse kinematics (IK) is a central component in robotic motion planning. For complex robots, IK methods are often based on root search and nonlinear optimization algorithms. 
These algorithms can be massively sped up using a neural network to predict a good initial guess, which can then be refined in a few numerical iterations. Besides previous work on learning-based IK, we present a learning approach for the fundamentally more complex problem of IK with collision avoidance. 
We do this in diverse and previously unseen environments. 
From a detailed analysis of the IK learning problem, we derive a network and unsupervised learning architecture that removes the need for a sample data generation step. 
Using the trained network's prediction as an initial guess for a two-stage Jacobian-based solver allows for fast and accurate computation of the collision-free IK. For the humanoid robot, Agile Justin (19 DoF), the collision-free IK is solved in less than 10 ms (on a single CPU core) and with an accuracy of 10^(−4)m and 10^(−3)rad based on a high-resolution world model generated from the robot's integrated 3D sensor. 
Our method massively outperforms a random multi-start baseline in a benchmark with the 19 DoF humanoid and challenging 3D environments. 
It requires ten times less training time than a supervised training method while achieving comparable results.


# Video
---
<p align="center">
<iframe width="560" height="315" 
src="https://www.youtube.com/embed/k96r7l2s384?si=rIMfyJil78aziiW7"
frameborder="0"
allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
referrerpolicy="strict-origin-when-cross-origin" 
allowfullscreen>
</iframe>
</p>


---

Cite this paper as:


    @inproceedings{Tenhumberg2023,
        author = {Johannes Tenhumberg and Arman Mielke and Berthold B{\"a}uml},
        title = {Efficient Learning of Fast Inverse Kinematics with Collision Avoidance},
        booktitle = {IEEE-RAS International Conference on Humanoid Robots (Humanoids)},
        year = 2023}

[arxiv](https://arxiv.org/pdf/2311.05938)