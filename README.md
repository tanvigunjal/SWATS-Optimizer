# SWATS-Optimizer
SWATS optimizer (switching from Adam to SGD)

# Overview
Adaptive optimization methods like RMSprop, Adagrad or Adam generalizes poorly despite their superior training performance when compared to Stochastic gradient descent (SGD). Adaptive optimization methods perform well in the initial training stage but lack in performance in later stages due to unstable and non-uniform learning rate at the end of training. Hence, SGD generalizes beter when compared to adaptive methods.

Adam has fast initial progress and good performance with default hyper-parameters, and SGD has good generalization properties. SWATS from aaaaaaaaaaaa is a method proposed to automatically switch from Adam to SGD when a triggering condition is satisfied. The SGD learning rate and switchover point from adam to SGD are both learned as a part of training process. The projection of the Adam step on the gradient subspace are monitored and use its exponential average as an estimate for the SGD learning rate after the switchover. The switchover is triggered when no chnage in this monitored quantity is detected.

# Experiment


# Setup
* batch_size = 128
* epochs = 150
* initial learning rate = 0.01
* threshold to switch \epsilonE = 10^-5 (In the paper \epsilon = 10^-9)

# Results

# Conclusion 



