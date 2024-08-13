---
title: "Bayesian Robustness"
permalink: /research/bayesian-robustness/
author_profile: true
---

## The problem

In statistics and machine learning, we typically develop probabilistic models which represent real-world phenomena. These models are at best mathematical idealisations and are therefore limited by our understanding of the world. They will also inevitably contain approximations such as omitted variables, incorrect functional forms, or incorrect distributional assumptions. This is a particular concern in safety critical applications, such as medical diagnosis, self-driving cars, or the criminal justice system, where model misspecification can have a severe impact. As a result, it is necessary to develop *robust* methods which can perform reasonably well when models are mildly misspecified.

Robustness is particularly important in Bayesian inference, since we would ultimately like to use Bayesian posterior distributions to represent our uncertainty about quantities of interest. But if the model is misspecified, not only will Bayesian methods return poor predictions, their posterior uncertainty will also become meaningless.

<p align="center">
  <img src="/images/robust-GP.png" alt="Robust Gaussian Process through Generalised Bayes" width="55%">
</p>


## Contributions to this field

* Dellaporta, C., Knoblauch, J., Damoulas, T. ***Briol. F-X.*** (2022). *Robust Bayesian inference for simulator-based models via the MMD posterior bootstrap*. Proceedings of The 25th International Conference on Artificial Intelligence and Statistics (AISTATS), PMLR 151:943-970. [(***Conference***)](https://proceedings.mlr.press/v151/dellaporta22a.html) [(***Preprint***)](https://arxiv.org/abs/2202.04744) [(***Code***)](https://github.com/haritadell/npl_mmd_project.git) [(***Video***)](https://youtu.be/h4yWC-01oqQ)
	* This paper received the [Best Paper Award](https://aistats.org/aistats2022/awards.html) at AISTATS 2022 (out of 1685 submissions and 492 accepted papers).
	* A preliminary version of the paper was accepted to the [NeurIPS 2021 workshop "Your Model is Wrong: 
Robustness and misspecification in probabilistic modeling"](https://sites.google.com/view/robustbayes-neurips21/home).
	* This paper was discussed on the blog of [Prof. Christian Robert](https://xianblog.wordpress.com/2022/06/03/nonparametric-abc-seminar/)

* Matsubara, T., Knoblauch, J., ***Briol, F-X.*** & Oates, C. J. (2022). *Robust generalised Bayesian inference for intractable likelihoods*. Journal of the Royal Statistical Society: Series B (Statistical Methodology), 84:3, 997– 1022. [(***Journal***)](https://rss.onlinelibrary.wiley.com/doi/10.1111/rssb.12500) [(***Preprint***)](https://arxiv.org/abs/2104.07359) [(***Code***)](https://github.com/takuomatsubara/KSD-Bayes) [(***Video***)](https://drive.google.com/file/d/1gs016iDfvDbO07GBglI5xtOB8bFmjbAH/view)
	* This paper received a *Student Paper Award* from the section on Bayesian Statistical Science of the American Statistical Association in 2022.
	* This paper received a *Best Student/Postdoc Contributed Paper Award* at ISBA 2021.
	* A preliminary version of the paper was accepted to the [NeurIPS 2021 workshop "Your Model is Wrong: 
Robustness and misspecification in probabilistic modeling"](https://sites.google.com/view/robustbayes-neurips21/home).

* Altamirano, M., ***Briol, F-X.*** & Knoblauch, J. (2023). *Robust and scalable Bayesian online changepoint detection*. Proceedings of the 40th International Conference on Machine Learning, PMLR 202:642-663. [(***Conference***)](https://proceedings.mlr.press/v202/altamirano23a.html) [(***Preprint***)](https://arxiv.org/abs/2302.04759) [(***Code***)](https://github.com/maltamiranomontero/DSM-bocd) [(***Video***)](https://www.youtube.com/watch?v=exhkRsqq6HA)

* Altamirano, M., ***Briol, F-X.*** & Knoblauch, J. (2024). *Robust and conjugate Gaussian process regression*. Proceedings of the 41st International Conference on Machine Learning, PMLR 235:1155-1185. [(***Conference***)](https://proceedings.mlr.press/v235/altamirano24a.html) [(***Preprint***)](https://arxiv.org/abs/2311.00463) [(***Code***)](https://github.com/maltamiranomontero/RCGP)
	* This paper was accepted as a spotlight paper (top 3.5% of submitted papers).

* Duran-Martin, G., Altamirano, M., Shestopaloff, A. Y., Sanchez-Betancourt, L., Knoblauch, J., Jones, M., ***Briol, F-X.*** & Murphy, K. (2024). *Outlier-robust Kalman filtering through generalised Bayes*. Proceedings of the 41st International Conference on Machine Learning, PMLR 235:12138-12171. [(***Conference***)](https://proceedings.mlr.press/v235/duran-martin24a.html) [(***Preprint***)](https://arxiv.org/abs/2405.05646) [(***Code***)](https://github.com/gerdm/weighted-likelihood-filter)

<p align="center">
  <img src="/images/wolf-IMQ.gif" alt="Robust Kalman Filter through Generalised Bayes" width="70%">
</p>



## Funding

* **EPSRC Small Grant in the Mathematical Sciences** grant [(EP/Y011805/1)](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/Y011805/1) on *"Robust Foundations for Bayesian Inference"*.

