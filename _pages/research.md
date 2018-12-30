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

<small>Topics : Continuous learning, open set recognition and meta-learning  </small>

<small>Duration: July 2018 - Present</small>

[//]: # (Primarily, I have been jointly working on curating the novel COncrete DEfect BRidge IMage dataset (CODEBRIM) for multi-target classification of five commonly appearing concrete defects. We have compared two meta-learning approaches to find suitable convolutional neural network architectures for this challenging multi-class multi-target task. We have observed that learned architectures have less overall parameters in addition to yielding better multi-target accuracy in comparison to popular CNN architectures from the literature evaluated in the context of our application. We have jointly submitted a paper from this project to a tier-1 vision conference of the likes of ECCV, CVPR, ICCV etc.

[Submitted manuscript](https://drive.google.com/open?id=1Q3kgJ0BIyIb_dl-aUi-mmVzQ8xl_srfy)
)

Primarily, I have been jointly working on curating the novel COncrete DEfect BRidge IMage dataset (CODEBRIM) for multi-target classification of five commonly appearing concrete defects. We have compared two meta-learning approaches to find suitable convolutional neural network architectures for this challenging multi-class multi-target task. We have observed that learned architectures have less overall parameters in addition to
yielding better multi-target accuracy in comparison to popular CNN architectures from the literature evaluated in the context of our application. We have jointly submitted a paper from this project to a tier-1 vision conference of the likes of ECCV, CVPR, ICCV etc.

[Submitted manuscript](https://drive.google.com/open?id=1Q3kgJ0BIyIb_dl-aUi-mmVzQ8xl_srfy)


I also got an opportunity to investigate a common trend of montonically incrementing feature amount with depth in a convolutional neural network (CNN). Several architectures with the same total feature amount but with different distribution of features across layers were trained and their performance vis-a-vis a certain task were compared. The comparison resulted in some interesting observations which questioned the afore-mentioned common practice. I co-authored a paper from this investigation at the [NeurIPS CRACT 2018 workshop](https://ml-critique-correct.github.io/)

[Publication](https://www.dropbox.com/s/vjt0on2dxizzv8v/CRACT_2018_paper_19.pdf?dl=0)|[Codebase](https://github.com/MrtnMndt/Rethinking_CNN_Layerwise_Feature_Amounts)

This is another ongoing project. Weight sharing in neural networks can result in efficient distillation of knowledge learnt from earlier tasks and prevent catastrophic forgetting when a new task is faced. Architecture search with weight sharing may produce optimal architectures for new tasks with knowledge retained from old tasks. More information on the project is to be released after completion. 

Moreover, I am working on the problem of openset recognition using variational deep neural networks for recognition of unknown data points or 'fooling/rubbish' data. This enables the network to recognize outliers or adversarial data on the basis of statistical measures  involving the network mean and variance. This can considerably speed up training while continuously training a network and reduce the number of false classifications. 

# Research Internship @ Frankfurt Institute for Advanced Studies
<small>Mentor : [Prof. Christoph von der Malsburg]</small> 

<small>Topic : Depth estimation from rotational motion using dynamic neural fields with attractor states</small>

<small>Duration: January 2018 - Present</small>


This is another ongoing project. In this one, the aim is to build a simple yet principled model of motion detection in the human cortex which has the ability to estimate the depth of a rigidly moving body, for eg. a rotating cube, when the eye can see the rotating body in rotation from only one side. Certain points of the rigid body, the eight vertices in the case of a cube, can be tracked and projected onto a plane when it is viewed from only one side as in the case of a camera. The different variables of motion in this case are the linear velocities of the points, the angular velocities and the positional coordinates of the points. The angular velocities are pre-given from another computational model which is not part of this pipeline or the trivial case of unit vector estimation for the angular velocities can be implemented and the actual angular velocity vector can be obtained by scaling the unit vector up by the pre-given scaling factor. Due to  mathematical dependencies among the variables of motion, ideally knowing any two of them should help in the accurate prediction of the third variable. But, in this case due to planar projection only two values for each of positional coordinates and the linear velocities can be known. This is turns calls for neural connections/fields which can detect velocities of moving points through the well-known delayed coincidence mechanism called Reichardt velocity detection, and use self-organization of the connections to exploit the mathematical inter-dependencies for converging to an accurate estimate even of the third unknown value of each of the positional coordinates and the linear velocities over a certain amount of training time. More information on the project is to be released after completion.

[Codebase - Depth Estimation - Motion in Cortex]

# Bachelor Thesis @ Goethe University Frankfurt
<small>Mentors : [Prof. Visvanathan Ramesh], [Mr. Martin Mundt]</small> 

<small>Topic : Exploration of neural architecture search algorithms and their efficient application to image classification and image generation tasks</small>

<small>Duration: January - June 2018</small>


My bachelor thesis involved the study of reinforcement learning based architecture search techniques, Q-learning ([MetaQNN]) and REINFORCE ([ENAS]) in particular, and their application to vision tasks. The tasks were image classification, and image generation with variational autoencoders (VAEs) and generative adversarial networks (GANs) on benchmark vision datasets. I also focused on the designing of reward function for RL based search with VAEs because of lack of convergence of variational models during training. In addition, I tried to reformulate the loss function of VAEs to improve convergence and make their training more stable. Besides, it was noticed that the Q-learning based search require very long search schedules for convergence on most tasks. A modification to the Q-learning update rule which is actually a fully greedy tree search algorithm was proposed for architecture search with shorter schedules. Moreover, the Q-learning and REINFORCE based architecture search were applied to the task of multi-label classification for anomaly/defect detection and semantic segmentation on bridge data which had both background and defect images as part of the [AEROBI] project. The models found during the search were found to considerably outperform the hand-engineered models for the same data and a comparative analysis was reported and demonstrated as part of the AEROBI project outcome. This work extensively involved the use of Pytorch and Tensorflow

[Thesis Report]|[Codebase - Architecture Search - Image Classification]|[Codebase - Architecture Search - Image Generation - VCAE]|[Codebase - Architecture Search - Image Generation - GAN]


# Research Internship @ Frankfurt Institute for Advanced Studies
<small>Mentor : [Prof. Christoph von der Malsburg]</small> 

<small>Topic : Image recognition using elastic graph matching</small>

<small>Duration: May - July 2017</small>

A principled image recognition system that used neural graph matching between model and image planes, and Gabor filters for feature extraction was built. A dynamic two-dimensional graph was created with Gabor filter stacks (corresponding to different orientations and frequencies) at each node. The dynamic nature of the graph (dynamic link architecture) allowed for global positioning of the whole grid corresponding to the center of gravity of the object to be recognized and local restricted movements of the nodes to account for local translations of object pixels and rotation of the grid and individual Gabor wavelets to offset the non-zero orientation, if any, of the object under consideration. This led to rotation and tranlation invariance of the system. This dynamic image graph was then matched against stored model graphs and the model graph with the best match gives the identity/label of the object recognized. Numpy and python were used for the code. A paper from the work on handwritten digit recognition got published at [JCP 2018].

[Publication]|[Codebase - Handwritten Image Recognition - Elastic Graph Matching]

# Research Internship @ Indian Institute of Remote Sensing
<small>Mentor : [Ms. Shefali Agarwal]</small> 

<small>Topic : Time synchronization of terrestrial laser scanner and global positioning system in a mobile mapping system</small>

<small>Duration: May - July 2016</small>

In a mobile mapping system, a global positioning system (GPS) measures time and acquires the global coordinates (Cartesian or Azimuthal) very precisely with the help of satellites while the terrestrial laser scanner (TLS) records the local coordinates at the point of measurement. Although the TLS has a clock for measuring time, the least count of it is in milliseconds which renders it less precise when compared with the time measurement by the GPS where the precision is in nanoseconds. Effective synchronisation is required in this case where the data points produced by the TLS can be mapped to the data points produced by the GPS with the timestamps as reference. Hence, it is necessary to pass the timestamp information from the GPS to the TLS at every point of measurement to succesfully map data points from the two devices. The goal was achieved by using a third computer which used two different communication protocols to interact with the GPS (network time protocol) and the TLS (dynamic host configuration protocol). Code written in C++ with proprietary libraries (RivLib)from the TLS manufacturer and bash scripts were run on the third computer for timestamp transfer. Besides, C++ code for the extraction of TLS data into a human-readable format (comma separated values) was also written. A paper from this work was presented at the techinal festival in BITS Pilani, APOGEE, which fetched me the second prize in the category.

[Paper Presentation]|[Internship Report]|[Codebase - Time Synchronization - Mobile Mapping System]

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
[Codebase - Depth Estimation - Motion in Cortex]:<https://github.com/SAGNIKMJR/DepthEstimation_from_Motion_in_Cortex>
[Internship Report]:<https://sagnikmjr.github.io/files/IIRSInternshipReport.pdf>
[NIPS 2018 Continual Learning Workshop]:<https://sites.google.com/view/continual2018/home?authuser=0>
[CVPR 2019]:<http://cvpr2019.thecvf.com/>
[MetaQNN]:<https://arxiv.org/abs/1611.02167>
[ENAS]:<https://arxiv.org/abs/1802.03268>
[Mr. Martin Mundt]:<http://martin-mundt.com/>