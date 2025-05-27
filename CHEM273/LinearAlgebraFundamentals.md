# Linear Algebra Fundamentals

1. Array in Python (shapes)
* A = np.arange(0,5,1)
* A = np.range(0,5,1)
* A = np.zeros((1,5))
* Anew = A.reshape((1,5))

2. Vectors
* Vectors vs scalars
* Cartesian coordinates
* unit vectors
* dot product of two vectors

3. Matrices
* Matrices multiplication
  - v1 = np.array([1,5,0,-3])
  - v2 = np.array([3,-1,2,2])
  - np.dot(v1, v2)
  - np.outer(v1, v2)
  - v3 = v1.reshape((len(v1),1)) => column vectors
  - v4 = v2.reshape((1,len(v2))) => row vectors
  - np.dot(v1,v1)**0.5 => dot product
  - np.multiply(v1,v2)
* Identity Matrix => np.eye()
* Inverse Matrix => np.linalg.inv(M) / print(np.dot(M,M_1))
  - Machine epsilon
* Transpose Matrix => M.transpose()
* Symmetry Matrix
  - distance matrices

4. Lecture Exercise
* np.zeros()
* np.arange()
* np.tile() => Construct an array by repeating A the number of times given by reps.
* np.transpose()

5. Solving Linear Systems
* Gaussian elimination
* determinant of A, det(A)
