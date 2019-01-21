---
layout: post

#event information
shorttitle:  "Likelihood-free inference beyond ABC"
title:  "Likelihood-free inference beyond ABC"
cover: "/assets/images/gp.gif"
date:   2019-01-25
start_time: "14:00"
end_time: "15:00"
location: "Room 22 / Department of Mathematics / Stockholm University / Kräftriket, House 5"
location_link: https://www.su.se/polopoly_fs/1.294747.1504850221!/menu/standard/file/SU%20kartor%20Original%20Kräftriket%2020170817.pdf
talk_link: 

#event speaker
speaker_name: "Justin Alsing"
speaker_affil: "Department of Physics"
speaker_photo: "https://upload.wikimedia.org/wikipedia/commons/d/d4/Thomas_Bayes.gif"


#event organiser details
organiser: "Jens Jasche"

---
Likelihood-free inference (LFI) provides a framework for performing Bayesian inference using only forward simulations. This has great appeal since it allows for inference under arbitrarily complex generative models — as long as you can simulate realizations from your model, you can do inference under it with LFI. Traditional approaches to LFI have been based on Approximate Bayesian Computation (ABC), which involves proposing model parameters, simulating mock data, and accepting/rejecting based on whether the simulated data fell “close” to the observed data. ABC typically requires a vast number of simulations, making it unfeasible when simulation is even modestly expensive, and the “closeness” criterion inevitably puffs up the inferred (approximate) posterior. I will talk about recent developments in likelihood-free inference beyond ABC that allow for high-fidelity posterior inference from many orders of magnitude fewer forward simulations than ABC. I’ll show cutting edge likelihood-free inference applications in epidemiology and cosmology (where simulation is expensive), and demo our public python package for state-of-the-art LFI.
