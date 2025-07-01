# Random Variables and Distributions

* distributions
  - discrete (=countable)
  - continuous => probability density function, dx defines the probability!
  - the mean (barycenter)
  - the variance (natural scatter)

1. Uniform Distribution
* continuous support = np.random.uniform(low, high, shape)
* discrete support = np.random.randint(low, high, shape)
  - Cumulative density function = np.cumsum(U)

2. Binomial Distribution
* Probability of having a sequence of k tails and n - k heads
* omega = n!/(n-k)!
* k are indistinguishable
* nchoosek.ipynb
* bino = "two"
```python
q = 0.2
n = 10
K = np.random.bionomial(n, q, N)

labels, counts = np.unique(K, return_counts = True)
plt.bar(labels, counts, aligns = 'center', width = 0.1)
plt.gca().set_kticks(labels)
plt.title('N = ' + str(N))
```

3. Poisson Distribution
* Starting binomial distribution, rare events => q<<1
* rare events
* events are mutually independent
* events have no duration
* example
  - radioactive decay
  - single photon detection
  - lightning
  - mutation of a gene
  - receiving WhatsApp messages/SMS

4. Normal Distribution

5. Cenral Limit Throrem
