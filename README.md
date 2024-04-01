# $\delta$-regularized Gradient Clipping Experiments

This repository contains experiment code used for testing the $\delta$-gradient clipping ($\delta$-GClip) optimization algorithm in various neural network training scenarios.

The optimization algorithm utilizes the following update step:
$$x_{t+1} = x_t - h(x_t) \cdot \nabla f (x_t), \text{    where } h(x_t) \coloneqq  \eta \cdot \min ( 1 , \max ( \delta, \frac{\gamma}{ || \nabla f (x_t) ||}   )  )$$
