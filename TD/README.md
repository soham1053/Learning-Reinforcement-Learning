# Temporal Difference Model-Free Prediction & Control
---
TD Learning is a value prediction method that rather than using total returns to learn its value estimate, uses a method called bootstraping. This means that instead of finding the total return of one state by going all the way to the end of an episode, we only go a few steps forward(in this implementation, just one step forward) in the environment, and estimate the rest with the current value function. The policy updates in accordance to the value function through the epsilon-greedy strategy. This strategy makes a tradeoff between exploring the environment by taking random actions, and acting greedily to the value function by choosing the action with the highest value estimate.

## Bias-Variance Tradeoff
Unlike Monte Carlo Learning, TD Learning has low variance, meaning that TD Learning learns much more efficiently since Monte Carlo Learning would need to train on many more samples of the environment. However, TD Learning has a lot of bias at the start, and since the value function is a factor of its own update, bias can lead to a lot of unstability in the training. 

## Links
- [David Silver's RL Course Lecture 4 - Model-Free Prediction](https://www.youtube.com/watch?v=PnHCvfgC_ZA&list=PLqYmG7hTraZBiG_XpjnPrSNw-1XQaM_gB&index=4)
- [David Silver's RL Course Lecture 5 - Model-Free Control](https://www.youtube.com/watch?v=0g4j2k_Ggc4&list=PLqYmG7hTraZBiG_XpjnPrSNw-1XQaM_gB&index=5)
- [Sarsa vs. Q-Learning](https://www.cse.unsw.edu.au/~cs9417ml/RL1/algorithms.html)