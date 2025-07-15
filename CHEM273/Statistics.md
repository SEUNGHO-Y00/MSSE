# Statistics for Data Science

1. Expectation, Variance, and Covariance

* mean^2 = e(x^2) - E(x)^2

* plotting two sets of random numbers x_1 and x_2
x1 = np.random.normal(0,2,(1000,))
x2 = np.random.normal(0,2,(1000,))

* x_1 and x_2 are unrealted and nutually independent -> featureless data cloud

* cov(x_1,x_2) = cov(x_2, x_1) = E(x_1x_2)-E(x_1)E(x_2)
  - [Covariance](https://blog.naver.com/sw4r/221025662499)
  - > Geometrical interpretation
  - > arithmetical interpretation
  - Same dependency, but different variance!
  - ranges from -1 to +1
  - -1: max anti correlation
  - +1: max correlation
  - sns.heatmap(data.corr(), cmap = "Blues")
 
* Correlation coefficient

2. Hypothesis Testing

1) Assume a likelihood function L as your model, aka null hypothesis H_0
2) take a datapoint x+0
3) calculate the probability P given L i. e. given H_0 is true, that x_0 has this value or a more extreme value
4) Accepting or rejecting H_0 based on P and the threshold alpha

* coveats:
  - the model L for H_0 has to be known
  - the p-value P(x >= X_0|H_0) does not tell if H_0 is true or not
  - the p-value P(x >= X_0|H_0) does not tell which hypothesis is more likely
  - the p-value just gives P(x >= X_0|H_0)
  - the threshold alpha for accepting/rejecting H_0 is arbitrary
  - we are aiming on disproving a hypothesis, by assuming it is true, without leading to a contradiction

* Z-test
* t-test
* ANalysis Of VAriance
* KS test
* ranking test

3. Confidence Intervals

* Two kinds of errors
  - Systematic errors: calibration, non-linearity of the detector
  - Statistical errors: limited precision, natural variance of the data => spread of the data around an average value
* Assumption: far from the detection limit and saturation
  - the spread follows approximately a normal distribution.
  - fitting a model to data points each with an error bar om_i.
* Error propagation
* Curve fitting
 
