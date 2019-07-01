# Complex function discovery with deep learning

## The Problem

Deep learning can help feature learning. After all, back propagation is about finding out the optimal weights for features. A lot of real world models have various number of features, from a few to the millions. A deeper network or a bigger number of neurons in each layers are used to dealt with complex models. There are things to pay attention to, such as, vanishing and exploding gradients, learning rate decay, batching, optimizations and tuning the hyperparameters.

## The Experiment

This project is to work on a labeled dataset of physics data, to classify if a sample is particle data or background noise. The dataset had been worked on and a 5-layer 100-feature each layer network had been used. I am wondering if there is a different deep learning approach to it, it will be a good exercise to explore and find out.

## The Data

I will be using the [HIGGS](https://archive.ics.uci.edu/ml/datasets/HIGGS) or [SUSY](https://archive.ics.uci.edu/ml/datasets/SUSY) data from the UCI machine learning repository, which has 11 millions and 5 millions samples respectively.

```
label, lepton 1 pT, lepton 1 eta, lepton 1 phi, lepton 2 pT, lepton 2 eta, lepton 2 phi, missing energy magnitude, missing energy phi, MET_rel, axial MET, M_R, M_TR_2, R, MT2, S_R, M_Delta_R, dPhi_r_b, cos(theta_r1)
0.000000000000000000e+00,9.728614687919616699e-01,6.538545489311218262e-01,1.176224589347839355e+00,1.157156467437744141e+00,-1.739873170852661133e+00,-8.743090629577636719e-01,5.677649974822998047e-01,-1.750000417232513428e-01,8.100607395172119141e-01,-2.525521218776702881e-01,1.921887040138244629e+00,8.896374106407165527e-01,4.107718467712402344e-01,1.145620822906494141e+00,1.932632088661193848e+00,9.944640994071960449e-01,1.367815494537353516e+00,4.071449860930442810e-02
```

## The Resource

Domino or AWS with GPU. Details will come later.

## References:
- [Searching for Exotic Particles in High-energy Physics with Deep Learning](https://arxiv.org/pdf/1402.4735.pdf)