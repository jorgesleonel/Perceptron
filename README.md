# Perceptron
Perceptron code in Python with comments

Perceptrons and artificial neurons actually date back to 1958. Frank Rosenblatt was a psychologist trying to solidify a mathematical model for biological neurons. To better understand the motivation behind the perceptron, we need a superficial understanding of the structure of biological neurons in our brains.

In the biological neuron, the point of this cell is to take in some input (in the form of electrical signals in our brains), do some processing, and produce some output (also an electrical signal). Inputs and outputs are binary (0 or 1). An individual neuron accepts inputs, usually from other neurons, through its dendrites.The dendrites connect with other neurons through a the synapse — that assigns a weight to a particular input. Then, all of these inputs are considered together when they are processed in the cell body (soma).

Neurons exhibit an all-or-nothing behavior :

* if the combination of inputs exceeds a certain threshold, then an output signal is produced (the neuron “fires”)
In this case, output travels along the axon to the axon terminals. These are connected to the dendrites of other neurons through the synapse.
* if the combination falls short of the threshold, then the neuron doesn’t produce any outpu (“doesn’t fire”).

The Perceptron neuron model has:
* n binary inputs (usually given as a vector) and
* exactly the same number of weights

We multiply and sum them up. Result is z , also called pre-activation.
There is another term, called the bias (a constant factor).

After taking the weighted sum, we apply an activation function to this and produce an activation a.

. if the input is greater than or equal to 0, then we produce an output of 1.
. If input is lower than 0, we produce an output of 0.

This is the mathematical model for a single neuron — most fundamental unit for a neural network.

In comparison with the bio neuron:
→ The inputs are analogous to the dendrites,
→ the weights model the synapse.
→ Combine the weighted inputs by summing and send that weighted sum to the activation function. This acts as the response function where 0 means the neuron didn’t produce an output.
→ inputs and outputs are also binary, which is in accordance with the biological model.

Since the output of a perceptron is binary, we can use it for binary classification, i.e., an input belongs to only one of two classes. The classic examples used to explain what perceptrons can model are logic gates.

***

It’s important to note that perceptrons are limited to solving problems that are linearly separable, ie., where it's possible to draw a single line to separate the classes. This is because we’re creating a line (named “decision boundary”) and indicating that everything on one side of the line belongs to one class and everything on the other side belongs to the other class. Moreover, organizing multiple perceptrons into layers and using an intermediate layer (named “hidden layer”) allow for solution of non-linearly separable problems and is in fact the foundation of modern neural networks.
