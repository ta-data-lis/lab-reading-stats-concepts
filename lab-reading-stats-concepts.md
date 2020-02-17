Challenge 1: What is the difference between expected value and mean?


Expected Value is used in case of Random Variables (or in other words Probability Distributions). Since, the average is defined as the sum of all the elements divided by the sum of their frequencies. But for the case of Probability distribution we can't describe a random variable in terms of its frequency beforehand, thus we use the probability instead. Conceptually, probability of an element is frequency of an event divided by size of sample space. Thus, the average in case of random variable can be given by sum of probabilities multiplied by its respective event (where p(x)*x is conceptually frequency of x divided by total frequency).

    Average on the other hand is used in case where we have the knowledge of frequencies of individual elements and total count of the elements, for example, in case of known data set or sample. We can simply use the fundamental definition of average to calculate it.

For instance in poker, you can have won on average 10 big blinds per 100 hands for a sample of x number of hands. However, your expected value won per 100 hands will be different (higher or lower than actual win/rate whether you've been unlucky or lucky). 

### Challenge 2: What is the "problem" in science with p-values?

it brings scientists to mistakenly assume that non-significance (high P value) means no effect. This can cause issues for instance in medical studies.

Challenge 3: Applying testing to a specific case: A/B testing.

Regarding the netflix example.I personnally dont like their recommendation system, I find it recommends a lot of movies I dislike. I would add a feature based on a famous rating website, like rotten tomatoes. And add the rotten tomatoes notation for movies that have a good notation on rotten tomatoes (both blockbuster movies and less known ones), making the rotten tomatoes logo apparent. Implementing this only for a small portion of the users, and see if it brings an increase in audience for the concerned movies.