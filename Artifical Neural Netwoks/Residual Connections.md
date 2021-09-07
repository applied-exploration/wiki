Also known as "skip connection" or a short cut.
![[Residual-connections.png]]
Connecting two layers that are "out of order", making it possible for a layer to be "discarded", if it's not "useful".
Because of normalization, the weights of the intermediary layer are always gonna be scaled down, and therefore it's easy to learn the "identitify function" (the intermediary layer containing zeros), if the layer is not useful during the learning process.
This makes it possible to train deeper ANN architectures, as it also helps with the vanishing gradient problem.

**Modularity**
It's a primitive step to make the ANN somewhat modular, as it can reduce the number of layers "in actual use".
[[Modularity in Neural Networks]]