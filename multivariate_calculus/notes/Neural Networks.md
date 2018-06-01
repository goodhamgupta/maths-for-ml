# Neural Networks

- Takes a variable in and gives a variable out as output
- Both these variables could be VECTORS
- For the function given below

```flowchart
st=>start: a0
e=>end: a1
st->e
```
- Here, `a1` can be expressed as
$$a_1=\sigma(wa_0+b)$$
$$a \text{ terms => activities}$$
$$w \text{ => weights}$$
$$b \text{ => bias}$$
$$\sigma { => activation function}$$

- _activation function_ => It helps neural networks get their property of a brain
  - Once it receives inputs that pass a certain threshold value, the neuron gets activated. This starts simulating it's neighbours in turn
- Function with a characteristic _S_ shape are called sigmoids(hence the name _sigma_)
  - Tanh
  - Sigmoid

- Let's say we add an additional neuron to out input layer. Now the inputs are $a_0^{(0)}$ and $a_1^{(0)}$ and the output is $a^{1}$
- Hence, we get
$$a^{(1)} = \sigma(w_0a_0^{(0)}+w_1a_1^{(0)} + b)$$

- Therefore, for `n` inputs
$$\sigma \bigg(\sum_{i=0}^nw_ia_i^{(0)}\bigg)+b$$
$$=\sigma(\boldsymbol{w}.\boldsymbol{a}+b)$$

- When we add another output neuron, out outputs will be $a_0^{(1)}$ and $a_1^{(1)}$
- Hence, we get

$$a_0^{(1)} = \sigma(\boldsymbol{w}_0.\boldsymbol{a}+b_0)$$
$$a_1^{(1)} = \sigma(\boldsymbol{w}_1.\boldsymbol{a}+b_1)$$

- This can again be expressed using vector dot product
  - The outputs will each be a row of a column vector
  - Weight vectors will be in a weight matrix
  - Two biases in a bias vector
$$\boldsymbol{a}^{(1)} = \sigma(\boldsymbol{W}^{(1)}.\boldsymbol{a}^{(0)}+\boldsymbol{b}^{(1)})$$

- The neural network can have one or several layers of neurons between the input and the output layer. This layers are called HIDDEN LAYERS
$$\boldsymbol{a}^{(L)} = \sigma(\boldsymbol{W}^{(L)}.\boldsymbol{a}^{(L-1)}+\boldsymbol{b}^{(L)})$$


