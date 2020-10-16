---
layout: category
title: Projects
---
<br/>

<!-- ### Prevalence of negation in negative reviews  -->
<!-- Performed lexical analysis on negative and positive reviews of various datasets and found that negative reviews have more negations than positive reviews. Analyzed its implications on downstream NLP tasks such as sentiment analysis, style transfer in text. Check out the source code [here](https://github.com/Negation-in-negative-review) -->

### Style Transfer on Tweets
This project was the result of my independent study with Prof. Chenhao Tan during Spring 2020. I replicated [Style Transfer from Non-Parallel Text by Cross-Alignment](https://papers.nips.cc/paper/7259-style-transfer-from-non-parallel-text-by-cross-alignment.pdf) paper by Shen et. al., and implemented this technique on non-parallel twitter data. The task here was to see whether we could efficiently translate an input tweet to a better worded tweet with the same content, so that the translated tweet may have a higher chance of getting retweeted. It was a great learning experience for me as I got to know a lot about style transfer in text, which is what I am working on now. Check out the Github repository [here](https://github.com/madhu-aithal/language-style-transfer-pytorch).


<!-- Implemented Cross-alignment style transfer technique for twitter data to translate an input tweet to a better worded tweet with the same content. The output tweet may have a higher chance of getting retweeted. [Source code]() -->


### Clipboard Synchronization Application
I worked on developing an application for synchronizing the clipboard data across multiple devices of a user. The idea here is to provide a simple solution for users to copy a text such as a website URL, between their devices without much hassle. If a user copies a text in one of their devices, it will be available in the clipboard of other devices. We used [electron.js](https://www.electronjs.org/) and Angular for developing the cross-platform desktop application, Node.js and MongoDB as our backend with [Keycloak](https://www.keycloak.org/) for Identity and Access Management. We made use of sockets for synchronizing texts between multiple devices. We deployed our applications and services on Google Cloud Platform. Checkout the source code [here](https://github.com/OOAD-Semester-Project).

### Event Sequence Prediction
<!-- Implemented an LSTM based model for event sequence prediction on Twitter and Hawkes data. Analyzed its performance (NLL Loss) in comparison with the Neural Hawkes model.  -->

Several events happen during our everyday life. In this project, we studied the pattern of such events. With a solid understanding of how events happen we can use it in many different application such as medical treatment, purchase prediction, and behavior study. We implemented an LSTM based sequence model for predicting such events on Twitter (rewteet events) and Hawkes data. We conducted an experiment and compared the [Neural Hawkes model](http://papers.nips.cc/paper/7252-the-neural-hawkes-process-a-neurally-self-modulating-multivariate-point-process.pdf) with our LSTM to see if the inclusion of the time difference directly influencing the hidden layers have any positive effect to predict future events. You can check out the source code for our LSTM model [here](https://github.com/CSCI-5922-DL-project).

<!-- Studying event sequence has a long history starting from the Poisson Process, while being a very strong analytical tool it has a flaw in that it assumes that every event is independent with each other. The Hawkes Process tries to overcome this drawback but still has a problem that events influence each other only in a positive way and their influences are independent with other influences. We suggest that a neural network can solve this problem by giving the machine free parameters to find the inherit causality of events. For the experiment we compared the CT-LSTM\cite{Mei2017TheNH} with the normal LSTM to see if the inclusion of the time difference directly influencing the hidden layers have any positive effect to predict future events. -->


### non-normal Recurrent Neural Networks
<!-- Performed hyperparameter explorations and ablation studies of nnRNNs. Implemented the Adding task for measuring the performance of nnRNNs against other RNN architectures. [Github repository]() -->


Recurrent neural networks (RNNs) have been proven to suffer from Exploding and Vanishing Gradient Problem (EVGP). In the recent years, a class of RNNs known as [Orthogonal RNNs](https://arxiv.org/pdf/1504.00941.pdf) have been developed which addresses this issue. The expressivity of orthogonal RNNs is limited because it spans only a subset of all transformations with unit norm eigen spectra. Non-normal Recurrent Neural Networks ([nnRNN](https://papers.nips.cc/paper/9513-non-normal-recurrent-neural-network-nnrnn-learning-long-time-dependencies-while-improving-expressivity-with-transient-dynamics.pdf)) solves this problem by relaxing the constraint on the orthogonal eigen basis. This allows to parameterize matrices with unit-norm eigenspectra without orthogonality constraints on eigenbasis, thereby providing better expressivity. In this project, we performed hyperparameter explorations and ablation studies of nnRNNs. We also implemented the Adding task to measure whether nnRNNs perform better against other RNN architectures. Check out the Github repository of our project [here](https://github.com/madhu-aithal/nnRNN_release).

<!-- . Orthogonal RNNs restrict the recurrent connectivity matrices to have unit norm eigen and singular spectra, thus ensuring that the signals (or gradients) can be propagated over long timescales. The expressivity of orthogonal RNNs is limited because it spans only a subset of all transformations with unit norm eigen spectra. Non-normal Recurrent Neural Networks (nnRNN) \cite{kerg2019non} solves this problem by relaxing the constraint on the orthogonal eigen basis. This allows to parameterize matrices with unit-norm eigenspectra without orthogonality constraints on eigenbasis. Thus nnRNN provides better expressivity with similar stable dynamics and training as Orthogonal RNNs.  -->