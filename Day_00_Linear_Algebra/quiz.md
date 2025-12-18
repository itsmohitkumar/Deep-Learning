# Day 0: Linear Algebra & NumPy Quiz

**Instructions:** Answer the questions to test your understanding of NumPy shapes and broadcasting.

## Part 1: Shapes & Dimensions

**1. What is the rank (number of dimensions) of a Vector?**
- [ ] 0
- [ ] 1
- [ ] 2
- [ ] 3

**2. If `A` has shape `(2, 3)` and `B` has shape `(3, 2)`, what is the shape of `np.dot(A, B)`?**
- [ ] `(2, 2)`
- [ ] `(3, 3)`
- [ ] `(2, 3)`
- [ ] Error (Shapes do not align)

**3. What happens if you try `np.dot(A, A)` where A is `(2, 3)`?**
- [ ] Result is `(2, 2)`
- [ ] Result is `(3, 3)`
- [ ] Error: Dimension mismatch (`3 != 2`)
- [ ] It element-wise squares the matrix.

**4. Which function allows you to swap the rows and columns of a matrix?**
- [ ] `np.swap()`
- [ ] `np.reshape()`
- [ ] `.T` (Transpose)
- [ ] `np.invert()`

**5. How many elements are in a tensor of shape `(2, 3, 4)`?**
- [ ] 9
- [ ] 12
- [ ] 24
- [ ] 234

## Part 2: Broadcasting

**6. Can you add a vector of shape `(3,)` to a matrix of shape `(5, 3)`?**
- [ ] Yes, broadcasting works (matches last dimension).
- [ ] No, dimensions must match exactly.
- [ ] Yes, but only if the matrix is zeros.
- [ ] No, the vector must be `(5,)`.

**7. Can you add a vector of shape `(5,)` to a matrix of shape `(5, 3)`?**
- [ ] Yes, broadcasting works.
- [ ] No, broadcasting will fail (3 vs 5 mismatch at last dim, and missing leading dim).
- [ ] Yes, `numpy` automatically transposes it.
- [ ] Yes, if forced.

**8. What is the result of `np.array([1, 2, 3]) * 2`?**
- [ ] `[1, 2, 3, 1, 2, 3]`
- [ ] `[2, 4, 6]`
- [ ] `[2, 2, 2]`
- [ ] Error

## Part 3: Terminology

**9. What is a "Scalar"?**
- [ ] A 1D array
- [ ] A single number (0D tensor)
- [ ] A matrix with only 1 row
- [ ] A complex number

**10. What is a "Tensor" in the context of Deep Learning frameworks?**
- [ ] A type of neural network layer
- [ ] A multi-dimensional array generalization (scalar, vector, matrix, n-D array)
- [ ] A database table
- [ ] A graphics processing unit

**11. Which NumPy attribute gives you the tuple of dimensions (e.g., `(2, 3)`)?**
- [ ] `.size`
- [ ] `.length`
- [ ] `.shape`
- [ ] `.dim`

**12. In the expression $W \cdot x + b$, if $W$ is $(10, 784)$ and $x$ is $(784,)$, what is the shape of $W \cdot x$?**
- [ ] $(784,)$
- [ ] $(10,)$
- [ ] $(10, 784)$
- [ ] $(784, 10)$

**13. What does `np.zeros((3,3))` create?**
- [ ] An empty list
- [ ] A 3x3 matrix filled with integer 0
- [ ] A 3x3 matrix filled with float 0.0
- [ ] A vector of length 9

**14. If you have an image of size 28x28 pixels, what shape would the flattened vector be?**
- [ ] $(28,)$
- [ ] $(56,)$
- [ ] $(784,)$
- [ ] $(28, 28)$

**15. Why do we prefer Batches (e.g., shape `(32, 784)`) over single inputs?**
- [ ] It is slower but more accurate
- [ ] It takes less memory
- [ ] It allows parallel computation (SIMD/GPU) for efficiency
- [ ] It is required by Python syntax
