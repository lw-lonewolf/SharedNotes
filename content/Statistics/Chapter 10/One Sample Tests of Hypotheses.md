 ## Statistical Hypotheses 
A *statistical hypothesis* is an assertion or conjecture concerning one or more populations. 

Rejection of a hypothesis implies that the sample evidence refutes it i.e. rejection means (for sure) that there is a very small possibility to obtain the sample information observed where the hypothesis is true. **IN ORDER TO REACH A CERTAIN CONCLUSION ABOUT SOMETHING, YOU MUST REACH A REJECTION OF A HYPOTHESIS.** *i.e. in order to prove that cancer and coffee consumption are  related. You must reject 'there is no increase in cancer risk produced by drinking coffee' instead.* 

Example: 
	`H0: defendant is innocent,
	`H1: defendant is guilty.
	
`The indictment comes because of suspicion of guilt. The hypothesis H0 (the status quo) stands in opposition to H1 and is maintained unless H1 is supported by evidence “beyond a reasonable doubt.” However, “failure to reject H0” in this case does not imply innocence, but merely that the evidence was insufficient to convict. So the jury does not necessarily accept H0 but fails to reject H0.`

### Alternative Hypothesis 
The study or claim that is to proved. Normally denoted by $R_{1}$
### Null Hypothesis
The null hypothesis $H_{0}$ *nullifies* or *opposes* the Alternative Hypothesis *$R_{1}$*


# Type I Error
*Rejection of the null hypothesis when it is actually true is called a type I error*
$$\text{Probability of Type I error} = \alpha = P(\text{type 1 error}) = P(\text{x > a when p = p}) = \sum_{x=a+1}^{n}b\left( x:20, p \right)$$
This probability is also known as 
# Type 2 Error
*Not rejecting the null hypothesis when it is actually false is a type II error*
$$\text{Probability of Type II error} = \beta = P(\text{type II error}) = P(x \leq a \text{ when } p = y) = \sum_{x=0}^{a}b(x:20, y)$$

>[!warning] Reducing both types of errors 
>Both types of errors can be reduced by increasing the sample size 


# Types of Tests
## One Tailed test
A test where the alternative ($H_{1}$) is one-sided is a one tailed test. 
e.g 
$$H_{0} : \theta = \theta_{0} \text{ and } H_{1} : \theta > \theta_{0}$$
or
$$H_{0} : \theta = \theta_{0} \text{ and } H_{1} : \theta < \theta_{0}$$

the direction of '<' or '>' signifies what direction the critical section will be. 

## Two Tailed Test 
The alternative where the $H_{1}$ is two-sided. 
e.g. 
$$H_{0} : \theta = \theta_{0} \text{ and } H_{1} : \theta \neq \theta_{0}$$