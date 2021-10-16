Reinforcement learning is the training of machine learning models to make a sequence of decisions.
Closely related to [[Sequence Learning]], but with RL, the decisions need to be made uni-directionally, left-to-right.
Can be also thought of as [[Search]], as the agent is exploring the search space and trying to find an optimal path (which is a sequence of actions).

**Markov property**
Reinforcement Learning Environments usually satisfy the "Markov property", which means the environment doesn't have a memory, and all of its state is accessible to the agent. 
"The Markov property means that evolution of the Markov process in the future depends only on the present state and does not depend on past history. The Markov process does not remember the past if the present state is given." [Source](https://www.sciencedirect.com/topics/engineering/markov-property)
Arguably, we don't have good enough sensors about and information about a complex real-world envrionment, therefore it's hard to find real-world problems that can be described with the Markovian property.

**Does the Markov assumption ever hold up in reality?**
With RL, the Markov assumption would mean that the current state of the environment should never depend on its previous state. **But is that really desirable even in the most controlled environment?** For example, in chess, or poker, we’d want to take the previous actions taken into account, for example, the opponent’s reaction to a move taken by us, because it could hold information about its style of play.  
For an MDP, for us to have access to this, we’d need to make the past actions taken also part of the state, which would kind of defeat the essence of its Markov property?

**RL Architectures**

*Actor-Critic*
It's common to have one neural network predicting the action to be taken, and another to evaluate how good the predicted action is.
This is the same mechanism that Monte Carlo Tree Search also uses.