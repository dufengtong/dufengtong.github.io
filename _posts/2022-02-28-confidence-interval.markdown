---
layout: post
title: "Confidence interval"
date: 2022-02-28 23:02:50 -0000
categories: Statistics
---

# Confidence interval

## Distribution of sample mean
<pre xml:lang="latex">X_1, X_2, … X_n</pre> are random variables(RVs) from distributions with the same mean $\mu$ and std $\sigma$.
The average of those RVs is $\bar X$.
$$
\bar X = \frac{X_1 + X_2+ … +X_n}{n}
$$
Then, 
$$ E(\bar X) = \mu $$
$$ SD(\bar X) = \sigma / \sqrt n $$ 
Normally, we can also call $\bar X$ sample mean, and call $\mu$ the population mean.

If n is a large number or Xs are drawn from the same normal distribution, 
$$\bar X \sim Normal(\mu,  \sigma / \sqrt n )$$

## How close is $\bar X$ to $\mu$?
In practice, we draw a large number of samples from distribution with mean $\mu$ and std $\sigma$, and calcualte sample mean $\bar X$ and sample std $\sigma_{\bar X}$. How good it is to use $\bar X$ to estimate population mean $\mu$?

We can measure it by how far  $\bar X$ is to $\mu$ by ultilizing the standard normal distribution.


In standard normal distribution, $$P(|X|<1.96)=95\%$$
And $$\bar X \sim Normal(\mu,  \sigma / \sqrt n )$$
Transform $\bar X$ into standard normal distribution 
$$P(\frac{|\bar X -\mu|}{\sigma / \sqrt n } < 1.96) = 95\% $$
Finally, we get
$$P(\bar X-\frac{1.96\sigma}{\sqrt n}<\mu<\bar X+\frac{1.96\sigma}{\sqrt n}) = 95\%$$
Now we have an estimation of a range of population mean and it's probability.

