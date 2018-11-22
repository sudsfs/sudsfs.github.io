---
layout: post

#event information
shorttitle:  "Solving non-linear ill-posed problems with the Levenberg-Marquardt algorithm."
title:  "Solving non-linear ill-posed problems with the Levenberg-Marquardt algorithm."
cover: "/assets/images/gp.gif"
date:   2018-11-30
start_time: "14:00"
end_time: "15:00"
location: "The Cramér Room  (306, level 3)/ Department of Mathematics / Stockholm University / Kräftriket, house no. 6 (easier from 6B)"
location_link: https://www.su.se/polopoly_fs/1.294747.1504850221!/menu/standard/file/SU%20kartor%20Original%20Kräftriket%2020170817.pdf
talk_link: 


#event speaker
speaker_name: "Jaime de la Cruz Rodriguez"
speaker_affil: "Astronomy Department"
speaker_photo: https://www.astro.su.se/polopoly_fs/1.345859!/image/image.jpg_gen/derivatives/article_505/image.jpg 


#event organiser details
organiser: "Emir Karamehmetoglu"

---
The Levenberg-Marquardt algorithm (LM) is an iterative method that allows to fit data with a non-linear model.
LM is particularly well suited for solving  problems where the calculation of derivatives of the model prediction is computationally challenging.
When the model parameters are well constrained by the model that we are employing, the algorithm is usually very robust. 
However, there are applications where the model parameters are not well constrained by the data in that case the solution can be degenerate.
I have implemented l-2 regularization into the Levenberg-Marquardt algorithm in order to solve problems with large number of parameters and to reduce the degeneracy of the solution, based on prior information.

In this talk I will discuss the derivation of this algorithm and the effect of different regularization functions in the solution.
