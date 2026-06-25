---
title: "Transfer Learning for Monte Carlo"
permalink: /research/multiple-integrals/
author_profile: true
---

## The problem

Estimating integrals or expectations through simulation is one of the key challenges in computational statistics and machine learning. Indeed, many quantities of interest including posterior moments, model evidences, tail probabilities and marginal likelihoods take the form of intractable integrals, and we hence need algorithms to obtain accurate estimates. One of the key challenges is the cost (either computational or financial) of obtaining integrand evaluations. When working with complex models, this cost can be very large, which limits the number of integrand evaluations available and can lead to poor accuracy of the resulting algorithms. In order to obtain highly accurate estimates of these integrals, it is therefore necessary to make use of any mathematical structure or additional information available.

There are of course many different types of additional information you could attempt to encode in your algorithms, but one key element which is often neglected is that we rarely have to compute a single isolated integral. Indeed, many practical problems will require you to compute several related integrals either simultaneously or sequentially. For example, in Bayesian statistics you usually have to compute some posterior expectation of interest, but you will also often want to calculate similar posterior expectations if you collect more data or want to try out different priors. Similarly, when working with mathematical models of physical or biological phenomenon, you will often have access to models of varying accuracy and may want to calculate integrals for each of these. In cases where the various integration problems are similar enough, it may be worth designing algorithms which can share integrand evaluations across tasks in order to improve accuracy.

<p align="center">
  <img src="/images/BQ-illumination.png" alt="Application of Bayesian Quadrature to Global Illumination" width="80%">
</p>

<br>

## Contributions to this field

My main contribution to answering this problem has been a series of papers which propose to use transfer learning for computing integrals. Transfer learning is a general paradigm in machine learning where algorithms are designed to transfer information across related tasks, and hence improve accuracy. There is a wide range of applications of transfer learning including for regression and classification, but there is surprisingly little in the context of numerical integration. 


* Xi, X., ***Briol, F-X.*** & Girolami, M. (2018). *Bayesian quadrature for multiple related integrals*. International Conference on Machine Learning, PMLR 80:5369-5378. [(***Conference***)](http://proceedings.mlr.press/v80/xi18a.html) [(***Preprint***)](https://arxiv.org/abs/1801.04153)

* Sun, Z., Barp, A. & ***Briol, F-X.*** (2023). *Vector-valued control variates*. Proceedings of the 40th International Conference on Machine Learning, PMLR 202:32819-32846. [(***Conference***)](https://proceedings.mlr.press/v202/sun23a.html) [(***Preprint***)](https://arxiv.org/abs/2109.08944) [(***Code***)](https://github.com/jz-fun/Vector-valued-Control-Variates-Code)
	* This paper received a *Student Paper Award* from the section on Bayesian Statistical Science of the American Statistical Association in 2022.
	* Zhuo Sun was awarded a Silver Medal for his poster on this paper at the 2021 Fry conference at Bristol.

* Li, K., Giles, D., Karvonen, T., Guillas, S. & ***Briol, F-X.*** (2023). *Multilevel Bayesian quadrature*. Proceedings of The 26th International Conference on Artificial Intelligence and Statistics, PMLR 206:1845-1868. [(***Conference***)](https://proceedings.mlr.press/v206/li23a.html) [(***Preprint***)](https://arxiv.org/abs/2210.08329) [(***Code***)](https://github.com/CeciliaKaiyu/MLBQ)
	* This paper was accepted for an oral presentation (top 6% of accepted papers) at AISTATS.

* Sun, Z., Oates, C. J. & ***Briol, F-X.*** (2023). *Meta-learning control variates: variance reduction with limited data*. Proceedings of the Thirty-Ninth Conference on Uncertainty in Artificial Intelligence, PMLR 216:2047-2057. [(***Conference***)](https://proceedings.mlr.press/v216/sun23a.html) [(***Preprint***)](https://arxiv.org/abs/2303.04756) [(***Code***)](https://github.com/jz-fun/Meta_Control_Variates)
	* This paper was accepted for oral presentation at UAI.

* Chen, Z., Naslydnik, M., Gretton, A. & ***Briol, F-X.*** (2024). *Conditional Bayesian quadrature*. Uncertainty in Artificial Intelligence, PMLR 244:648-684. [(***Conference***)](https://proceedings.mlr.press/v244/chen24b.html) [(***Preprint***)](https://arxiv.org/abs/2406.16530) [(***Code***)](https://github.com/hudsonchen/CBQ) [(***Slides***)](https://fxbriol.github.io/pdfs/slides-CBQ.pdf)

* Chen, Z., Naslidnyk, M. & ***Briol, F-X.*** (2025). *Nested expectations with kernel quadrature*. Proceedings of the 42nd International Conference on Machine Learning, PMLR 267:8760-8793. [(***Conference***)](https://proceedings.mlr.press/v267/chen25av.html) [(***Preprint***)](https://arxiv.org/abs/2502.18284) [(***Code***)](https://github.com/hudsonchen/nest_kq) [(***Slides***)](https://fxbriol.github.io/pdfs/slides-NKQ.pdf)


## Funding

* **Amazon Research Award** for a project entitled *"Transfer Learning for Numerical Integration in Expensive Machine Learning Systems"*. See the following [Amazon announcement](https://www.amazon.science/blog/recipients-of-the-2019-amazon-research-awards-announced) and [UCL press release](https://www.ucl.ac.uk/mathematical-physical-sciences/news/2020/jul/ucl-statistical-science-lecturer-receives-2019-amazon-research-award) for more details.
* **EPSRC New Investigator Award** grant [(EP/Y022300/1)](https://gow.epsrc.ukri.org/NGBOViewGrant.aspx?GrantRef=EP/Y022300/1) on *"Transfer Learning for Monte Carlo Methods"*.


<div style="position:relative;padding-bottom:56.25%;height:0;overflow:hidden;max-width:100%;">
  <iframe
      src="https://www.youtube.com/embed/WeiP2LCANdw"
      style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;"
      title="YouTube video"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen>
  </iframe>
</div>
