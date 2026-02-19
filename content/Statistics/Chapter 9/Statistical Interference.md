=### Point Estimate 
A *point estimate* of some population parameter $\theta$ is a single value of $\hat{\theta}$ of a statistic $\bar{\theta}$ For example, the value $\bar{x}$ of the statistic $\bar{X}$, computed from a sample size of $n$ is a point estimate of the population parameter $\mu$.
### Unbiased Estimator
A statistic $\hat{\theta}$ is said to be unbiased estimator of the parameter $\theta$ if $\mu_{\bar{\theta}} = E(\bar{\hat{\theta}}) = \theta$

>[!important] Efficient Estimator
>* If we consider all possible unbiased estimators of some parameter $\theta$, the one with the smallest variance is called the most efficient estimator of $\theta$.

>[!tip] Efficient Estimator for a Normal Distribution
>For normal populations, one can show that both $\bar{x}$ and $\tilde{x}$ would be unbiased estimators of the population mean $\mu$ but variance of $\bar{x}$ would be less than $\tilde{x}$ hence we use that as our efficient estimator 
>* $\bar{x}$ -> mean of the population sample 
>* $\tilde{x}$ -> median of the population sample
### Interval Estimates 
Even the most efficient unbiased estimator may not yield the population parameter exactly. There are many situations when it is better to calculate an interval within which we would expect to find the value of the parameter. i.e. $\hat{\theta_{L} < \theta < \hat{\theta_{U}}}$ . This is an *interval estimate.*

>[!important] Interpretation 
>As the sample size increases, $\sigma^2_{X} = \frac{\sigma^2}{n}$ decreases, and hence our estimate is more likely to be closer to the parameter $\mu$ resulting in a shorter interval. By the length of the estimate interval, we define the accuracy of the point estimate. 

### Interpretation of Interval Estimates
Formula: 
$$P(\hat{\Theta_{L} < \Theta < \Theta_{U}}) = 1 - \alpha$$
for $0< \alpha < 1$
The interval $\hat{\theta}_{L} < \theta < \hat{\theta}_{U}$ is known as the $100(1-\alpha)\%$ confidence interval, the fraction $1-\alpha$ is the confidence coefficient or the degree of confidence. and the interval endpoints are the lower and upper confidence limits. 
>[!important] Value of $\alpha$
>if $\alpha = 0.05$ we have a 95% confidence interval.
>What we want is a **higher** confidence value and a **smaller** confidence interval.

## Estimating the Mean ($\bar{X}$)
### Case 1: $\sigma$ is known 
The formulae are: 
* *Confidence Interval on $\mu$ when $\sigma^2$ is known:*
$$\bar{x}-z_\frac{\alpha}{2}\frac{\sigma}{\sqrt{ n }} < \mu < \bar{x}+z_{\frac{\alpha}{2}}\frac{\sigma}{\sqrt{ n }}$$
	(To get $\alpha$ -> 1-confidence interval (percentage/100). then find $\frac{\alpha}{2}$. Check against  table 3 to find z value. )
	0.05 -> 0.025

* *Finding $n$ for a certain confidence level*
$$n = \left( \frac{z_{\frac{\alpha}{2}} \sigma}{E}\right)^2$$
Found by putting $e = \frac{z_{\frac{\alpha}{2}} \sigma}{\sqrt{ n }}$
*One-sided Confidence Intervals:*
Upper Confidence Interval: $\bar{x}+z_\alpha\frac{\sigma}{\sqrt{ n }}$
Lower Confidence Interval : $\bar{x}-z_\alpha\frac{\sigma}{\sqrt{ n }}$

### Case 2: $\sigma$ is not known 
To deal with the case where $\sigma$ is not known. We convert a standard normal distribution to a t-distribution where S is sample standard deviation. 
i.e. $$T = \frac{\bar{X}-\mu}{\frac{S}{\sqrt{ n }}}$$
Now, 
$P\left( -t_{\frac{\alpha}{2}} < T < t_{\frac{\alpha}{2}}\right)  = 1-\alpha$

or 
$P\left( \bar{X}- t_{\frac{a}{2}}\frac{S}{\sqrt{ n }} < \mu < \bar{X} + t_{\frac{\alpha}{2}}{\frac{S}{\sqrt{ n }}} \right) = 1-\alpha$

If x̄ and s are the mean and standard deviation of a random sample from a normal population with unknown variance σ 2 , a 100(1 − α)% confidence interval for μ is:
$$\bar{x} - t_{\frac{\alpha}{2}}{\frac{s}{\sqrt{ n }} < \mu < \bar{x} + t_{\frac{\alpha}{2}}}{\frac{s}{\sqrt{ n }}}$$


## PREDICTION INTERVAL 
$$\bar{x} - z_{\frac{\alpha}{2}}\sigma \sqrt{ 1+\frac{1}{n} } < x_{0} < \bar{x} + z_{\frac{\alpha}{2}}\sigma \sqrt{ 1+\frac{1}{n} }$$
$\sigma$ unknown
$$\bar{x} - t_{\frac{\alpha}{2}}s \sqrt{ 1+\frac{1}{n} } < x_{0} < \bar{x} + t_{\frac{\alpha}{2}}s \sqrt{ 1+\frac{1}{n} }$$

### WHEN POPULATION SIZE N IS GIVEN z
This formula is used when N is known and `n covers more than 5% of N`: 

$$\text{Confidence Interval} =\bar{x}\pm t_{\frac{\alpha}{2}}\frac{s}{\sqrt{ n }}\left(\sqrt{ \frac{{N-n}}{N-1}} \right)$$