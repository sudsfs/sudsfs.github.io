---
layout: post

#event information
shorttitle:  "Beyond end-to-end learning"
title:  "Beyond end-to-end learning: injecting knowledge in the architecture"
cover: "/assets/images/gp.gif"
date:   2018-10-26
start_time: "14:00"
end_time: "15:00"
location: "Roslagstullsbacken 21, Huvudbyggnaden, våningsplan 5, AlbaNova Rumsnr: B5:1046 Lokalkod: FB54"
location_link: https://www.kth.se/places/room/id/27a5a141-8803-4ec1-9795-d3afe3f40673



#event speaker
speaker_name: "David Menéndez Hurtado"
speaker_affil: "Department of Biochemistry and Biophysics, Stockholm University"
speaker_photo: "https://upload.wikimedia.org/wikipedia/en/5/52/Mark_I_perceptron.jpeg"


#event organiser details
organiser: "Jens Jasche"

---
Background:
=======
The goal of supervised learning is to find, from a set of examples, a function mapping between a set of inputs and a set of outputs, or labels. Most of the general machine learning research has been focused on finding better machinery to learn such mappings [1], such as SVMs, Random Forests, Markov Models, or Neural Networks; while application research has been focused on finding better representation of the inputs [2], or even different outputs [3].

Deep learning [4] research has exploded in the later years for several reasons:

Access to bigger data sets.
Availability of computational power to process them.
Flexibility in model building.
Leverage of structure in the data.

Only the last two points are relevant to this talk.

A “Deep” learning model is a stack of “layers”, most of which are relatively simple mathematical operations [5]. Deep learning provides a framework where these simple bricks can be freely combined to build arbitrarily complex models, which in turn empowers us to take full advantage of the structure of the data, and tailor our model to our specific domain. To give some classical example: in computer vision, pixels on an image group together to form edges and textures, that are combined to form shapes; a convolutional neural network is built to extract this very hierarchy from the raw pixels. And when processing the meaning of a sentence in natural language, every word is conditioned by everything that has happened before: a recurrent network can memorise past information and use it to understand the current word.


Content:
=====
In this talk I will present how to bring this one step up and use not only the structure of the data, but also the problem itself. I will illustrate with the problem of evaluating protein structure models in the absence of experimental data. [6] Here, we are presented with a collection of protein models of diverse quality, and a measurement of their similarity to the real structure. The relevant figures of merit are local correlations (how well can good and bad parts of a model be identified), global correlations (how well can models be ranked as a whole), and per target correlations (how well can we rank models from the same protein, or target).

As any other machine learning problem, one needs to find a suitable representation of the inputs, settle on a machine learning algorithm, and an appropriate measurement of quality, each of them has been subject of countless research papers.

In our work on ProQ4 [7], we show that there is another open front: for each protein we have a large number of models, a redundancy in our training set. But we can turn this around and focus our training on selecting the better model of every pair. From N examples, we obtain N(N-1)/2 pairs. I will show how to include this structure in the training, and how the final result is significantly improved.

I hope this procedure can inspire others to find underlying and underused structures in their problems, and encourage to turn redundancies from weaknesses to strengths.


Notes and references:
----------------------------

[1] [https://xkcd.com/1838/](https://xkcd.com/1838/)

[2] For example, in computer vision, SIFT features were the state of the art until the explosion of Deep Learning. [link](https://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_feature2d/py_sift_intro/py_sift_intro.html)

[3] Uziela K, Menéndez Hurtado D, Shu N, Wallner B, Elofsson A. Improved protein model quality assessments by changing the target function. Proteins. 2018;86:654–663. [link](https://doi.org/10.1002/prot.25492)

[4] A good and thorough introduction: www.deeplearningbook.org. For something shorter: LeCunn Y, Bengio Y, Hinton G, Deep learning. Nature. 2015. [link](https://doi.org/10.1038/nature14539)

[5] Ie, mostly linear operations, with a point-wise non-linear operation.

[6] Daisuke Kihara, Hao Chen and Yifeng David Yang, “Quality Assessment of Protein Structure Models”, Current Protein & Peptide Science (2009) 10: 216. [link](https://doi.org/10.2174/138920309788452173)

[7] Menéndez Hurtado D, Uziela K, Elofsson A, “Deep transfer learning in the assessment of the quality of protein models” (2018) [arXiv:1804.06281](https://arxiv.org/abs/1804.06281)
