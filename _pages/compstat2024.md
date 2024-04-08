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
*11:30-12:30*	- Talk by Alex Beskos \
*12:00-12:30* - Talk by Karla Ordaz 

*12:30-13:30* - Lunch break \
*13:30-14:30*	- Poster session 

*14:30-15:00*	- Talk by Ioanna Manolopoulou \
*15:00-15:30*	- Talk by F-X Briol 

*15:30-16:00*	- Break 

*16:00-17:00*	- Talk by Jeremias Knoblauch \
*16:30-17:00*	- Talk by Javier Rubio 

*17:00-onwards* - Pub trip at [TCR](https://bartcr.com). (Table reserved under F-X Briol).

### Titles and abstracts

Speaker: Petros Dellaportas\
Title:  Can independent Metropolis beat crude Monte Carlo? \
Abstract: Assume that we would like to estimate the expected value of a function $F$ with respect to a density $\pi$.  We prove that if $\pi$ is close enough under KL divergence to another density $q$, an independent Metropolis sampler estimator that obtains samples from $\pi$ with proposal density $q$, enriched with a variance reduction computational strategy based on control variates, achieves smaller asymptotic variance than that of the crude Monte Carlo estimator. The control variates construction requires no extra computational effort but assumes that the expected value of $F$ under $q$ is analytically available. We illustrate this  result by calculating the marginal likelihood in a linear regression model with  prior-likelihood conflict and a non-conjugate prior. Furthermore, we propose an adaptive independent Metropolis algorithm that adapts the proposal density such that its KL divergence with the target is being reduced. We demonstrate its applicability in a Bayesian logistic and Gaussian process regression problems and we rigorously justify our asymptotic arguments under  easily verifiable and essentially minimal conditions.

Speaker: Sam Livingstone \
Title: Bayesian variable selection: random neighbourhood samplers and large p asymptotics \
Abstract: Choosing which variables to include in a probabilistic model is a classical problem. The Bayesian solution is to place a prior distribution on a model with each possible combination of the p variables under consideration. This leads to a posterior over 2^p possible models. To decide on the best model or average over them for e.g. prediction, this model space must be explored, which can be difficult when p is large. Recently sophisticated Markov chain Monte Carlo (MCMC) algorithms have been proposed for this purpose. Some rely on intelligent global approximations to the posterior, while others consider sophisticated moves within a neighbourhood of the current model. I will argue that in the latter case the choice of neighbourhood is crucial to performance and scalability, and that ideas from the former case can help design such a neighbourhood, leading to algorithms that combine many recently proposed approaches to produce practical and scalable methodology for variable selection. I will then discuss more recent work on convergence of algorithms in the large p regime. Joint work with Xitong Liang and Jim Griffin.

