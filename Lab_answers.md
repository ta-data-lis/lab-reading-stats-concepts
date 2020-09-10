## Challenges

### Challenge 1: What is the difference between expected value and mean?

The mean is total sum of observations, divided by the total number of observations, as simple as that.
In other hand, the expected value is the average value we expect to get when we repeat an experiment a lot of times.

### Challenge 2: What is the "problem" in science with p-values?

There are two problems in my opinion: the first one is that the p-value is misinterpretated a lot of times, for example, let's see this 
example: url = https://blog.minitab.com/blog/adventures-in-statistics-2/how-to-correctly-interpret-p-values

For example, suppose that a vaccine study produced a P value of 0.04. This P value indicates that if the vaccine had no effect, you’d obtain the observed difference or more in 4% of studies due to random sampling error. The correct way to interpretate this is:

Correct: Assuming that the vaccine had no effect, you’d obtain the observed difference or more in 4% of studies due to random sampling error.
 
Incorrect: If you reject the null hypothesis, there’s a 4% chance that you’re making a mistake.

The second problem is that, it is generally expected that a study should have a P < 0.05 as way to avoid considering 'statistically non-significant' outliers, that threshold can lead scientists to disregard data to keep within the P < 0.05, without considering whether the data is significant or not.

### Challenge 3: Applying testing to a specific case: A/B testing.

I chose the netflix article. On this article they try to demonstrate if changing the art of a picture they were able to increase the active time of the subscribers. I think that it would also be interesting to test different regions, and to point the main characteristics of the art with bigger results. 