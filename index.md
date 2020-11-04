# About Me

![](./images/photo.jpg)

I’m a second-year Ph.D. student in Electrical and Computer Enigneering, Carnegie Mellon University (CMU). I am co-advised by Prof.[Anupam Datta](http://www.andrew.cmu.edu/user/danupam/) and Prof. [Matt Fredrikson](http://www.cs.cmu.edu/~mfredrik/) in the [Accountable System Lab](https://fairlyaccountable.org). My current concentration focuses on the development of interpretations for deep neural networks. I received my Master degree in Electrical & Computer Enigneering from CMU, Silicon Valley Campus, a small and warm community located in Mountain View, CA. Before attending CMU, I received my Bachelor degree in Electronic Science and Technology from Beijing Institute of Technology, Beijing, China. Outside my professional life, I am an outgoing video game player, a hiker who also loves camping and road trip, and right now I am learning to play the skateboard. I also have a cat whose name is Pikachu. He is handsome and active. 



**Check out my latest [Resume](https://drive.google.com/file/d/1hSX3ouJPLr_LI8ANhXMPfkMYiSHNNwTb/view?usp=sharing)**



# Publicaitons 

### Smoothed Geometry for Robust Attribution [NeurIPS 2020]  

**Zifan Wang**, Haofan Wang, Shakul Ramkumar, Matt Fredrikson, Piotr Mardziel, Anupam Datta

Check the [paper](https://arxiv.org/pdf/2006.06643v1.pdf)

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

### Towards Behavior-Level Explanation for Deep Reinforcement Learning

Xuan Chen, **Zifan Wang**, Yucai Fan, Bonan Jin, Piotr Mardziel, Carlee Joe-Wong, Anupam Datta

Check the [paper](https://arxiv.org/pdf/2009.08507.pdf)

*Current explanation techniques towards a transparent Convolutional Neural Network (CNN) mainly focuses on building connections between the human-understandable input features with models' prediction, overlooking an alternative representation of the input, the frequency components decomposition. In this work, we present an analysis of the connection between the distribution of frequency components in the input dataset and the reasoning process the model learns from the data. We further provide quantification analysis about the contribution of different frequency components toward the model's prediction. We show that the vulnerability of the model against tiny distortions is a result of the model is relying on the high-frequency features, the target features of the adversarial (black and white-box) attackers, to make the prediction. We further show that if the model develops stronger association between the low-frequency component with true labels, the model is more robust, which is the explanation of why adversarially trained models are more robust against tiny distortions.*

***



### Towards Frequency-Based Explanation for Robust CNN

**Zifan Wang**, Yilin Yang, Ankit Shrivastava, Varun Rawal, Zihao Ding

Check the [paper](https://arxiv.org/abs/2005.03141) and [video](https://www.youtube.com/watch?v=GbwO8Qh-Wv0)

*Current explanation techniques towards a transparent Convolutional Neural Network (CNN) mainly focuses on building connections between the human-understandable input features with models' prediction, overlooking an alternative representation of the input, the frequency components decomposition. In this work, we present an analysis of the connection between the distribution of frequency components in the input dataset and the reasoning process the model learns from the data. We further provide quantification analysis about the contribution of different frequency components toward the model's prediction. We show that the vulnerability of the model against tiny distortions is a result of the model is relying on the high-frequency features, the target features of the adversarial (black and white-box) attackers, to make the prediction. We further show that if the model develops stronger association between the low-frequency component with true labels, the model is more robust, which is the explanation of why adversarially trained models are more robust against tiny distortions.*

***



### Abstracting Influence Paths for Explaining (Contextualization of) BERT Models

Kaiji Lu, **Zifan Wang**, Piotr Mardzie, and Anupam Datta

*While “attention is all you need” may be proving true, we do not yet know why: attention-based models such as BERT are superior but how they contextualize information even for simple grammatical rules such as subject-verb number agreement (SVA) is uncertain. We introduce multi-partite patterns, abstractions of sets of paths through a neural network model. Patterns quantify and localize the effect of an input concept (e.g., a subject’s number) on an output concept (e.g. corresponding verb’s number) to paths passing through a sequence of model components, thus surfacing how BERT contextualizes information. We describe guided pattern refinement, an efficient search procedure for finding patterns representative of concept-critical paths. We discover that patterns generate succinct and meaningful explanations for BERT, highlighted by “copy” and “transfer” operations implemented by skip connections and attention heads, respectively. We also show how pattern visualizations help us understand how BERT contextualizes SVA across clauses, and why it makes errors in some cases while succeeding in others.*



# Teaching Assistance

**Fall 2019**          CMU 18-661: [Introduction to Machine Learning for Engineers](https://18661.github.io/)

**Spring 2020**    CMU 18-739: [Security and Fairness of Deep Learning](http://www.archive.ece.cmu.edu/~ece739/index.html)



# Presentations

### [2020-05-16] 言聚 Talk

强大却无法理解的AI, 该不该使用？[Link](https://mp.weixin.qq.com/s/sjHVnp7sRN0eMf9c-1DDjQ)



### [2020-07-15] AISC Presentation

Towards Frequency-Based Explanation for Robust CNN [Link](https://ai.science/e/towards-frequency-based-explanation-for-robust-cnn--hBiCzxIOpi3iOm0woCyY)



