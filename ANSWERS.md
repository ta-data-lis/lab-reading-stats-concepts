### Challenge 1: What is the difference between expected value and mean?

It seems that both terms can be used interchangeably, and are functionally very similar, but we must be careful with what is being discussed, as they are often used in different contexts.

From what I've gathered, it looks like the 'mean' or 'average' is used when discussing samples in statistics to characterize a certain sample. The 'expected value', on the other hand, seems to be the average of all the outcomes of a certain experiment that was repeated many times.


### Challenge 2: What is the "problem" in science with p-values?

I believe we first should start with what is the p-value, in order to better understand the problem it may pose in science.

The texts below are excerpts of articles I found online, and that I think greatly help understand the p-value, its usefulness as well as its problems.

*A p-value is the probability of observing a test statistic as extreme as the data shows, given that the null hypothesis is true*. It does not, however, tell us what the probability of the hypothesis is given the data. Confusing these two is equivalent to mixing up “given that someone is Catholic, what is the probability that they are the Pope?” and “given that someone is the Pope, what is the probability that they are Catholic?”

I think that the example above helps to shed a light on what the p-value is, and how it may be very troublesome to get it mixed up.


# How are p-values useful?

P-values help us make a decision regarding the null hypothesis. A null hypothesis states that there is no difference between specified populations, and that any observed difference can be attributed to sampling or experimental error. 

A small p-value indicates that there is strong evidence against the null hypothesis, and indicates that you should reject this claim in favor of the alternative. The alternative hypothesis rivals the null, stating that the observations are the result of a real effect.


# Problems with p-values

While p-values can be very useful in statistics, they can also be manipulated. p-hacking (data dredging) and p-HARKing (hypothesis after results are known) are processes by which researchers collect or select data that make nonsignificant results become significant.

Influencing data to make it significant, or to draw a hypothesis after you already know the results, is just bad science. It is the responsibility of the scientific community to know what a truly significant p-value looks like, and more importantly, what it means.


The correct interpretation of a p-value is:
- Assuming that your null is true, a p-value quantifies the probability of seeing a data point at or beyond your current observation.

The best way to combat the fickle p-value is to increase the number of replicates that you do and see if your p-value jumps around or if it stays consistently low


# A little historic background at the origins of the p-value, in case someone wants to read it.

In 1925 British geneticist and statistician Ronald Fisher published a book called Statistical Methods for Research Workers. The title doesn’t scream “best seller,” but the book was a huge success and established Fisher as the father of modern statistics. In it, he tackles the problem of how researchers can apply statistical tests to numerical data to draw conclusions about what they have found and determine whether it is worth pursuing. He references a statistical test that summarizes the compatibility of data with a proposed model and produces a p value. Fisher suggests that researchers might consider a p value of 0.05 as a handy guide: “It is convenient to take this point as a limit in judging whether a deviation ought to be considered significant or not.” Pursue results with p values below that threshold, he advises, and do not spend time on results that fall above it. Thus was born the idea that a value of p less than 0.05 equates to what is known as statistical significance—a mathematical definition of “significant” results.

Sources:
- https://towardsdatascience.com/a-case-study-of-the-p-value-f0d708861334
- https://www.acsh.org/news/2018/06/29/problem-p-values-13130







