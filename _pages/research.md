---
title: "Research Experience -"
excerpt: "Research papers/reports/codebase"
author_profile: true
permalink: /research/
redirect_from:
  - /tags/
---
Research experience from research assistantship, bachelor thesis and internships

# Research Assistantship @ Goethe University Frankfurt 
<small>Mentors : [Prof. Visvanathan Ramesh], [Mr. Martin Mundt]</small> 

<small>Topics : Continuous learning, statistical outlier detection, Bayesian inference, Generative models  </small>

<small>Duration: July 2018 - May 2019</small>

<!-- [//]: # (Primarily, I have been jointly working on curating the novel COncrete DEfect BRidge IMage dataset (CODEBRIM) for multi-target classification of five commonly appearing concrete defects. We have compared two meta-learning approaches to find suitable convolutional neural network architectures for this challenging multi-class multi-target task. We have observed that learned architectures have less overall parameters in addition to yielding better multi-target accuracy in comparison to popular CNN architectures from the literature evaluated in the context of our application. We have jointly submitted a paper from this project to a tier-1 vision conference of the likes of ECCV, CVPR, ICCV etc.) 

[//]: # ([Submitted manuscript](https://drive.google.com/open?id=1Q3kgJ0BIyIb_dl-aUi-mmVzQ8xl_srfy)) -->

During the first half of the year-long RAship, I jointly worked with my mentors on curating the novel COncrete DEfect BRidge IMage (CODEBRIM) dataset for multi-target classification of five commonly appearing concrete defects and background. We compared two meta-learning approaches to find suitable convolutional neural network architectures for this challenging multi-class multi-target task. We observed that learned architectures have less overall parameters in addition to yielding better multi-target accuracy in comparison to best-in-practice CNN architectures from literature evaluated in the context of our application. We published a paper at the main conference of [CVPR 2019](http://cvpr2019.thecvf.com/). The code for this project is in PyTorch and Tensorflow.

[Publication](http://openaccess.thecvf.com/content_CVPR_2019/html/Mundt_Meta-Learning_Convolutional_Neural_Architectures_for_Multi-Target_Concrete_Defect_Classification_With_CVPR_2019_paper.html)|[Full Codebase](https://github.com/MrtnMndt/meta-learning-CODEBRIM)|[MetaQNN Codebase](https://github.com/SAGNIKMJR/CODEBRIM_MetaQNN)

I also got an opportunity to investigate a common trend of montonically incrementing feature amount with depth in a convolutional neural network (CNN). Several architectures with the same total feature amount but with different distribution of features across layers were trained and their performance vis-a-vis a certain task were compared. The comparison resulted in some interesting observations which questioned the afore-mentioned common practice. I co-authored a paper from this investigation at the [NeurIPS CRACT 2018 workshop](https://ml-critique-correct.github.io/). We wrote the code for this work in PyTorch.

[Publication](https://arxiv.org/abs/1812.05836)|[Codebase](https://github.com/MrtnMndt/Rethinking_CNN_Layerwise_Feature_Amounts)

Later during my time as an RA, my mentors and I worked on the problem of robust continual learning with deep generative replay and statistical outlier detection and rejection.  We used variational autoencoders with a classifier sitting on top of the latent embedding, to learn to make class-specific latent clusters (class-specific posterios) and continually generate image data from previously seen tasks. On top of this, we adapted the [OpenSet](https://arxiv.org/abs/1511.06233) algorithm to provide confidence bounds vis-a-vis the generated images actually belonging to the image data distribution seen until now, by exploiting the class-specific posteriors. This resulted in a system that can keep generating high-quality data and use that data to continually learn new tasks while robustly remembering old knowledge. We tested our framework on multiple benchmark datasets and got state-of-the-art classification results on intra-dataset continual learning across classes and cross-modality (music to image data, and vice-versa) continual learning across datasets. We have managed to publish a workshop paper from this project at the [ICCV Statistical Deep Learning for Computer Vision (SDLCV) 2019](http://www.sdlcv-workshop.com/) workshop. We are also going to submit a full paper to a tier-1 ML conference soon but have a preprint of it online already. The code from this work has been written in PyTorch.

[Preprint](https://arxiv.org/abs/1905.12019)|[Workshop publication](https://arxiv.org/abs/1908.09625)|[Codebase](https://github.com/MrtnMndt/OCDVAE_ContinualLearning)

# Research Internship @ Frankfurt Institute for Advanced Studies
<small>Mentor : [Prof. Christoph von der Malsburg]</small> 

<small>Topic : Depth estimation from rotational motion using dynamic neural fields with attractor states</small>

<small>Duration: January 2018 - Present</small>


This is an ongoing project. Here, the aim is to build a simple yet principled model of motion detection in the human cortex which has the ability to estimate the depth of a rigidly moving body, for eg. a rotating cube, when the eye can see the rotating body in rotation from only one side. Certain points of the rigid body, the eight vertices in the case of a cube, can be tracked and projected onto a plane when it is viewed from only one side as in the case of a camera. The different variables of motion in this case are the linear velocities of the points, the angular velocities and the positional coordinates of the points. The angular velocities are pre-given from another computational model which is not part of this pipeline or the trivial case of unit vector estimation for the angular velocities can be implemented and the actual angular velocity vector can be obtained by scaling the unit vector up by the pre-given scaling factor. Due to  mathematical dependencies among the variables of motion, ideally knowing any two of them should help in the accurate prediction of the third variable. But, in this case due to planar projection only two values for each of positional coordinates and the linear velocities can be known. This is turns calls for neural connections/fields which can detect velocities of moving points through the well-known delayed coincidence mechanism called Reichardt velocity detection, and use self-organization of the connections to exploit the mathematical inter-dependencies for converging to an accurate estimate even of the third unknown value of each of the positional coordinates and the linear velocities over a certain amount of training time. More information on the project is to be released after completion. Most of the code for this project has been written using Numpy and Scikit-learn.

[Codebase](https://github.com/SAGNIKMJR/DepthEstimation_from_Motion_in_Cortex)

# Bachelor Thesis @ Goethe University Frankfurt
<small>Mentors : [Prof. Visvanathan Ramesh], [Mr. Martin Mundt]</small> 

<small>Topic : Exploration of neural architecture search algorithms and their efficient application to image classification and image generation tasks</small>

<small>Duration: January - June 2018</small>


My bachelor thesis involved the study of reinforcement learning based architecture search techniques, Q-learning ([MetaQNN]) and REINFORCE ([ENAS]) in particular, and their application to vision tasks. The tasks were image classification, and image generation with variational autoencoders (VAEs) and generative adversarial networks (GANs) on benchmark vision datasets. I also focused on the designing of reward function for RL based search with VAEs because of lack of convergence of variational models during training. In addition, I tried to reformulate the loss function of VAEs to improve convergence and make their training more stable. Besides, it was noticed that the Q-learning based search require very long search schedules for convergence on most tasks. A modification to the Q-learning update rule which is actually a fully greedy tree search algorithm was proposed for architecture search with shorter schedules. Moreover, the Q-learning and REINFORCE based architecture search were applied to the task of multi-label classification for anomaly/defect detection and semantic segmentation on bridge data which had both background and defect images as part of the [AEROBI] project. The models found during the search were found to considerably outperform the hand-engineered models for the same data and a comparative analysis was reported and demonstrated as part of the AEROBI project outcome. This work involved the extensive use of Pytorch and Tensorflow.

[Thesis Report]|[CNN Codebase]|[VCAE Codebase]|[GAN Codebase]


# Research Internship @ Frankfurt Institute for Advanced Studies
<small>Mentor : [Prof. Christoph von der Malsburg]</small> 

<small>Topic : Image recognition using elastic graph matching</small>

<small>Duration: May - July 2017</small>

A principled image recognition system that used neural graph matching between model and image planes, and Gabor filters for feature extraction was built. A dynamic two-dimensional graph was created with Gabor filter stacks (corresponding to different orientations and frequencies) at each node. The dynamic nature of the graph (dynamic link architecture) allowed for global positioning of the whole grid corresponding to the center of gravity of the object to be recognized and local restricted movements of the nodes to account for local translations of object pixels and rotation of the grid and individual Gabor wavelets to offset the non-zero orientation, if any, of the object under consideration. This led to rotation and tranlation invariance of the system. This dynamic image graph was then matched against stored model graphs and the model graph with the best match gives the identity/label of the object recognized. Numpy and python were used for the code. A paper from the work on handwritten digit recognition got published at [JCP 2018].

[Publication]|[Codebase]

# Research Internship @ Indian Institute of Remote Sensing
<small>Mentor : [Ms. Shefali Agarwal]</small> 

<small>Topic : Time synchronization of terrestrial laser scanner and global positioning system in a mobile mapping system</small>

<small>Duration: May - July 2016</small>

In a mobile mapping system, a global positioning system (GPS) measures time and acquires the global coordinates (Cartesian or Azimuthal) very precisely with the help of satellites while the terrestrial laser scanner (TLS) records the local coordinates at the point of measurement. Although the TLS has a clock for measuring time, the least count of it is in milliseconds which renders it less precise when compared with the time measurement by the GPS where the precision is in nanoseconds. Effective synchronisation is required in this case where the data points produced by the TLS can be mapped to the data points produced by the GPS with the timestamps as reference. Hence, it is necessary to pass the timestamp information from the GPS to the TLS at every point of measurement to succesfully map data points from the two devices. The goal was achieved by using a third computer which used two different communication protocols to interact with the GPS (network time protocol) and the TLS (dynamic host configuration protocol). Code written in C++ with proprietary libraries (RivLib)from the TLS manufacturer and bash scripts were run on the third computer for timestamp transfer. Besides, C++ code for the extraction of TLS data into a human-readable format (comma separated values) was also written. A paper from this work was presented at the techinal festival in BITS Pilani, APOGEE, which fetched me the second prize in the category.

[Paper Presentation]|[Internship Report]|[Codebase]

[Prof. Visvanathan Ramesh]:<https://scholar.google.co.in/citations?hl=en&user=SS10xIgAAAAJ&view_op=list_works>
[AEROBI]:<http://www.aerobi.eu/>
[WACV 2019]:<http://wacv19.wacv.net/>
[Thesis Report]:<https://sagnikmjr.github.io/files/Bachelor_Thesis_Report.pdf>
[Codebase - Architecture Search - Image Classification]:<https://github.com/SAGNIKMJR/MetaQNN_ImageClassification_PyTorch>
[Codebase - Architecture Search - Image Generation - VCAE]:<https://github.com/SAGNIKMJR/MetaQNN_ImageGenerationVCAE_PyTorch>
[Codebase - Architecture Search - Image Generation - GAN]:<https://github.com/SAGNIKMJR/MetaQNN_ImageGenerationGAN_DiscriminatorFixed_PyTorch>
[Prof. Christoph von der Malsburg]:<https://en.wikipedia.org/wiki/Christoph_von_der_Malsburg>
[JCP 2018]:<http://www.jcomputers.us/>
[Publication]:<http://www.jcomputers.us/index.php?m=content&c=index&a=show&catid=201&id=2862>
[Codebase - Handwritten Image Recognition - Elastic Graph Matching]:<https://github.com/SAGNIKMJR/HandwrittenDigitRecognition_ElasticMatching_Python>
[Ms. Shefali Agarwal]:<https://www.iirs.gov.in/Shefali-profile>
[Paper Presentation]:<https://sagnikmjr.github.io/files/Time_Synchronisation_in_Mobile_Mapping_System.pdf>
[Codebase - Time Synchronization - Mobile Mapping System]:<https://github.com/SAGNIKMJR/Time-Synchronisation-of-Mobile-Mapping-System>
<!-- [Codebase - Depth Estimation - Motion in Cortex]:<https://github.com/SAGNIKMJR/DepthEstimation_from_Motion_in_Cortex>
 -->
 [Internship Report]:<https://sagnikmjr.github.io/files/IIRSInternshipReport.pdf>
[NIPS 2018 Continual Learning Workshop]:<https://sites.google.com/view/continual2018/home?authuser=0>
[CVPR 2019]:<http://cvpr2019.thecvf.com/>
[MetaQNN]:<https://arxiv.org/abs/1611.02167>
[ENAS]:<https://arxiv.org/abs/1802.03268>
[Mr. Martin Mundt]:<http://martin-mundt.com/>