## Challenge Answers

### Challenge 1: What is the difference between expected value and mean?

- The expected value refers to a probability distribution, it is a weighted average of all the possible values in the distribution multiplied by the probability of that value occurring. 
- The mean refers to observed values. If we run an experiment on a variable with the same probability distribution as before, we should obtain values within the same range, **but the ones that have low probability should show up less often**. 
- As we run the experiment a million more times, the arithmetic mean should become more and more like the expected value.

### Challenge 2: What is the "problem" in science with p-values?
- The way I see it, the problems lie with making **binary decisions** based on the comparison between a p-value and a threshold. This is specially true in biomedical sciences where is large variability between samples. Just because a p-value is below threshold does not mean that the null hypothesis is false and vice-versa. To better describe an experiment it should be given more importance to the entire range of the data and those around the 'point estimate'.