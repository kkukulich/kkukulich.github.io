---
layout: post
title: Solid state phase transformation in titanium alloys
date: 2019-12-16 00:00:00 +0300

img: 3d-cal-2.png # Add image post (optional)
tags: [Productivity, Software] # add tag
---

### Skills learnt

* C++
* Large scale software development
* Modular programming
* Partial Differential Equations
* FFT

### Deliverables: 

* An interactive C++ suite that can be integrated into a multi-scale framework as well as used as a standalone phase field module has been developed. A preliminary version has been made public [here](https://github.com/ArunBaskaran/InteractivePFSuite), and doesnt include the elastic strain modules. 

### Detailed description

* A multi-phase field model is implemented to understand the morphological origins behind the
solid state phase transformations in Ti-6Al-4V(Ti64). Ti64 is a dual phase alloy at room
temperature, and the coexisting thermodynamic phases are α (HCP) and β (BCC). Orientational
relationship between α and β and crystal symmetry constraints result in twelve different
α-variants that can nucleate from the β matrix. 


 <img src = "{{site.url}}/assets/images/var1-habitplane.png" hspace="25" height="300" width="300" />
  <img src = "{{site.url}}/assets/images/var12-habitplane.png" hspace="25" height="300" width="300" />
  
  
The variety of morphological features observed in
the alloy, such as basket-weave and colony, result from the variant selection process
undergone by the alloy during its microstructural evolution. Since different morphologies result
in different mechanical properties, such as fracture toughness and fatigue, it is important to
understand the influence of processing conditions on the morphological origins of the alloy. The
phase field model is coupled to realistic thermodynamic databases in order to model the
evolution of solute fields, and the microelasticity theory in order to incorporate the
transformation and lattice mismatch strains occurring during the solid state phase
transformation. The driving force for nucleation is modeled as the sum of chemical driving force
and strain energy driving force.


Modeling of the spatial evolution of strain interaction energy and solute concentration fields
enables us to identify the alpha-variant with the highest probability of nucleation at any given
spatial point. The phase field equations govern the subsequent growth of nucleated variants,
incorporating the solute supersaturation at boundaries, interaction of the variant’s transformation
strain with the strain field in the microstructure, anisotropic interfacial energies, and temperature.
The modeling of co-evolution of phase fields, solute fields, and the strain field makes it possible
to rationalize the morphologies observed in experiments. We report the work in progress
towards modeling the influence of cooling rate on morphological evolution in the alloy.

 <img src = "{{site.url}}/assets/images/3d-cal-2.png" hspace="25" height="300" width="300"/>
  <img src = "{{site.url}}/assets/images/3d-cal-3.png" hspace="25" height="300" width="300" />
