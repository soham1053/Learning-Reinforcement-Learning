# Monte Carlo Model-Free Prediction & Control
---
Unlike Dynamic Programming, the Monte Carlo method does not have full knowledge of the MDP; rather, all it can do given a policy is go through the ennvironment and receive a history of states, actions, and rewards.

In order to estimate the value function given a policy, the algorithm goes through many episodes in the environment, and averages out the total(sum) return per state.

As the value function updates, the policy updates to be epsilon greedy to the value. This means the policy makes a tradeoff between exploring the environment by taking random actions, and acting greedily to the value function by choosing the action with the highest value estimate.

<br>
A problem with Monte Carlo learning is that although it has no bias by taking the average of every exact total return the policy got from a state, it has high variance as the total return of one state is based on the remaining rewards of the episode starting at that state, which could be a long line of rewards. This means there could have been many possibilities for that line of rewards, hence the high variance.

## Links
- [David Silver's RL Course Lecture 4 - Model-Free Prediction](https://www.youtube.com/watch?v=PnHCvfgC_ZA&list=PLqYmG7hTraZBiG_XpjnPrSNw-1XQaM_gB&index=4)
- [David Silver's RL Course Lecture 5 - Model-Free Control](https://www.youtube.com/watch?v=0g4j2k_Ggc4&list=PLqYmG7hTraZBiG_XpjnPrSNw-1XQaM_gB&index=5)