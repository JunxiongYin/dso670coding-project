# DSO 670 Coding Project

This repo is for DSP 670 final coding project DSO 670. The code used for simulation is in sanity_check.Rmd.

In this coding project, I focused on the customized pricing problem as described in Section 5.1 of [Chen, Xi, et al. "A statistical learning approach to personalization in revenue management." Available at SSRN 2579462 (2015)](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2579462) and investigated the trade-offs of pooling data in personalized revenue management through numerical experiments.
I tested performance of three models of different levels of personalization: the model described in the paper, logit model with individual fixed effect and separate estimation for each customer, which can correspond to full data pooling, intermediate level of data pooling and no data pooling at all, respectively.

The results of the numerical experiments show that not too many observations for each customer are needed for no data pooling to outperform full data pooling.
This suggests that in practice, if we have enough data for each customer, then it would be better to learn each customer's choice behavior separately rather than do shared learning.
Besides, the results also suggest that when we do not have enough data for each customer, then learning more about each customer's features can be an alternative to differentiate customers and improve data pooling.