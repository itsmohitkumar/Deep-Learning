# Deep Learning Fundamentals Quiz - Solutions

## Part 1: Basic Concepts

**1. What is the primary inspiration for Neural Networks?**
- **Answer:** The human brain
- *Explanation:* Neural networks mimic the interconnected structure of biological neurons.

**2. In an artificial neuron, what mathematical operation is applied to the inputs before adding the bias?**
- **Answer:** Multiplication by weights
- *Explanation:* inputs ($x$) are multiplied by weights ($w$) to determine importance: $\sum (w \cdot x) + b$.

**3. Which component of a biological neuron is comparable to the "Output" or "Axon" in an artificial neuron?**
- **Answer:** Axon
- *Explanation:* The axon transmits the signal to other neurons.

## Part 2: The Perceptron & Logic

**4. Why is a single-layer perceptron unable to solve the XOR problem?**
- **Answer:** It can only draw linear decision boundaries
- *Explanation:* XOR is not linearly separable; it requires a non-linear boundary (or two linear boundaries combined).

**5. For an AND gate perceptron with weights $w_1=1, w_2=1$, which threshold $t$ would work?**
- **Answer:** $t = 1.5$
- *Explanation:* 
    - (0,0) -> sum 0 < 1.5 (False)
    - (0,1) -> sum 1 < 1.5 (False)
    - (1,1) -> sum 2 > 1.5 (True)

**6. True or False: A Multi-Layer Perceptron (MLP) with hidden layers can solve non-linear problems like XOR.**
- **Answer:** True
- *Explanation:* Hidden layers allow the network to combine linear boundaries into complex non-linear shapes.

## Part 3: Activation Functions

**7. Why do we need activation functions in neural networks?**
- **Answer:** To introduce non-linearity so the network can learn complex patterns
- *Explanation:* Without them, a multi-layer net would just be a single linear transformation.

**8. Which activation function squashes inputs to a range between 0 and 1?**
- **Answer:** Sigmoid
- *Explanation:* $\sigma(x) = \frac{1}{1+e^{-x}}$. Tanh is -1 to 1. ReLU is 0 to infinity.

**9. Which activation function is defined as $f(x) = \max(0, x)$?**
- **Answer:** ReLU
- *Explanation:* Rectified Linear Unit.

## Part 4: Training & Backpropagation

**10. What is the role of the "Loss Function" (or Error Function) during training?**
- **Answer:** To measure how far the network's prediction is from the correct answer
- *Explanation:* Minimizing this value is the goal of training.

**11. What algorithm is used to communicate the error *backward* through the network to update weights?**
- **Answer:** Backpropagation
- *Explanation:* It propagates the gradient of the loss backwards from output to input.

**12. In the analogy of "Hiking down a mountain in fog," what does the "Gradient" represent?**
- **Answer:** The direction of steepest ascent (uphill)
- *Explanation:* So we step in the *negative* gradient direction to go downhill (minimize error).

**13. What happens if your Learning Rate is too high?**
- **Answer:** The model might overshoot the minimum and fail to converge
- *Explanation:* Steps are too big, bouncing around the valley.

## Part 5: Advanced Challenges & Techniques

**14. What is the "Vanishing Gradient" problem?**
- **Answer:** When gradients become too small in deep layers, causing slow or stopped learning
- *Explanation:* Common with Sigmoid/Tanh in deep nets; gradients multiply (<1) and vanish.

**15. What is "Overfitting"?**
- **Answer:** When the model learns the training data (and noise) too well but fails on new data
- *Explanation:* It effectively memorizes the examples instead of learning general rules.

**16. Which technique involves randomly turning off some neurons during training to prevent overfitting?**
- **Answer:** Dropout
- *Explanation:* Forces the network to learn robust features that don't rely on single neurons.

**17. Batch Normalization helps by:**
- **Answer:** Normalizing the inputs of each layer to stabilize training
- *Explanation:* It keeps activations in a stable range, allowing faster learning rates.

**18. What does "Momentum" help with in Gradient Descent?**
- **Answer:** Accelerating the descent in the right direction and dampening oscillations
- *Explanation:* Like a heavy ball rolling down a hill, it keeps going even over small bumps.
