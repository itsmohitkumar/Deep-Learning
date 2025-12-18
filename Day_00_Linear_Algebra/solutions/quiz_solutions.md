# Day 0: Linear Algebra & NumPy Quiz - Solutions

## Part 1: Shapes & Dimensions

**1. What is the rank (number of dimensions) of a Vector?**
- **Answer:** 1
- *Explanation:* A vector is a 1D array. A scalar is 0, matrix is 2.

**2. If `A` has shape `(2, 3)` and `B` has shape `(3, 2)`, what is the shape of `np.dot(A, B)`?**
- **Answer:** `(2, 2)`
- *Explanation:* The inner dimensions (3) match and disappear. The outer dimensions (2 and 2) remain.

**3. What happens if you try `np.dot(A, A)` where A is `(2, 3)`?**
- **Answer:** Error: Dimension mismatch (`3 != 2`)
- *Explanation:* You cannot dot product `(2,3)` with `(2,3)`. The columns of the first (3) must match rows of the second (2).

**4. Which function allows you to swap the rows and columns of a matrix?**
- **Answer:** `.T` (Transpose)
- *Explanation:* `matrix.T` returns the transpose.

**5. How many elements are in a tensor of shape `(2, 3, 4)`?**
- **Answer:** 24
- *Explanation:* $2 \times 3 \times 4 = 24$.

## Part 2: Broadcasting

**6. Can you add a vector of shape `(3,)` to a matrix of shape `(5, 3)`?**
- **Answer:** Yes, broadcasting works (matches last dimension).
- *Explanation:* Shape `(3,)` is treated as `(1, 3)` and stretched to `(5, 3)`.

**7. Can you add a vector of shape `(5,)` to a matrix of shape `(5, 3)`?**
- **Answer:** No, broadcasting will fail.
- *Explanation:* The trailing dimensions (5 and 3) do not match and neither is 1.

**8. What is the result of `np.array([1, 2, 3]) * 2`?**
- **Answer:** `[2, 4, 6]`
- *Explanation:* Element-wise multiplication.

## Part 3: Terminology

**9. What is a "Scalar"?**
- **Answer:** A single number (0D tensor)

**10. What is a "Tensor" in the context of Deep Learning frameworks?**
- **Answer:** A multi-dimensional array generalization

**11. Which NumPy attribute gives you the tuple of dimensions (e.g., `(2, 3)`)?**
- **Answer:** `.shape`

**12. In the expression $W \cdot x + b$, if $W$ is $(10, 784)$ and $x$ is $(784,)$, what is the shape of $W \cdot x$?**
- **Answer:** $(10,)$
- *Explanation:* $(10, 784) \cdot (784,) \rightarrow (10,)$.

**13. What does `np.zeros((3,3))` create?**
- **Answer:** A 3x3 matrix filled with float 0.0

**14. If you have an image of size 28x28 pixels, what shape would the flattened vector be?**
- **Answer:** $(784,)$
- *Explanation:* $28 \times 28 = 784$.

**15. Why do we prefer Batches (e.g., shape `(32, 784)`) over single inputs?**
- **Answer:** It allows parallel computation (SIMD/GPU) for efficiency
