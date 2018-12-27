"What I cannot create, I do not understand." - Richard Feynman.

# Akkordeon: Training a neural net with Akka

This project shows how to train a neural net with Akka.

The mechanics are as follows:

Every layer is an actor. 
The results of the forward and backward pass are passed as messages from one layer to another.
Calculations inside a layer are performed asynchronously from other layers.
Thus, a layer does not have to wait for the backward pass in order to perform the forward pass of the next batch.










[Actor model of a neural network](https://towardsdatascience.com/akkordeon-actor-model-of-a-neural-network-ff748096a5a3)

