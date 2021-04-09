# Dynamic Programming: Model-Based RL, Policy Iteration and Value Iteration
---
With full knowledge of the MDP(Markov Decision Process), we can train an agent to take optimal actions in the environment. The action space must be discrete for dynamic programming to work. This training is done using the Bellman Equations.

Policy Evaluation - Based on a given policy, an agent learns how much long term reward it will get from a state using a value function.

Policy Iteration - Policy Evaluation with a greedy policy, meaning the policy extracts out the action that will give the greatest value estimate for the next state. 1) The value function evaluates the policy, 2) The policy changes to act greedily to the new value function, 3) repeat.

Value Iteration - Uses the Bellman Optimality Equation to find the optimal value function (optimal meaning if the policy function were optimal, the value function would be correct for it). Then, the policy acts greedily and it is then optimal as well.

## Links
- [David Silver's RL Course Lecture 3 - Planning by Dynamic Programming](https://www.youtube.com/watch?v=Nd1-UUMVfz4&list=PLqYmG7hTraZBiG_XpjnPrSNw-1XQaM_gB&index=3)
- [Bellman Equation](https://towardsdatascience.com/the-bellman-equation-59258a0d3fa7)
- [Contraction Mapping (used for proving the algorithms converge to an optimal solution)](https://www.youtube.com/watch?v=_DynXugXksU)