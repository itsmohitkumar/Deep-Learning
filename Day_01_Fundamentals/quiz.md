# Deep Learning Fundamentals Quiz

**Instructions:** Answer the following questions based on the lecture material.

## Part 1: Basic Concepts (Definitions)

**1. What is the primary inspiration for Neural Networks?**
- [ ] A computer processor
- [ ] The human brain
- [ ] a decision tree
- [ ] A plumbing system

**2. In an artificial neuron, what mathematical operation is applied to the inputs before adding the bias?**
- [ ] Division by weights
- [ ] Subtraction of weights
- [ ] Multiplication by weights
- [ ] Squaring the weights

**3. Which component of a biological neuron is comparable to the "Output" or "Axon" in an artificial neuron?**
- [ ] Dendrite
- [ ] Soma (Cell Body)
- [ ] Synapse
- [ ] Axon

## Part 2: The Perceptron & Logic

**4. Why is a single-layer perceptron unable to solve the XOR problem?**
- [ ] It cannot have negative weights
- [ ] It can only draw linear decision boundaries
- [ ] It does not have enough inputs
- [ ] The activation function is too slow

**5. For an AND gate perceptron with weights $w_1=1, w_2=1$, which threshold $t$ would work?**
- [ ] $t = 0.5$
- [ ] $t = 1.5$
- [ ] $t = 2.5$
- [ ] $t = -0.5$

**6. True or False: A Multi-Layer Perceptron (MLP) with hidden layers can solve non-linear problems like XOR.**
- [ ] True
- [ ] False

## Part 3: Activation Functions

**7. Why do we need activation functions in neural networks?**
- [ ] To make the math easier
- [ ] To introduce non-linearity so the network can learn complex patterns
- [ ] To ensure outputs are always positive
- [ ] To clear the memory

**8. Which activation function squashes inputs to a range between 0 and 1?**
- [ ] ReLU
- [ ] Tanh
- [ ] Sigmoid
- [ ] Linear

**9. Which activation function is defined as $f(x) = \max(0, x)$?**
- [ ] Sigmoid
- [ ] Tanh
- [ ] ReLU
- [ ] Softmax

## Part 4: Training & Backpropagation

**10. What is the role of the "Loss Function" (or Error Function) during training?**
- [ ] To increase the speed of the network
- [ ] To measure how far the network's prediction is from the correct answer
- [ ] To initialize the weights
- [ ] To choose the activation function

**11. What algorithm is used to communicate the error *backward* through the network to update weights?**
- [ ] Forward Propagation
- [ ] K-Means Clustering
- [ ] Backpropagation
- [ ] Binary Search

**12. In the analogy of "Hiking down a mountain in fog," what does the "Gradient" represent?**
- [ ] The altitude
- [ ] The direction of steepest ascent (uphill)
- [ ] The destination
- [ ] The weather

**13. What happens if your Learning Rate is too high?**
- [ ] The model trains very slowly
- [ ] The model might overshoot the minimum and fail to converge
- [ ] The model will definitely find the global minimum
- [ ] The gradient becomes zero

## Part 5: Advanced Challenges & Techniques

**14. What is the "Vanishing Gradient" problem?**
- [ ] When the training data disappears
- [ ] When gradients become too small in deep layers, causing slow or stopped learning
- [ ] When the weights become zero
- [ ] When the output layer disappears

**15. What is "Overfitting"?**
- [ ] When the model assumes the data fits on one screen
- [ ] When the model learns the training data (and noise) too well but fails on new data
- [ ] When the learning rate is too low
- [ ] When the network has too many layers

**16. Which technique involves randomly turning off some neurons during training to prevent overfitting?**
- [ ] Batch Normalization
- [ ] Gradient Descent
- [ ] Dropout
- [ ] Momentum

**17. Batch Normalization helps by:**
- [ ] Normalizing the inputs of each layer to stabilize training
- [ ] Removing bad data points
- [ ] Increasing the batch size
- [ ] normalizing the final output between 0 and 1 only

**18. What does "Momentum" help with in Gradient Descent?**
- [ ] Stopping the descent immediately
- [ ] Accelerating the descent in the right direction and dampening oscillations
- [ ] Removing the need for a learning rate
- [ ] Ignoring the gradient completely
