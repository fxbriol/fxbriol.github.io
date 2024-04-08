---
permalink: /compstat2024
title: ""
excerpt: "Computational Statistics Theme Day"
redirect_from: 
---

# Computational Statistics Theme Day

The "Computational Statistics Theme Day" is a whole-day internal event for the members of the Computational Statistics theme at UCL Statistical Science. The aim of the event is to get everyone together to discuss exciting research directions in the department.

**When/where:** The event will take place on **Tuesday 23rd April* in *room 102 at 1-19 Torrington Place**.

### Schedule

*09:00-09:30* - Welcome \
*09:30-10:30* -	Talk by Petros Dellaportas \
*10:00-10:30* -	Talk by Sam Livingstone 

*10:30-11:00*	- Break

*11:00-11:30* - Talk by Giampiero Marra \
*11:30-12:30*	- Talk by Karla Ordaz \
*12:00-12:30* -  Talk by Alex Beskos 

*12:30-13:30* - Lunch break \
*13:30-14:30*	- Poster session 

*14:30-15:00*	- Talk by Ioanna Manolopoulou \
*15:00-15:30*	- Talk by F-X Briol 

*15:30-16:00*	- Break 

*16:00-17:00*	- Talk by Jeremias Knoblauch \
*16:30-17:00*	- Talk by Javier Rubio 

*17:00-onwards* - Pub trip at [TCR](https://bartcr.com). (Table reserved under F-X Briol).

### Titles and abstracts

*Speaker:* **Petros Dellaportas**\
*Title:*  Can independent Metropolis beat crude Monte Carlo? \
Abstract: Assume that we would like to estimate the expected value of a function $F$ with respect to a density $\pi$.  We prove that if $\pi$ is close enough under KL divergence to another density $q$, an independent Metropolis sampler estimator that obtains samples from $\pi$ with proposal density $q$, enriched with a variance reduction computational strategy based on control variates, achieves smaller asymptotic variance than that of the crude Monte Carlo estimator. The control variates construction requires no extra computational effort but assumes that the expected value of $F$ under $q$ is analytically available. We illustrate this  result by calculating the marginal likelihood in a linear regression model with  prior-likelihood conflict and a non-conjugate prior. Furthermore, we propose an adaptive independent Metropolis algorithm that adapts the proposal density such that its KL divergence with the target is being reduced. We demonstrate its applicability in a Bayesian logistic and Gaussian process regression problems and we rigorously justify our asymptotic arguments under  easily verifiable and essentially minimal conditions.

*Speaker:* Sam Livingstone \
*Title:* Bayesian variable selection: random neighbourhood samplers and large p asymptotics \
*Abstract:* Choosing which variables to include in a probabilistic model is a classical problem. The Bayesian solution is to place a prior distribution on a model with each possible combination of the p variables under consideration. This leads to a posterior over 2^p possible models. To decide on the best model or average over them for e.g. prediction, this model space must be explored, which can be difficult when p is large. Recently sophisticated Markov chain Monte Carlo (MCMC) algorithms have been proposed for this purpose. Some rely on intelligent global approximations to the posterior, while others consider sophisticated moves within a neighbourhood of the current model. I will argue that in the latter case the choice of neighbourhood is crucial to performance and scalability, and that ideas from the former case can help design such a neighbourhood, leading to algorithms that combine many recently proposed approaches to produce practical and scalable methodology for variable selection. I will then discuss more recent work on convergence of algorithms in the large p regime. Joint work with Xitong Liang and Jim Griffin.

Speaker: Giampiero Marra \
Title: Estimating the causal effect of a binary treatment on a survival outcome via a distributional regression spline model \
Abstract: TBC

Speaker: Karla Ordaz \
Title: TBC \
Abstract: TBC \

Speaker: Alex Beskos \
Title: Posterior Computation for Gaussian Graphical Models \
Abstract:  Gaussian graphical models can capture complex dependency structures among variables. For such models, Bayesian inference is attractive as it provides principled ways to incorporate prior information and to quantify uncertainty through the posterior distribution. However, posterior computation under the conjugate G-Wishart prior distribution on the precision matrix is expensive for general non-decomposable graphs. We therefore propose a new Markov chain Monte Carlo (MCMC) method named the "G-Wishart weighted proposal algorithm" (WWA). WWA’s distinctive features include delayed acceptance MCMC, Gibbs updates for the precision matrix and an informed proposal distribution on the graph space that enables embarrassingly parallel computations. Compared to existing approaches, WWA reduces the frequency of the relatively expensive sampling from the G-Wishart distribution. This results in faster MCMC convergence, improved MCMC mixing and reduced computing time. Numerical studies on simulated and real data show that WWA provides a more efficient tool for posterior inference than competing state-of-the-art MCMC algorithms. 

Speaker: Ioanna Manolopoulou \
Title: Sampling distributions and partial identifiability in Bayesian modelling \
Abstract: In this talk I'll give an overview of one stream of my research over the past decade and into the future. I will briefly cover 3 separate but connected works. The first concerns modelling binary data which have been observed with inhomogeneous (and unknown) label noise. The second relates to observing a point process through an non-uniform (and unknown) observation model. The third is in causal inference of heterogeneous treatment effects, where the treatment allocation process is unknown. All these models share a important aspect: they are only partially identifiable. Typical Bayesian solutions  address this be resolving the identifiability issue through a prior distribution. However, these prior distributions are not always transparent in their knock-on effects on posterior distributions of parameters, and may artificially shrink posterior uncertainty. More recently, modular and semi-modular priors have been proposed in the literature to alleviate these issues. I'd like to explore how heterogeneous noise models are connected to adaptive semi-modular models, and how these techniques can be used most effectively within partially identified models. 




