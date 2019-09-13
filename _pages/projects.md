---
title: "Undergraduate Projects -"
excerpt: "Undergrad/Course Projects"
author_profile: true
permalink: /projects/
redirect_from:
  - /tags/
---

The relevant projects from my undergraduate days. 

# Laboratory/Design Projects:

# Multimedia Research Laboratory @ BITS Pilani
<small>Mentors : [Prof. Kamlesh Tiwari], [Prof. Surekha Bhanot]</small>

<small>Topic : Image to text translation with deep neural networks for the speech impaired</small>

<small>Duration: August - December 2017</small>

* The linear layers and the classifier of an [AlexNet] model, trained on the [ImageNet] dataset, were finetuned on the [ASL Fingerspelling dataset A]; data augmentation techniques were used on the ASL dataset to prevent overfitting by Alexnet 
* Suitable training hyperparameters were experimentally found through grid search
* I learnt about language modeling with deep neural networks and experimented with common bag of words (CBOW) model for the [Tiny Shakespeare] dataset
* A character RNN was trained on the Tiny Shakespeare dataset to complete sentences given a primer text of characters
* Finally, the outputs/character labels of the fine-tuned CNN are used to provide the primer text for the RNN to generate the rest of the text
* This work can have practical application in the form of voice generation system for the speech impaired
* Most of the code was written in Pytorch and Tensorflow

[Project Report](https://sagnikmjr.github.io/files/LOP17_report.pdf)

# Multimedia Research Laboratory @ BITS Pilani
<small>Mentor : [Prof. Surekha Bhanot]</small>

<small>Topic : Face recognition using convolutional neural networks</small>

<small>Duration: January - May 2017</small>

* I studied the working of CNNs and their use for different computer vision tasks
* [(VGG-D , VGG-E)](https://arxiv.org/abs/1409.1556) were trained end to end on [Color Feret](https://www.nist.gov/itl/iad/image-group/color-feret-database) and [Youtube Faces](https://www.cs.tau.ac.il/~wolf/ytfaces/) datasets
* The linear layers and the classifier of VGG-E models trained on Youtube Faces, were finetuned on the [LFW](http://vis-www.cs.umass.edu/lfw/) dataset; the [OpenFace](https://github.com/cmusatyalab/openface.git) toolbox was used for scaling and aligning the images from LFW dataset because the images from LFW are far more diverse in style due to variety in poses, lighting etc.
* I experimentally found suitable training hyperparameters through grid search
* Caffe and python were used for coding most part of the project

[Project Report](https://sagnikmjr.github.io/files/DOP17_report.pdf)|[Codebase](https://github.com/SAGNIKMJR/Speed-Limit-Recognition-using-VGG19-on-GTSRB-in-Caffe)



# Collaboration Projects:

# Nano-Bio Sensors Group @ CSIR-CEERI Pilani
<small>Mentor : [Mr. Soumendu Sinha](https://www.ceeri.res.in/profiles/soumendu-sinha/)</small>

<small>Topic : Temperature compensation with machine learning models in ISFET based pH-meter</small>

<small>Duration: January - May 2017</small>

* An ISFET based pH-meter was designed at the fabrication unit of the institute
* pH data at different temperatures (pH sensitivity with temperature) was collected
* Features from the collected data were centered around the feature means and scaled down by the inverse of the feature standard deviations
* Several regression models (3-layered feedforward fully-connected neural network, Random Forrests, Support Vector Regression, Polynomial Regression) were trained on the collected data for temperature compensation
* Majority of the code was written using scikit learn and numpy in python. 
* Two papers from this work have been published at [IEEE RSM 2017](https://ieeexplore.ieee.org/document/8069141/) and [IJCTA 2019](https://onlinelibrary.wiley.com/journal/1097007x)


[Publication 1](https://sagnikmjr.github.io/files/Temperature_Compensation_of_ISFET_Based_pH_Sensor_Using_Artificial_Neural_Networks.pdf)|[Publciation 2](https://onlinelibrary.wiley.com/doi/pdf/10.1002/cta.2618)


# Minor Projects:

# Multimedia Research Laboratory @ BITS Pilani
<small>Mentor : [Prof. Kamlesh Tiwari]</small>

<small>Topic : Scale specific CNNs for scene recognition</small>

<small>Duration: March - April 2017</small>

* An ensemble of scale-specific CNNs to recognize scenes of variable scales was designed
* I reproduced baseline results from the [publication](https://arxiv.org/abs/1801.06867) on [SUN397](https://groups.csail.mit.edu/vision/SUN/) dataset


[Project Report](https://sagnikmjr.github.io/files/MLReportFinal.pdf)


# Multimedia Research Laboratory @ BITS Pilani
<small>Topic : Online traffic sign recognition system with Canny edge detection and CNNs</small>

<small>Duration: March - April 2017</small>

* Traffic signs from traffic scene images in [GTSRB](http://benchmark.ini.rub.de/?section=gtsrb&subsection=news) dataset were detected using Canny edge detection
* A VGG-19 ImageNet model was fine-tuned on the data for traffic sign classification
* I built a GUI using PyQT4 for online inference of traffic scene images using the model
* The project was presented at APOGEE 2017, BITS Pilani annual technical festival


# Wireless Sensor Networks Systems Laboratory @ CSIR-CEERI Pilani
<small>Mentor : [Dr. Kota Solomon Raju](https://sites.google.com/site/drsolomonrcswsn/)</small>

<small>Topic : Signal denoising of household power lines using wavelet transform in python</small>

<small>Duration: August - December 2016</small>

* An in-depth literature survey of signal denoising in house-hold power lines was done
* Finally, wavelet transform was chosen as the method to denoise in combined time-frequency domain
* Code was written in python for performing denoising on real-time simulations of household power signals


[Prof. Surekha Bhanot]:<http://universe.bits-pilani.ac.in/Pilani/surekha/profile>
[Prof. Kamlesh Tiwari]:<http://www.bits-pilani.ac.in/pilani/kamleshtiwari/Profile>
[ASL Fingerspelling dataset A]:<http://empslocal.ex.ac.uk/people/staff/np331/index.php?section=FingerSpellingDataset>
[ImageNet]:<http://www.image-net.org/>
[AlexNet]:<https://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf>
[Tiny Shakespeare]:<https://github.com/karpathy/char-rnn/tree/master/data/tinyshakespeare>





