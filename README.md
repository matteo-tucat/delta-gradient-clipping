# $\delta$-regularized Gradient Clipping Experiments

This repository contains experiment code used to test the $\delta$-gradient clipping ($\delta$-GClip) optimization algorithm in various neural network training scenarios.

In [our paper](https://arxiv.org/abs/2404.08624) we introduce $\\delta$-Gradient Clipping ($\\delta$-GClip) as the only known way to optimize neural networks using adaptive gradients with provable convergence guarantees on deep neural networks.

The optimization algorithm utilizes the following update step:
$$x_{t+1} = x_t - h(x_t) \cdot \nabla f (x_t), \text{    where } h(x_t) \coloneqq  \eta \cdot \min ( 1 , \max ( \delta, \frac{\gamma}{ || \nabla f (x_t) ||}   )  )$$
