# Awesome Bias in Deep Learning [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
*Last updated on December 18, 2020.*  
<br>

## Introduction
This list aims to be a curate list focusing on the **systematic bias rooted in deep learning models**. To start with, we define bias as the error between the model prediction and the reality. In the later part of this list, we would give more accurate definitions for bias under different senarios.

On one hand, bias is long assumed to be a unavoidable property of learning models *in the presence of disparity between training and test set*. In the eyes of supporters of [The No Free Lunch Theorem](https://www.wikiwand.com/en/No_free_lunch_in_search_and_optimization), **bias means specialization**, as illustrated in figure 1. It implies that, without prior knowledge (*e.g.* a universal rule), it is impossible to make prediction for any unseen data<a href="#note1" id="note1ref"><sup>1</sup></a>; to make a model to work, we **have to incorporate a preference or bias** through model<a href="#note2" id="note2ref"><sup>2</sup></a> or dataset<a href="#note3" id="note3ref"><sup>3</sup></a> design, implicitly or explictly. In practice, we need to identify where the bias resides and what its effect is, which will be covered in [Causes](#Causes).

<p align="center">
  <img width="60%" src="https://github.com/ZIYU-DEEP/awesome-bias-in-deep-learning/blob/main/images/NFLT.jpeg">
</p>
<p align="center" style="font-size:6px;color:gray">
  Figure 1. Illustration of No Free Lunch Theorem. Adapted from Leon Fedden's <a href="https://medium.com/@LeonFedden/the-no-free-lunch-theorem-62ae2c3ed10c">post</a>.
</p>

However, there is hope. In theory, [The Free Lunch Theorem](https://machinethoughts.wordpress.com/2014/08/02/the-free-lunch-theorem/) or [Occam Guarantee](https://mcallester.github.io/ttic-31230/Fall2020/07regularization/PACBayes.pdf) claims *there exists some universal algorithm for learning neural networks that succeed in arbitrary domains* with limited training data. In practice, there exist numerous strategies in mitigating known bias from model or dataset design, which will be covered in [Solutions](#Solutions).

To sum up, this list will be organized as follow:  
- [Categories](#Categories): a short summary on different aspects or manifestation of bias in deep learning.
- [Causes](#Causes): theories, conjectures or evidence on the root causes of the bias.  
- [Solutions](#Solutions): practical solutions or mitigating strategies for the bias.

## Categories
*To be continued...* (Topics include dataset bias, exposure bias, expressivity bias, social bias, negative transfer, bias in catastrophic forgetting, bias in anomaly detection, bias in constrastive learning.)

## Causes
*To be continued...*

## Solutions
### Model-Driven Solutions
*To be continued...*
(A typical example is in negative transfer / catastrophic forgetting problems, in order to maintain the performance of an updated model with an unbiased model, people usually use the strategy of **fine-tuning** or **co-training**.)
### Data-Driven Solutions
*To be continued...*
(When the bias is known (on a seen specific class), typical strategies include **memory bufferring**, **up-sampling / downsampling**. But when the bias is on unseen data, the strategies are limited. )
    
     
     
    
<br>
<a id="note1" href="#note1ref"><sup>1</sup></a> More precisely speaking, there exists a algorithm or function in theory with low error on unseen data from the population, but such a function must be structureless thus we are not able to learn.

<a id="note2" href="#note2ref"><sup>2</sup></a> An example would be the choice of optimization, like SGD will always leads to the minimum norm solution for linear models. <br>
<a id="note3" href="#note3ref"><sup>3</sup></a> For instance, by introducing additional labeled data in training, anomaly detection models can become more discriminative on certain types of anomalies.

