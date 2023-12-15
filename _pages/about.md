permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I’m a PhD student at the Laboratory of Machine Learning & Health Informatics at the Computer Science and Engineering Department, [University of Connecticut](https://uconn.edu/), advised by [Prof. Jinbo Bi](http://www.engr.uconn.edu/~jinbo/). 

My research interests lie primarily in **reinforcement learning** (focusing on deep stochastic contexture bandit problem and Monte Carlo tree search) and **deep neural networks-based recommendation system** with an emphasis on self-attention module and click-through rate prediction.

explainable deep neural networks-based recommendation systems, reinforcement learning, and deep learning for MRI diagnostics, with an emphasis on **attention module**,  **stochastic contexture bandit problem**, and **DNN model diagnosing alcohol/nicotine use disorder with brain image datasets**.

# Experience

**01/2018 - Present, Research Assistant, University of Connecticut, US**

Research interests: Explainable deep neural networks-based recommendation system, reinforcement learning, and deep learning for MRI diagnostics.

**09/2014 – 01/2017, Research Assistant, Northeastern University, Shenyang, PR China**

Thesis: Research and Application of Algorithm on Knowledge Learning from Expert Game Records of Go

# Selected Publications (7 out of 18)
__[Polyhedron Attention Module: Learning Adaptive-order Interactions](https://openreview.net/forum?id=6JrckqCxtl)__    
**Tan Zhu**, Fei Dou, Xinyu Wang, Jin Lu, Jinbo Bi.
**NeurIPS 2023, (A<sup>+</sup> conference, acceptance rate: 26.1%)**

__[Machine Learning of Functional Connectivity to Biotype Alcohol and Nicotine Use Disorders](https://www.sciencedirect.com/science/article/pii/S2451902223002227)__  
**Tan Zhu**, Wuyi Wang, Yu Chen, Henry R Kranzler, Chiang-Shan R Li, Jinbo Bi.
Biological Psychiatry: Cognitive Neuroscience and Neuroimaging, 2023, __(Q1 journal, IF: 5.9)__

 __[On-Device Indoor Positioning: A Federated Reinforcement Learning Approach With Heterogeneous Devices](https://ieeexplore.ieee.org/document/10214616)__  
Fei Dou, Jin Lu, **Tan Zhu**, Jinbo Bi.
IEEE Internet of Things Journal, 2023, __(Q1 journal, IF: 9.9)__

__[Identifying Alcohol Misuse Biotypes from Neural Connectivity Markers and Concurrent Genetic Associations](https://www.nature.com/articles/s41398-022-01983-1)__  
**Tan Zhu**, Chloe Becquey, Yu Chen, Carl W. Lejuez, Chiang-Shan R. Li, Jinbo Bi.
Translational Psychiatry, 12(1), 253, 2022, __(by Nature Publishing Group, Q1 journal, IF: 7.9)__

__[Federated Optimization of ℓ 0-norm Regularized Sparse Learning](https://www.mdpi.com/1999-4893/15/9/319)__  
Qianqian Tong,Guannan Liang, Jiahao Ding, **Tan Zhu**, Miao Pan, Jinbo Bi.
Federated Optimization of ℓ 0-norm Regularized Sparse Learning. Algorithms, 15(9), 319, 2022, __(Q2 journal, IF: 2.3)__

__[An Efficient Algorithm for Deep Stochastic Contextual Bandits](https://ojs.aaai.org/index.php/AAAI/article/view/17335)__  
**Tan Zhu**, Guannan Liang, Chunjiang Zhu, Haining Li, Jinbo Bi.
**AAAI 2021, (A<sup>+</sup> conference, acceptance rate: 21.4%)**

__[Communication-optimal Distributed Dynamic Graph Clustering](https://ojs.aaai.org/index.php/AAAI/article/view/4547)__  
Chun Jiang Zhu, **Tan Zhu**, Kam-Yiu Lam, Song Han, and Jinbo Bi.
**AAAI 2019, (A<sup>+</sup> conference, acceptance rate: 16.2%)**

# Projects

## __Polyhedron Attention Module: Learning Adaptive-order Interactions__

<!-- Learning feature interactions can be the key for multivariate predictive modeling. ReLU-activated neural networks create piecewise linear prediction models, and other nonlinear activation functions lead to models with only high-order feature interactions. Recent methods incorporate candidate polynomial terms of fixed orders into deep learning, which is subject to the issue of c0--=ombinatorial explosion, or learn the orders that are difficult to adapt to different regions of the feature space. We propose a Polyhedron Attention Module (PAM) to create piecewise polynomial models where the input space is split into polyhedrons which define the different pieces and on each piece the hyperplanes that define the polyhedron boundary multiply to form the interactive terms, resulting in interactions of adaptive order to each piece. PAM is interpretable to identify important interactions in predicting a target. Theoretic analysis shows that PAM has stronger expression capability than ReLU-activated networks. Extensive experimental results demonstrate the superior classification performance of PAM on massive datasets of the click-through rate prediction and PAM can learn meaningful interaction effects in a medical problem. -->

* Design and implement a module called Polyhedron Attention Module (PAM) for deep neural networks to explicitly model the interaction effects among the model’s inputs on the model’s output. Results have been published in __NeurIPS 2023 (Acceptance rate: 26.1%)__ .
  <div>
  <img src="/images/nips_pipeline.jpg" height="400">
  </div>
* Our module splits the input space into subspaces (polyhedrons) and adaptively learns different interactive terms in each subspace. An input sample will be assigned to one or more subspaces, and interactions learned in these subspaces were used to predict the targets. Theoretic analysis shows that our module has stronger expression capability than ReLU-activated networks.
  <details close>
  <summary><strong>Click to see the example</strong></summary>
  <div>
    <img src="/images/nips_adaptive_interactions.jpg" height="800"> 
    </div>
  </details>
  
* Our model has state-of-the-art performance on massive datasets of the __click-through rate prediction__, a critical machine learning problem in the __recommendation system__.
  <details close>
  <summary> <strong>Click to see the result in our paper</strong> </summary>
  <div>
  <img src="/images/nips_result.jpg"  height="700"> 
  </div>   
  </details>
  
* Our module is interpretable to identify important interactions in predicting a target. Experiment shows that our module can learn meaningful interaction effects in a medical problem (predict brain age with brain image).
  <div>
  <img src="/images/model_interpretation.jpg"  height="250">
  </div>
  
## __An Efficient Algorithm for Deep Stochastic Contextual Bandits__
  <div>
  <img src="/images/AAAI_problem.jpg" height="400">
  </div>
* We formulate a stage-wised optimization algorithm for deep stochastic contextual bandits problem. Results have been published in __AAAI 2021 (Acceptance rate: 21.1%)__ .
  <details close>
  <summary> <strong>Click to see the pseudocode</strong> </summary>
  <hr>
  <div >
  <img src="/images/aaai_pseudo_code.jpg" height="400">
  </div>
  <hr>
  </details>
* We prove that with high probability, the action sequence chosen by this algorithm converges to a greedy action policy respecting a local optimal reward function.
  <details close>
  <summary> <strong>Click to see our theory conclusion in the published paper</strong>  </summary>
   <hr>
  <div >
  <img src="/images/theorem_conclusion.jpg" height="200">
  </div>
    <hr>
  </details>
* Extensive experiments have been performed to demonstrate the effectiveness and efficiency of the proposed algorithm on multiple real-world datasets.
  <details close>
  <summary> <strong>Click to see the result in our paper</strong> </summary>
  <div>
    <img src="/images/AAAI_performance.jpg" height="800"> 
    </div>
  </details>
  

## __Diagnosing Addictions with Artificial Neural Networks utilizing the knowledge of substance use biotypes__

* Design and implement the clustering pipeline to generate substance-use biotypes based on functional connectivity features (FCs) in the Functional magnetic resonance imaging (fMRI) matrix.
  <div>
  <img src="/images/brain_net.png" height="600"> 
  </div>
* Propose novel Artificial Neural Networks (ANN) diagnosing addictions with FCs of fMRI.
  <div >
  <img src="/images/classification_result.jpg"  width="500"/>
  </div>
  <details close>
  <summary> <strong>Click to see the architecture of the ANN</strong>  </summary>
  <div >
  <img src="/images/ANN_structure.png" height="400"> 
  </div>
  </details>
* Results have been published in _Translational Psychiatry_ __(Nature Communications, Q1 journal)__ and _Biological Psychiatry: Cognitive Neuroscience and Neuroimaging_ **(Q1 journal)**.



# Contact
Email: tan.zhu@uconn.com
