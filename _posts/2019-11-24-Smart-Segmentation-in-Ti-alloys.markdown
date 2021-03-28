---
layout: post
title: Contextual Segmentation of Microstructural Features using Deep Learning
date: 2019-12-30 13:32:20 +0300
# Add post description (optional)
img: 1990seg.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: 
---

### Python Libraries Used

* Keras
* Scikit-Learn
* OpenCV
* MatplotLib

### Techniques

* Neural network design.
* Parameter and Hyperparameter search.
* Regularization.



### Graphical Summary: 

* Design of the pipeline:

<img src = "{{site.url}}/assets/images/pipeline2.png" hspace="80" height="450" width="550" />

* Best accuracy achieved during classification: 94.07%

* Image processing to extract morphological data:

<img src = "{{site.url}}/assets/images/1990seg.png" hspace="50" align="middle" height="300" width="300" />
<img src = "{{site.url}}/assets/images/433seg.png" align="middle" height="280" width="280" />

### Dataset:

* **Source:** Micrographs generated from Scanning Electron Micrography.

* **Augmentation:** Sectioning/Cropping to increase the size of the dataset.

* **Data cleaning:** Pre-processing steps undertaken include a Gaussian blur for the classification step, and a Contrast Limited Adaptive Histogram Equalization (CLAHE) filter for the segmentation step.

### Publication: 

The work has undergone peer-reviewed publication in Computational Material Science, and can be found [here](https://www.sciencedirect.com/science/article/pii/S0927025620300847). 



### Description: 

The microstructures of Titanium alloys exhibit a wide variety of morphological features (such asglobules, needles, lamellae, etc.), each of which influences the physical properties of the alloy in its own way. Thus, to fulfill a comprehensive process-structure-property mapping, it is essential to quantify these features for any given sample. However, generating a quantitative finger-print for a sample through manual selection of conventional image processing methods would be an inefficient process. Towards this goal, we have demonstrated an efficient paradigm for quantitative characterization of a microstructure dataset by leveraging the power of machine learning tools and image segmentation algorithms. A two stage pipeline consisting of a classification step and a segmentation step is used to process titanium microstructures  and output quantitative measurements relevant to the particular class of microstructure identified. 

For the classification step, a Convolutional Neural Network is trained using the TensorFlow framework, with the architecture consisting of three convolutional layers and one fully connected layer. The microstructures are classified into three labels: “lamellar”, “duplex”, and “acicular”. For the training step, a material microstructure dataset of 1225 images is established, comprised of Ti-6Al-4V alloy micrographs acquired from seven different thermal processing conditions. It reported an accuracy of 93.00 ± 1.16 %, averaged over 5 trials incorporating a random division of the total dataset into training and test sets.  

For the second stage of the pipeline, image processing techniques were selected specific to the classification label of
the micrograph. The area fraction of equiaxed grains is extracted from bi-modal microstructures using a marker-based watershed technique, and the area fraction of the dominant α-variant is extracted from basket-weave structures using a Histogram of Oriented Gradients (HOG) method. Computational tools similar to the proof of concept pipeline demonstrated in this work can be used by engineers to better identify microstructural features that arise due to process or material variations.

The major challenge was having to work with a relatively small material image dataset, which is typical for the domain. The architecture of the CNN was arrived at with a trial-and-error method, and the hyperparameters were optimized with the Keras tuner. This work highlights the potential in application of the advances in artificial intelligence in a traditional physical sciences field such as Material Science, and at the same time brings to the forefront the challenges brought by material datasets towards such applications. 







