# Monte Carlo Prediction and Control
Unlike Dynamic Programming, the Monte Carlo method does not have full knowledge of the MDP; rather, all it can do is given a policy, go through the ennvironment and receive a history of states, actions, and rewards.

In order to estimate the value function given a policy, the algorithm goes through many episodes in the environment, and averages out the total(sum) return per state.

From this estimation, the target policy acts greedily, and the process repeats.

<br>
A problem with Monte Carlo learning is that although it has no bias by taking the average of every total return the policy got from a state, it has high variance as the total return of one state is based on the remaining rewards of the episode starting at that state, which could be a long line of rewards. This means there could have been many possibilities for that line of rewards, hence the high variance.
