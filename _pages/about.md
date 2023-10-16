---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I’m a PhD student at the Laboratory of Machine Learning & Health Informatics at the Computer Science and Engineering Department, [University of Connecticut](https://uconn.edu/), advised by [Prof. Jinbo Bi](http://www.engr.uconn.edu/~jinbo/). 

My research interests lie primarily in explainable recommendation systems, reinforcement learning, and deep learning-based Disease Diagnosis models, with an emphasis on Click-through rate (CTR) prediction, stochastic contexture bandit problem, DNN model diagnosing alcohol/nicotine use disorder using brain Magnetic resonance imaging (MRI) image datasets.

## Experience

**01/2018 - Present, Research Assistant, University of Connecticut, US**
<!--- * Designed graph neural networks, NLP, machine learning methods to improve drug discovery, knowledge graph completion, depression detection and so on. -->
<!--- * Supervisors: [Prof. Jinbo Bi](http://www.engr.uconn.edu/~jinbo/) and [Prof. Fei Wang](https://scholar.google.com/citations?user=FjCbjDYAAAAJ&hl=en) (Advised by Prof. Wang for a year).-->

**09/2014 – 01/2017, Research Assistant, Northeastern University, Shenyang, PR China**

## Projects

__Polyhedron Attention Module: Learning Adaptive-order Interactions__

<!-- Learning feature interactions can be the key for multivariate predictive modeling. ReLU-activated neural networks create piecewise linear prediction models, and other nonlinear activation functions lead to models with only high-order feature interactions. Recent methods incorporate candidate polynomial terms of fixed orders into deep learning, which is subject to the issue of c0--=ombinatorial explosion, or learn the orders that are difficult to adapt to different regions of the feature space. We propose a Polyhedron Attention Module (PAM) to create piecewise polynomial models where the input space is split into polyhedrons which define the different pieces and on each piece the hyperplanes that define the polyhedron boundary multiply to form the interactive terms, resulting in interactions of adaptive order to each piece. PAM is interpretable to identify important interactions in predicting a target. Theoretic analysis shows that PAM has stronger expression capability than ReLU-activated networks. Extensive experimental results demonstrate the superior classification performance of PAM on massive datasets of the click-through rate prediction and PAM can learn meaningful interaction effects in a medical problem. -->

* Design and implement a module called Polyhedron Attention Module (PAM) for deep neural networks (DNN) to explicitly model the interactions among the model's inputs on the target. Results have been published in __NeurIPS 2023 (Accept Ratio: 26.1%)__ .
  <div>
  <img src="/images/nips_pipeline.jpg" height="400">
  </div>
* Our module splits the input space into subspaces (polyhedrons) and adaptively learns different interactive terms in each subspace. An input sample will be assigned to one or more subspaces, and interactions learned in these subspaces were used to predict the targets. Theoretic analysis shows that our module has stronger expression capability than ReLU-activated networks.
  <details close>
  <summary> Click to see the example </summary>
  <div>
    <img src="/images/nips_adaptive_interactions.jpg" height="800"> 
    </div>
  </details>
  
* Our model has state-of-the-art performance on massive datasets of the __click-through rate prediction__, a critical machine learning problem in the __recommendation system__.
  <details close>
  <summary> Click to see the result in our paper </summary>
  <div>
  <img src="/images/nips_result.jpg"  height="700"> 
  </div>   
  </details>
  
* Our module is interpretable to identify important interactions in predicting a target. Experiment shows that our module can learn meaningful interaction effects in a medical problem (predict brain age with brain image).
  <div>
  <img src="/images/model_interpretation.jpg"  height="250">
  </div>
  
__An Efficient Algorithm for Deep Stochastic Contextual Bandits__
  <div>
  <img src="/images/AAAI_problem.jpg" height="400">
  </div>
* We formulate a stage-wised optimization algorithm for deep stochastic contextual bandits problem. Results have been published in __AAAI 2021 (Accept Ratio: 21.1%)__ .
  <details close>
  <summary> Click to see the pseudocode </summary>
  <hr>
  <div >
  <img src="/images/aaai_pseudo_code.jpg" height="400">
  </div>
  <hr>
  </details>
* We prove that with high probability, the action sequence chosen by this algorithm converges to a greedy action policy respecting a local optimal reward function.
  <details close>
  <summary> Click to see our theory conclusion in the published paper  </summary>
   <hr>
  <div >
  <img src="/images/theorem_conclusion.jpg" height="200">
  </div>
    <hr>
  </details>
* Extensive experiments have been performed to demonstrate the effectiveness and efficiency of the proposed algorithm on multiple real-world datasets.
  <details close>
  <summary> Click to see the result in our paper </summary>
  <div>
    <img src="/images/AAAI_performance.jpg" height="800"> 
    </div>
  </details>
  

__Diagnosing Addictions with Artificial Neural Networks utilizing the knowledge of substance use biotypes__

* Design and implement the clustering pipeline to generate substance-use biotypes based on functional connectivity features (FCs) in the Functional magnetic resonance imaging (fMRI) matrix.
  <div>
  <img src="/images/brain_net.png" height="600"> 
  </div>
* Propose novel Artificial Neural Networks (ANN) diagnosing addictions with FCs of fMRI.
  
  <img src="/images/classification_result.jpg"  height="250">
  
  <details close>
  <summary> Click to see the architecture of the ANN  </summary>
  <div >
  <img src="/images/ANN_structure.png" height="400"> 
  </div>
  </details>
* Results have been published in _Translational Psychiatry_ __(Nature Communications, Q1 journal)__ and _Biological Psychiatry: Cognitive Neuroscience and Neuroimaging_ **(Q1 journal)**.


## Selected Publications
__[Polyhedron Attention Module: Learning Adaptive-order Interactions](https://openreview.net/forum?id=6JrckqCxtl&noteId=zIxILt5xSz)__  
**Tan Zhu**, Fei Dou, Xinyu Wang, Jin Lu, Jinbo Bi.
**NeurIPS 2023, (Accept Ratio: 26.1%)**

__[Machine Learning of Functional Connectivity to Biotype Alcohol and Nicotine Use Disorders](https://www.sciencedirect.com/science/article/pii/S2451902223002227)__  
**Tan Zhu**, Wuyi Wang, Yu Chen, Henry R Kranzler, Chiang-Shan R Li, Jinbo Bi.
Biological Psychiatry: Cognitive Neuroscience and Neuroimaging, 2023, __(Q1 journal)__

 __[On-Device Indoor Positioning: A Federated Reinforcement Learning Approach With Heterogeneous Devices](https://ieeexplore.ieee.org/document/10214616)__  
Fei Dou, Jin Lu, **Tan Zhu**, Jinbo Bi.
IEEE Internet of Things Journal, 2023, __(Q1 journal)__

__[Identifying Alcohol Misuse Biotypes from Neural Connectivity Markers and Concurrent Genetic Associations](https://www.nature.com/articles/s41398-022-01983-1)__  
**Tan Zhu**, Chloe Becquey, Yu Chen, Carl W. Lejuez, Chiang-Shan R. Li, Jinbo Bi.
Translational Psychiatry, 12(1), 253, 2022, __(Nature Communications, Q1 journal)__

__[Federated Optimization of ℓ 0-norm Regularized Sparse Learning](https://www.mdpi.com/1999-4893/15/9/319)__  
Qianqian Tong,Guannan Liang, Jiahao Ding, **Tan Zhu**, Miao Pan, Jinbo Bi.
Federated Optimization of ℓ 0-norm Regularized Sparse Learning. Algorithms, 15(9), 319, 2022, __(Q2 journal)__

__[An Efficient Algorithm for Deep Stochastic Contextual Bandits](https://ojs.aaai.org/index.php/AAAI/article/view/17335)__  
**Tan Zhu**, Guannan Liang, Chunjiang Zhu, Haining Li, Jinbo Bi.
**AAAI 2021, (Accept Ratio: 21.1%)**

__[Communication-optimal Distributed Dynamic Graph Clustering](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9275443/)__
Chun Jiang Zhu, **Tan Zhu**, Kam-Yiu Lam, Song Han, and Jinbo Bi.
**AAAI 2019, (Accept Ratio: 19.2%)**

## Contact
Email: tan.zhu@uconn.com
