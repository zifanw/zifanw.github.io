# About Me

![](./images/photo.jpg)

I’m a second-year Ph.D. student in Electrical and Computer Enigneering, Carnegie Mellon University (CMU). I am co-advised by Prof.[Anupam Datta](http://www.andrew.cmu.edu/user/danupam/) and Prof. [Matt Fredrikson](http://www.cs.cmu.edu/~mfredrik/) in the [Accountable System Lab](https://fairlyaccountable.org). My current concentration focuses on the development of interpretations for deep neural networks. I received my Master degree in Electrical & Computer Enigneering from CMU, Silicon Valley Campus, a small and warm community located in Mountain View, CA. Before attending CMU, I received my Bachelor degree in Electronic Science and Technology from Beijing Institute of Technology, Beijing, China. Outside my professional life, I am an outgoing video game player, a hiker who also loves camping and road trip, and right now I am learning to play the skateboard. I also have a cat whose name is Pikachu. He is handsome and active. 


**Check out my latest [Resume](https://drive.google.com/file/d/1hSX3ouJPLr_LI8ANhXMPfkMYiSHNNwTb/view?usp=sharing)**



# News!
- Check out our *AAAI-21* Tutorial on model explainability from our tutorial [homepage](https://fairlyaccountable.org/aaai-2021-tutorial/) and recordings from the [AAAI virtual cite](https://virtual.2021.aaai.org/tutorial_AH3.html).

- Check out [TruLens](https://github.com/truera/trulens), a Python library for explaining Deep Neural Networks.

# Publicaitons 

### Smoothed Geometry for Robust Attribution [NeurIPS 2020]  

**Zifan Wang**, Haofan Wang, Shakul Ramkumar, Matt Fredrikson, Piotr Mardziel, Anupam Datta

Check the [paper](https://arxiv.org/pdf/2006.06643v1.pdf), [poster](./resource/doc/smooth_poster.pdf)

*Feature attributions are a popular tool for explaining the behavior of Deep Neural Networks (DNNs), but have recently been shown to be vulnerable to attacks that produce divergent explanations for nearby inputs. This lack of robustness is especially problematic in high-stakes applications where adversarially-manipulated explanations could impair safety and trustworthiness. Building on a geometric understanding of these attacks presented in recent work, we identify Lipschitz continuity conditions on models' gradient that lead to robust gradient-based attributions, and observe that smoothness may also be related to the ability of an attack to transfer across multiple attribution methods. To mitigate these attacks in practice, we propose an inexpensive regularization method that promotes these conditions in DNNs, as well as a stochastic smoothing technique that does not require re-training. Our experiments on a range of image models demonstrate that both of these mitigations consistently improve attribution robustness, and confirm the role that smooth geometry plays in these attacks on real, large-scale models.*

***



### Interpreting Interpretations: Organizing Attribution Methods by Criteria [CVPR Workshop 2020]

**Zifan Wang**, Piotr Mardziel, Anupam Datta, Matt Fredrikson

Check the [paper](https://arxiv.org/abs/2002.07985), [slides](./resource/IIOAMC/slides.pdf) and [video](https://youtu.be/cyYHoTyNMfQ)

*Motivated by distinct, though related, criteria, a growing number of attribution methods have been developed tointerprete deep learning. While each relies on the interpretability of the concept of "importance" and our ability to visualize patterns, explanations produced by the methods often differ. As a result, input attribution for vision models fail to provide any level of human understanding of model behaviour. In this work we expand the foundationsof human-understandable concepts with which attributionscan be interpreted beyond "importance" and its visualization; we incorporate the logical concepts of necessity andsufficiency, and the concept of proportionality. We definemetrics to represent these concepts as quantitative aspectsof an attribution. This allows us to compare attributionsproduced by different methods and interpret them in novelways: to what extent does this attribution (or this method)represent the necessity or sufficiency of the highlighted inputs, and to what extent is it proportional? We evaluate our measures on a collection of methods explaining convolutional neural networks (CNN) for image classification. We conclude that some attribution methods are more appropriate for interpretation in terms of necessity while others are in terms of sufficiency, while no method is always the most appropriate in terms of both.*

***



### Score-CAM: Score-Weighted Visual Explanations for Convolutional Neural Networks [CVPR Workshop 2020]

Haofan Wang, **Zifan Wang**, Mengnan Du, Fan Yang, Zijian Zhang, Sirui Ding, Piotr Mardziel, Xia Hu 

Check the [paper](http://openaccess.thecvf.com/content_CVPRW_2020/papers/w1/Wang_Score-CAM_Score-Weighted_Visual_Explanations_for_Convolutional_Neural_Networks_CVPRW_2020_paper.pdf), [slides](./resource/Score_CAM/slides.pdf) and [video](https://www.youtube.com/watch?v=lB0nZ71ASpo)

*Recently, increasing attention has been drawn to the internal mechanisms of convolutional neural networks, and the reason why the network makes specific decisions. In this paper, we develop a novel post-hoc visual explanation method called Score-CAM based on class activation mapping. Unlike previous class activation mapping based approaches, Score-CAM gets rid of the dependence on gradients by obtaining the weight of each activation map through its forward passing score on target class, the final result is obtained by a linear combination of weights and activation maps. We demonstrate that Score-CAM achieves better visual performance and fairness for interpreting the decision making process. Our approach outperforms previous methods on both recognition and localization tasks, it also passes the sanity check. We also indicate its application as debugging tools. Official code has been released.*



# Preprint

### Boundary Attributions Provide Normal (Vector) Explanations

**Zifan Wang**, Matt Fredrikson, Anupam Datta

Check the [paper](https://arxiv.org/pdf/2103.11257.pdf)

*Recent work on explaining Deep Neural Networks (DNNs) focuses on attributing the model's output scores to input features. However, when it comes to classification problems, a more fundamental question is how much does each feature contributes to the model's decision to classify an input instance into a specific class. Our first contribution is Boundary Attribution, a new explanation method to address this question. BA leverages an understanding of the geometry of activation regions. Specifically, they involve computing (and aggregating) normal vectors of the local decision boundaries for the target input. Our second contribution is a set of analytical results connecting the adversarial robustness of the network and the quality of gradient-based explanations. Specifically, we prove two theorems for ReLU networks: BA of randomized smoothed networks or robustly trained networks is much closer to non-boundary attribution methods than that in standard networks. These analytics encourage users to improve model robustness for high-quality explanations. Finally, we evaluate the proposed methods on ImageNet and show BAs produce more concentrated and sharper visualizations compared with non-boundary ones. We further demonstrate that our method also helps to reduce the sensitivity of attributions to the baseline input if one is required.*

***


### Globally-Robust Neural Networks

Klas Leino, **Zifan Wang**, Matt Fredrikson

Check the [paper](https://arxiv.org/pdf/2102.08452.pdf)

*The threat of adversarial examples has motivated work on training certifiably robust neural networks, to facilitate efficient verification of local robustness at inference time. We formalize a notion of global robustness, which captures the operational properties of on-line local robustness certification while yielding a natural learning objective for robust training. We show that widely-used architectures can be easily adapted to this objective by incorporating efficient global Lipschitz bounds into the network, yielding certifiably-robust models by construction that achieve state-of-the-art verifiable accuracy. Notably, this approach requires significantly less time and memory than recent certifiable training methods, and leads to negligible costs when certifying points on-line; for example, our evaluation shows that it is possible to train a large tiny-imagenet model in a matter of hours. We posit that this is possible using inexpensive global bounds—despite prior suggestions that tighter local bounds are needed for good performance—because these models are trained to achieve tighter global bounds. Namely, we prove that the maximum achievable verifiable accuracy for a given dataset is not improved by using a local bound.*

***

### Reconstructing Actions To Explain Deep Reinforcement Learning

**Zifan Wang\***, Xuan Chen\*, Yucai Fan, Bonan Jin, Piotr Mardziel, Carlee Joe-Wong, Anupam Datta

Check the [paper](https://arxiv.org/pdf/2009.08507.pdf)

*Feature attribution has been a foundational building block for explaining the input feature importance in supervised learning with Deep Neural Network (DNNs), but face new challenges when applied to deep Reinforcement Learning (RL).We propose a new approach to explaining deep RL actions by defining a class of \emph{action reconstruction} functions that mimic the behavior of a network in deep RL. This approach allows us to answer more complex explainability questions than direct application of DNN attribution methods, which we adapt to \emph{behavior-level attributions} in building our action reconstructions. It also allows us to define \emph{agreement}, a metric for quantitatively evaluating the explainability of our methods. Our experiments on a variety of Atari games suggest that perturbation-based attribution methods are significantly more suitable in reconstructing actions to explain the deep RL agent than alternative attribution methods, and show greater \emph{agreement} than existing explainability work utilizing attention. We further show that action reconstruction allows us to demonstrate how a deep agent learns to play Pac-Man game.*

***



### Towards Frequency-Based Explanation for Robust CNN

**Zifan Wang**, Yilin Yang, Ankit Shrivastava, Varun Rawal, Zihao Ding

Check the [paper](https://arxiv.org/abs/2005.03141) and [video](https://www.youtube.com/watch?v=GbwO8Qh-Wv0)

*Current explanation techniques towards a transparent Convolutional Neural Network (CNN) mainly focuses on building connections between the human-understandable input features with models' prediction, overlooking an alternative representation of the input, the frequency components decomposition. In this work, we present an analysis of the connection between the distribution of frequency components in the input dataset and the reasoning process the model learns from the data. We further provide quantification analysis about the contribution of different frequency components toward the model's prediction. We show that the vulnerability of the model against tiny distortions is a result of the model is relying on the high-frequency features, the target features of the adversarial (black and white-box) attackers, to make the prediction. We further show that if the model develops stronger association between the low-frequency component with true labels, the model is more robust, which is the explanation of why adversarially trained models are more robust against tiny distortions.*

***



### Abstracting Influence Paths for Explaining (Contextualization of) BERT Models

Kaiji Lu, **Zifan Wang**, Piotr Mardzie, and Anupam Datta

Check the [paper](https://arxiv.org/abs/2011.00740) 

*While “attention is all you need” may be proving true, we do not yet know why: attention-based models such as BERT are superior but how they contextualize information even for simple grammatical rules such as subject-verb number agreement (SVA) is uncertain. We introduce multi-partite patterns, abstractions of sets of paths through a neural network model. Patterns quantify and localize the effect of an input concept (e.g., a subject’s number) on an output concept (e.g. corresponding verb’s number) to paths passing through a sequence of model components, thus surfacing how BERT contextualizes information. We describe guided pattern refinement, an efficient search procedure for finding patterns representative of concept-critical paths. We discover that patterns generate succinct and meaningful explanations for BERT, highlighted by “copy” and “transfer” operations implemented by skip connections and attention heads, respectively. We also show how pattern visualizations help us understand how BERT contextualizes SVA across clauses, and why it makes errors in some cases while succeeding in others.*


# Open-Source Projects

### [TruLens](https://github.com/truera/trulens): Library for Explaining Deep Neural Networks.

```
@misc{Trulens,
  doi = {10.5281/ZENODO.4495856},
  url = {https://zenodo.org/record/4495856},
  author = {Leino, Klas and Shih, Ricardo and Fredrikson, Matt and She, Jennifer and Wang, Zifan and Lu, Caleb and Sen, Shayak and Gopinath, Divya and {, Anupam}},
  title = {truera/trulens: Trulens},
  publisher = {Zenodo},
  year = {2021},
  copyright = {Open Access}
}
```



# Teaching Assistance

**Fall 2019**          CMU 18-661: [Introduction to Machine Learning for Engineers](https://18661.github.io/)

**Spring 2020**    CMU 18-739: [Security and Fairness of Deep Learning](http://www.archive.ece.cmu.edu/~ece739/index.html)



# Presentations

### [2020-05-16] 言聚 Talk

强大却无法理解的AI, 该不该使用？[Link](https://mp.weixin.qq.com/s/sjHVnp7sRN0eMf9c-1DDjQ)



### [2020-07-15] AISC Presentation

Towards Frequency-Based Explanation for Robust CNN [Link](https://ai.science/e/towards-frequency-based-explanation-for-robust-cnn--hBiCzxIOpi3iOm0woCyY)



