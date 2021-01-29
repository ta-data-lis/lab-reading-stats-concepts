## Challenges
### Challenge 1: What is the difference between expected value and mean?

The average value is a statistical generalization of multiple occurrences of an event. This is a result of an experiment, given a number of observations.

The expected value refers to a single event that will happen in the future. This is a result from each outcome multiplied by the probability of that outcome. The expected value is numerically the same as the average value, but it is a prediction for a specific future occurrence rather than a generalization across multiple occurrences.

### Challenge 2: What is the "problem" in science with p-values?

The p-value is used in hypothesis testing to determine whether to accept or reject the null hypothesis. It is the smallest level of significance where the null hypothesis can be rejected.

The p-value reflects the strength of the evidence against the null hypothesis. A smaller p-value means that there is stronger evidence in favor of the alternative hypothesis. 

Aparently, there could be a lack of understanding of p values and what they imply.

Taken the information from 
https://www.khanacademy.org/math/ap-statistics/tests-significance-ap/idea-significance-tests/a/p-value-conclusions 
https://scientificallysound.org/2016/03/31/the-limitations-of-p-values/
https://www.nature.com/news/statisticians-issue-warning-over-misuse-of-p-values-1.19503?WT.mc_id=FBK_NatureNews
I can conclude that the issues with p-value follows this reasoning:

    1. P values do not measure the probability that the studied hypothesis is true
    
    2. It is said that if P value is greater than or equal to the significance level, then we fail to reject the null hypothesis H0, but this doesn't mean we accept H0.
    
    3. A p value, or statistical significance, does not measure the size of an effect or the importance of a result.
    
    4. "... p values is they do not indicate how worthwhile or how precise the effect is... Providing information on effect size and precision (i.e., 95% CI) forces the reader to consider whether the effect observed is big enough, sufficiently precise, and important enough to be worth caring about. This kind of statistics is known as estimation."

    5. The misinterpretation or misunderstanding of what p value means seems to be the issue, for the sake of science.
    
### Challenge 3: Applying testing to a specific case: A/B testing.

I'm going to part from this:

    "If you don’t capture a member’s attention within 90 seconds, that member will likely lose interest and move onto another activity. Such failed sessions could at times be because we did not show the right content or because we did show the right content but did not provide sufficient evidence as to why our member should watch it."
    
I'm not a Netflix member since a long time, but I have experienced this in Netflix and Youtube: by trying to match something they think you would like to watch, they "encapsulate" you in a "pattern", offering you the same similar "kinds" everytime, and exploring the "universe" tends to be harder. Somehow you start forgetting that there is more outside your four walls. 

So, I would try this test: Something that works with a more random algorithm. A buttom like "Bored? Discover more!", and then it brings you random movies, series, documentaries, that you don't know yet but that you might be interested in watching.
