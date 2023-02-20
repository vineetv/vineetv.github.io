---
layout: post
title: Normalizing to a benchmark
subtitle: 
tags: [benchmarking, normalizing, statistics]
comments: true
---

One often needs to compare data across samples, say, when one or more samples
constitute a benchmark. For example, consider comparing interview scores
across panels when one of the panels is considered to be the benchmark.

The objective is to transform the data of a sample $$\{Y\}$$ so as to match its
mean $$(\mu_Y)$$ and standard deviation $$(\sigma_Y)$$ to that of the benchmark
sample. That is, we begin with:

$$\begin{aligned} \mathbb{E}[Y] &= \mu_Y\\ \mathbb{E}[\big(Y - \mu\big)^2] &=
\sigma_Y^2 \end{aligned}$$

and we need to transform data $$\{Y\}$$ as $$\{Z = cY + d\}$$ such that $$\mu_Z
= \mu_B$$ and $$\sigma_Z^2 = \sigma_B^2.$$ where $$\mu_B$$ and $$\sigma_B$$
respectively represent the mean and standard deviation of the benchmark sample.

The [method of
moments](https://en.wikipedia.org/wiki/Method_of_moments_(statistics)){:target="_blank"}
approach in statistics consists of finding parameters $$c$$ and $$d$$ such that:

$$\begin{aligned} \mathbb{E}[cY + d] &= \mu_B \\ \Rightarrow c^2 \mu_Y^2 + d^2 +
2cd\mu_Y &= \mu_B^2 \\ \mathbb{E}[\big((cY + d) - \mu_B \big)^2] &= \sigma_B^2
\end{aligned}$$

Simplifying the third equation, and after a bit a algebra, we get:

$$\begin{aligned} c &= \frac{\sigma_B}{\sigma_Y} \\ d &= \mu_B - c\mathbb{E}[Y]
=\mu_B - c\mu_Y \\ &= \mu_B - \dfrac{\sigma_B}{\sigma_Y}\mu_Y\end{aligned}$$

Plugging the finding back into $$Z = cY + d$$ tells us that transforming $$Y$$
as

$$Z = \dfrac{\sigma_B}{\sigma_Y}(Y - \mu_Y) + \mu_B$$

ensures that $$Z$$ has the same mean and standard deviation as the benchmark
data. Needless to say that this will work best for situations where the
underlying data can be safely assumed to be coming from the Normal distribution
or any of its
[kin](http://en.wikipedia.org/wiki/Elliptical_distribution){:target="_blank"}
(why?).

Looking at the transformation, upon a moment's reflection it almost appears
obvious, doesn't it? To the point that this whole post seems moot. So, why
bother? Well, while this is a simple enough example, the method of moments is
important enough in economics and finance for its [generalized
version](http://en.wikipedia.org/wiki/Generalized_method_of_moments){:target="_blank"}
to be granted the [Nobel
prize](http://www.nobelprize.org/nobel_prizes/economic-sciences/laureates/2013/hansen-facts.html){:target="_blank"}
a couple of years ago.
