---
layout: post
title: Sample Variance Decay in Randomly Initialized ReLU Networks
description: This is a description of the first postThis is a description of the first postThis is a description of the first postThis is a description of the first post
featured-image: /assets/images/sample_variance_overview.png
---
Background
	Initialization important
Key idea: Variance preservation
Sample Variance
	Look at the fixed
Quick Fix
Gradients
Batch Normalization
Training
Other Activation Functions
Related Work

It's hard to understate the impact of weight initialization on the trainability of a deep neural network, especially if you are not using techniques like Batch Normazliation. Forgetting a factor of 2 from the initial distribution's variance can render a modestly sized network untrainable \cite{kaiming}.  


### Weight Initialization Principle from the 90's

Unlike many areas of deep learning, we actually have some useful theory to guide us, dating back to at least the 90's.  The principle can be stated:

> **Variance Preservation Principle:**  Sample the weights to preserve the variance.


This was popularized by Glorot and Kaiming. Even today, current work extending.

Example with reLU

There is an oddity though, in actual network use, we sample a single fixed network, and propagate samples from the training set.
You might wonder if there is some large n, argue they should be one in the same. We argue below that this isn't true.

### The Sample Variance is Different from the Total Variance
We'll call the sample variance. Here well just give the intuition and

### Quick Fix

### Gradients

### Batch Normalization Preserves Sample Variances


#### Now What: How to Initialize your networks?
Well it's easy to implement this idea
We think its important conceptually though.
