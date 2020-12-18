# Awesome Bias in Deep Learning [![Awesome](https://awesome.re/badge-flat2.svg)](https://awesome.re)
*Last updated on December 18, 2020.*  
<br>

## Introduction
This list aims to be a curate list focusing on the **systematic bias rooted in deep learning models**. To start with, we define bias as the error between the model prediction and the reality. In the later part of this list, we would give more accurate definitions for bias under different senarios.

On one hand, bias is long assumed to be a unavoidable property of learning models *in the presence of disparity between training and test set*. In the eyes of supporters of [No Free Lunch Theorem](https://www.wikiwand.com/en/No_free_lunch_in_search_and_optimization), **bias means specialization**, as illustrated in figure 1. It implies that, without prior knowledge (*e.g.* a universal rule), it is impossible to make prediction for any unseen data; to make a model to work, we have to incorporate a preference or bias through model<a href="#note1" id="note1ref"><sup>1</sup></a> or dataset<a href="#note2" id="note2ref"><sup>2</sup></a> design.

<p align="center">
  <img width="60%" src="https://github.com/ZIYU-DEEP/awesome-bias-in-deep-learning/blob/main/images/NFLT.jpeg">
</p>
<p align="center" style="font-size:6px;color:gray">
  Figure 1. Illustration of No Free Lunch Theorem. Adapted from Leon Fedden's <a href="https://medium.com/@LeonFedden/the-no-free-lunch-theorem-62ae2c3ed10c">post</a>.
</p>

The list is organized as follows:  
- [Categories](#Categories): a short summary on different aspects or manifestation of bias in deep learning.
- [Causes](#Causes): theories, conjectures or evidence on the root causes of the bias.  
- [Solutions](#Solutions): practical solutions or mitigating strategies for the bias.

## Categories
*To be continued...*

## Causes
*To be continued...*

## Solutions
*To be continued...*
    
     
     
    
   
<a id="note1" href="#note1ref"><sup>1</sup></a>An example would be the choice of optimization, like SGD will always leads to the minimum norm solution for linear models.
<a id="note2" href="#note2ref"><sup>2</sup></a>For instance, by introducing additional labeled data in training, anomaly detection models can become more discriminative on certain classes.

