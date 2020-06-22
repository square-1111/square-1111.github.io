---
layout: post
title: "Day 035, Understanding Deep Learning Requires Rethinking Generalization"
comments: true
description: ""
keywords: "dummy content"
---


*This is a summary of Understanding Deep Learning Requires Rethinking Generalization paper which has been awarded for the best paper award at ICLR 2017. One of the best papers I have read so far, an eye-opener but quite verbose.*

Some models generalize better than others. But how do we distinguish between them? Answering this question would help us interpret the Artificial Neural Network (ANN) and help us create reliable and principled model architecture. Before we move further ahead, generalization error is the difference between training and testing error. 

The central idea of the paper was 
> Deep neural networks easily fit random labels.  

and   
> Explicit regularization may improve generalization performance, but is neither necessary nor by itself sufficient for controlling generalization error.

## Randomization Test  : Fitting Random Labels and Pixels
The paper explained the memorization capacity of the paper through randomizing labels and pixels. Authors trained several standard architectures with randomized labels. They found DNNs easily fit random labels. Moreso, the training error becomes zero, while the testing error is the same as any random chance. Furthering this they experimented with the pixels as well — shuffled pixels, random pixel, and gaussian noise. Surprisingly, stochastic gradient descent with unchanged hyperparameters can optimize weight to fit random labels perfectly. Adding to this astonishment, it was observed that as the noise in the image increases, the generalization error decreases.

## Explicit Regularization
Explicit regularization techniques like dropout, weight decay, data augmentation are the tools of deep learning. These techniques were tested on random labels. As expected, the results were better. But the point that labels were shuffled makes it difficult to comprehend. Not only this  but implicit regularizers like early stopping also contributed for the betterment of the model trained on shuffled class labels. But we can’t miss that regularizers don’t tamper the weights too much but make subtle changes to make weights more smooth.

This all boils down to explain that deep neural networks work on rote memory than on semantic understanding, making neural networks far less interpretable and reliable.




