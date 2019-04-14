# Lecture 2: Supervised Learning of Behaviors

2019.04.14

## Terminology & notation

$\pi_\theta(a_t|o_t)$

Differences between state and observation.

## Imitation Learning

Learning from a stabilizing controller. Augmenting data by 3 cameras.


### DAgger: Dataset Aggregation

Goal: collect training data from $p_\pi_\theta(o_t)$ instead of $p_{data}(o_t)$.

Run $\pi_\theta(a_t|o_t)$!

Problem: Ask human to label $D_\pi$ with action $a_t$.


### Fail to fit

1. Non-Markovian behavior: depends on all past observations, often very unnatural for human demonstrators.
   
   Use the whole history: RNN state(LSTM).

2. Multimodal behavior: 
   
* Output mixture of Gaussians
* Latten (潜在的) variable models
* Autoregressive discretiazation

