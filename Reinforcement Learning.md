Reinforcement learning is the training of machine learning models to make a sequence of decisions.
Closely related to [[Sequence Learning]], but with RL, the decisions need to be made uni-directionally, left-to-right.
Can be also thought of as [[Search]], as the agent is exploring the search space and trying to find an optimal path (which is a sequence of actions).

**Markov property**
Reinforcement Learning Environments usually satisfy the "Markov property", which means the environment doesn't have a memory, and all of its state is accessible to the agent. 
"The Markov property means that evolution of the Markov process in the future depends only on the present state and does not depend on past history. The Markov process does not remember the past if the present state is given." [Source](https://www.sciencedirect.com/topics/engineering/markov-property)
Arguably, we don't have good enough sensors about and information about a complex real-world envrionment, therefore it's hard to find real-world problems that can be described with the Markovian property.

