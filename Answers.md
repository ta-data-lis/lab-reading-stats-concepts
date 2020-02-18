<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Lab | Reading About Statistic Concepts

## Introduction

In the future, you will need to understand deep statistical concepts by reading technical articles. As a training for that, it is interesting to start from here. Also, as we have limited time, this is a way to have some self guided learning to understand everything better and have a wider knowledge.

This week you will find some questions here that you will need to answer by documentating yourself. So you will do a different PR for each question (you are meant to answer the questions in different days). Don't hesitate to write as many text as you need and push images if you need them.

Remember for this lab: there is a right answer. But there is no perfect way to explain it (except for in a mathematical way, but this is another story).

## Challenges

### Challenge 1: What is the difference between expected value and mean?

In the context of discrete random variables expected value is the probability-weighted average of all its possible values, i.e . the sum of each possible value multipied by it´s probability.

If it´s a continuous random variable it´s the integral of the variable times the  pdf over the whole range.

The mean is, by definition exactly that when we are discussing random variables, so the concepts are equivalent.


### Challenge 2: What is the "problem" in science with p-values?

They are used erroneously many times, with the result the of the test being considered as a binary assumption of
success or insuccess. These analysis fail to take into account the true nature of the P value testing Any analysis should always take into account the assumptions of the statistical study undertaken, the p value & confidence intervals and the level of significance defined. The rejecting/acceptance of the Null Hip has always
to be perceived as being done to the significance level defined and not as a deterministic written in stone
conclusion.

In essence, the problem is one of "stretching" sometimes for the benefit of a conclusion, sometimes for ignorance, the mathematical concepts underlying the analysis.


### Challenge 3: Applying testing to a specific case: A/B testing.
Goal  Find out if the new website vs. is producing a better response than the previous one.

Approach:
1.	Test the outcomes using two metrics: Average time spent on landing page & Conversion Rate (% of visits that end in a transaction).
2.	Split traffic between users, give access to the test version to a sample group versus the rest. Non 50-50 split can be considered due to commercial considerations, but that might impact the time to have statistical significant results (the more the skew, the more time).
3.	Do the A/B Testing on these groups during a given period, taking into account the statistical significance /confidence intervals for the samples taken (Z-test, Chi-Squared test).
4.	Analyse the results and validate/reject the Null Hip given the scenario that has been setup.
5.	After it has been considered that the conclusions are statistically robust, implement the new website for all users or send back to review by the design team if results are not satisfactory.
