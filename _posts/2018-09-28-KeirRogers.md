---
layout: post

#event information
shorttitle:  "Bayesian optimisation and Gaussian process emulators"
title:  "Optimised interpolation of costly simulations: Bayesian optimisation and Gaussian process emulators"
cover: "/assets/images/gp.gif"
date:   2018-09-28
start_time: "14:00"
end_time: "15:00"
location: "The Cramér Room  (306, level 3)/ Department of Mathematics / Stockholm University / Kräftriket, house no. 6"
location_link: 

#event speaker
speaker_name: "Keir Rogers"
speaker_affil: "Department of Physics, Stockholm University"
speaker_photo: "https://upload.wikimedia.org/wikipedia/commons/e/ec/Carl_Friedrich_Gauss_1840_by_Jensen.jpg"


#event organiser details
organiser: "Jens Jasche"

---
The generic problem in data science is to compare data to theory. However, for example in sampling the posterior probability distribution of the parameters of a theory, this often requires millions of simulations of mock data from a chosen theory. This is often impossible because such simulation is too computationally expensive. I will discuss the technique of Gaussian process emulation, where a small training set of simulations is used to predict (the conditional distribution of) simulation outputs throughout parameter space. This is essentially interpolation, but expressed as a Bayesian inference, where the Gaussian process modelling allows the consideration of a wide function space. The construction of the training set is key. I will discuss the technique of Bayesian optimisation, where the training set is actively built up, conditional on the information already learnt and the uncertainty present from previous iterations of the training data. Together, these allow an arbitrary number of evaluations of a theory and solve the problem of how to compare data to costly simulations.
