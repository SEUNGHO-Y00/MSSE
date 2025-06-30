# Scientific Computing

1. introduction to numpy
* type: numpy array
* useful numpy coomand
  - np.arange()
  - np.zeros(())
  - np.eye()
  - np.tile([], reps = ())
* math vs numpy
  - Task: Calculating cosine from an array!

2. linear algebra with numpy
* np.dot(v1, v2) => 3,1 * 1,3 = 1
* np.outer(v1.v2) => 1,3 * 3,1 = 3,3
* Broadcasting describes how Numpy treats arrays with different shapes during arithmetic operations

3. avoiding loops
* np.zeros()
* np.arange()
* np.tile()
* np.transpose()
* Normal loop
* efficient loop
* no loop

4. random numbers
* uniform
  - continuous support
  - np.random.uniform(low, high, shape)
  - discrete support
  - np.random.randint(low, high, shape)
* binomial
  - flipping a coin n times
  - np.random.binomial(n, q, N)
* poissonian
  - rate of c WhatsUp messages/day
  - np.random.poisson(lam, N)
* normal(gaussian)
  - np.random.normal(mu, s, N)
