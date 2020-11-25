---
title: "We are More than Our Joints: Predicting how 3D Bodies Move"
collection: publications
permalink: /publication/MOJO
date: 2020-11-20
venue: 'tbd'
paperurl: 'tbd'
---
![alt text](http://yz-cnsdqz.github.io/images/MOJO-teaser.png)<!-- .element height="20%" width="20%" -->

__Abstract:__ 

A key step towards understanding human behavior is the prediction of 3D human motion. Successful solutions have many applications in human tracking, HCI, and graphics. Most previous work focuses on predicting a time series of future 3D joint locations given a sequence 3D joints from the past. This Euclidean formulation generally works better than predicting pose in terms of joint rotations. Body joint locations, however, do not fully constrain 3D human pose, leaving degrees of freedom (like rotation about a limb) undefined, making it hard to animate a realistic human from only the joints. Note that the 3D joints can be viewed as a sparse {\em point cloud}. Thus the problem of human motion prediction can be seen as a problem of point cloud prediction. With this observation, we instead predict a sparse set of locations on the body {\em surface} that correspond to motion capture markers. Given such markers, we fit a parametric body model to recover the 3D body shape and pose of the person. These sparse surface markers also carry detailed information about human movement that is not present in the joints, increasing the naturalness of the predicted motions. Using the AMASS dataset, we train MOJO (More than Our JOints), which is a novel variational autoencoder with a latent DCT space that generates motions from latent frequencies. MOJO preserves the full temporal resolution of the input motion, and sampling from the latent frequencies explicitly introduces high-frequency components into the generated motion. We note that motion prediction methods accumulate errors over time, resulting in joints or markers that diverge from true human bodies. To address this, we exploit the body model and fit SMPL-X to the predictions at each time step, projecting the solution back onto the space of valid bodies. These valid markers are then propagated in time. Quantitative and qualitative experiments show that our approach produces state-of-the-art results and realistic 3D body animations. Code will be made available for research purposes.

[Project Page](../MOJO/MOJO.html)



