---
layout: post
title:  "Projects"

img: sea.png # Add image post (optional)
date:   2019-10-24 18:24:51 -0500

---

---


## Augmenting the feature vector for material design through analysis of grain growth

### Software tools used

* Surface Evolver
* Mathematica

### Python Libraries Used

* Matplotlib

### Techniques Used 

* Voronoi Tesselation

### Graphical Summary

<img src = "{{site.url}}/assets/img/nVSxratio.png" style="display: block; margin: auto;" />

### Description
Material design for nanocrystalline applications, focusing towards a particular stable grain size, is an emerging field.
Focus has largely been on alloy selection based on enthalpy of solute segreation to the grain boundaries([1](https://link.springer.com/article/10.1007/s11837-015-1636-9), [2](https://science.sciencemag.org/content/337/6097/951)). This work brings to light a new parameter, X<sub>ratio</sub>, that can potentially be used for improved alloy designing. 

X<sub>ratio</sub> is defined to be X<sub>bulk*</sub>/X<sub>total</sub>. X<sub>bulk*</sub> is the bulk mole fraction of the solute that corresponds to a theoretical zero value of the grain boundary energy. X<sub>total</sub> is the total mole fraction of the solute in the entire alloy. While the former depends on material parameters such as the enthalpy of solute segregation, T, and grain boundary energy of the pure solvent, the latter is a microstructural parameter that depends only on the average grain size of the material. Essentially, X<sub>ratio</sub> combines both material parameters and microstructural parameters into one compact parameter. As seen in the image in graphical summary above and in the figure below, X<sub>ratio</sub> not only influences the steady state grain size, but also influences the n-exponent of the grain growth.

We investigate the kinetic regimes of solute segregation inhibited grain growth under the condition of dynamic solute redistribution between the grain boundaries and the bulk.Langmuir-Mclean's analytical framework is adopted to model solute equilibrium between grain boundaries and the bulk, and the Gibbs adsorption isotherm is used to model the dependence of the grain boundary energy on the solute mole fraction. The inhibition of grain growth is incorporated in the model through a segregation-induced reduction in the grain boundary interfacial energy. Two-dimensional numerical simulations, performed by implementing this model within the framework of Surface Evolver, are used to validate predictions from the analytical framework and provide insights into the kinetic behavior of alloy systems under the given conditions. Under the stated assumptions, two different regimes of grain growth are identified depending on the steady state value of X-bulk. When X-bulk is asymptotic to X-bulk* , grain growth is completely impeded, whereas when it is asymptotic to X-tot, the total mole fraction of solute in the material, grain growth continues unimpeded.


<img src = "{{site.url}}/assets/images/Regime-Summary.png" style="display: block; margin: auto;" />

---

## Predicting later-time grain stability based on initial topographical data

### Python Libraries Used

* Scikit-Learn
* Pandas
* Numpy

### Techniques Used 

* Data Cleaning
* Feature Engineering
* Classifiers - Random Forest, Decision Trees, 1D-CNN

### Code repository

https://github.com/ArunBaskaran/DS-Projects/GrainStability

### Description

To be Updated




---



