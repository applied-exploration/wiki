 Recurrent Neural Networks process sequentual data by feeding each element in the sequence one-at-a-time, as well as the resulting weights of the previous computation.
RNNs enable weight sharing "across time" by using [[Recursion]].

While feed-forward Deep [[Neural Networks]] also by nature have [[Recursion]] operations, the number of elements that can be processed are theoretically infinite with RNNs (although in practice, the gradients "vanish/explode", which prevents effective training of really long sequences in one go).

Also related to [[Convolution]].

Some RNN architectures (like LSTM, GRU) are designed emulate the working of a [[Memory]], and a computer's memory update / read / write operations, within a [[Neural Networks]].