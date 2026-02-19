**Wiegers' Matrix** is a prioritization technique that evaluates requirements based on multiple dimensions: **benefit**, **penalty**, **cost**, and **risk**. These dimensions are assigned values and relative weights, and a formula is used to calculate the overall priority of each requirement. This method helps ensure that decision-making is semi-quantitative and balances value against cost and risk.

-> *STEP 1:* Assign value to each dimension
	`Relative Benifit`, `Relative Penalty`, `Relative Cost`, `Relative Risk`
-> *STEP 2:* Assign Relative Weights for Dimensions 

**Total Value:**
$$\text{total value} = \text{relative benifit * weightage for relative benifit + relative penalty * weightage}$$
**Value%:**
$$\text{value\%} = \frac{\text{total value}}{\sum \text{(total values)}} * 100$$
**Cost%:**
$$\text{cost\%} = \frac{\text{relative cost}}{\sum \text{(total costs)}} * 100$$
**Risk%:**
$$\text{risk\%} = \frac{\text{relative risk}}{\sum \text{(total risks)}} * 100$$
**Priority:**
$$\text{Priority} = \frac{\text{value\%}}{\text{(cost\% * cost weight) + (risk\% * risk weight)}}$$