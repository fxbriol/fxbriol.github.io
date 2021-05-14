---
title: "Inference for Intractable Models"
permalink: /research/intractable-models/
author_profile: true
---

## About

Give examples of intractable models and explain why they pose a problem for modern statistical machine learning

The term *intractable model* is a general term encompassing all models for which the corresponding likelihood function is not available. 

There are many different types of intractability. A first example includes *intractable generative models* or *simulator-based models*, which are models for which nothing is known about the likelihood function, but it is possible to simulate new data given a fixed value of the parameters. A second example are  *unnormalised models*, in which case the likelihood function can be evaluated, but only up to some unknown normalisation constant. For each class of intractable model, alternative approaches need to be developed for parameter estimation.


## Contributions to this field

My work in this area is focussed on developping methodology which can balance several desirable properties. First, our algorithms should be robust in the sense that mild model misspecification or a few outliers should not have a disproportionate impact. Second, the algorithm should be efficient in the sense that we obtain estimates which are as accurate as possible given the finite amount of data available. Finally, the algorithms should be scalable and computationally efficient in the sense that they should be able to deal with large datasets or high-dimensional problems.

For generative models, the maximum mean discrepancy:

* ***Briol, F-X.***, Barp, A., Duncan, A. B., Girolami, M. (2019). *Statistical inference for generative models with maximum mean discrepancy*. arXiv:1906.05944. [(***Preprint***)](https://arxiv.org/abs/1906.05944) [(***Talk/Video***)](https://youtu.be/mm7bHjEzhow)

For unnormalised models, a convenient choice of distance are the so-called [Stein discrepancies](https://fxbriol.github.io/research/Stein/), which I have used to obtain flexible families of frequentist statistical estimators or generalised Bayesian inference approaches.

* Barp, A., ***Briol, F-X.***, Duncan, A. B., Girolami, M., Mackey, L. (2019). *Minimum Stein discrepancy estimators*. Neural Information Processing Systems, 12964-12976. [(***Conference***)](https://papers.nips.cc/paper/9457-minimum-stein-discrepancy-estimators) [(***Preprint***)](https://arxiv.org/abs/1906.08283) [(***Talk/Video***)](https://slideslive.com/38917866/minimun-stein-discrepancy-estimators)


* Mastubara, T., Knoblauch, J., ***Briol, F-X.***, Oates, C. J. (2021). *Robust generalised Bayesian inference for intractable likelihoods*. arXiv:2104.07359. [(***Preprint***)](https://arxiv.org/abs/2104.07359) [(***Code***)](https://github.com/takuomatsubara/KSD-Bayes)


<p align="center">
  <img src="/images/protein-signalling-network.png" alt="Robust Bayesian Estimation of Protein Signalling Networks" width="60%">
</p>

<br>

As part of my work in the Data-Centric Engineering programme of The Alan Turing Institute, I have also worked in specialising some of the methods above to solve important engineering problems, and in particular in the field of telecommunications.

* Bharti, A., ***Briol, F-X.***, Pedersen, T. (2020). *A general method for calibrating stochastic radio channel models with kernels*. arXiv:2012.09612. Accepted for publication in IEEE Transactions on Antennas and Propagation. [(***Preprint***)](https://arxiv.org/abs/2012.09612) 


<p align="center">
  <img src="/images/stochastic-radio-channels.png" alt="Intractable Models in Telecommunications" width="70%">
</p>

<br>
