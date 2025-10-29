# ee250-lab8

## Team Members
- Leyaa George
- Rida Faraz

## Questions
**Question 1: What are the denominations of the US coins from the green, blue, and orange distributions? Can you think why the coins from the same denomination might show variation in weight, although they are specified to be of the same weight? If your vending machine had a weight sensor, how would you use the weight of a coin that was just inserted to find the denomination?**

We can determine that the green, blue, and orange distributions are respectively pennies, nickels, and dollar coins based on the mean weight.
Even though each denomination represents the same coin, the variation in weight could be a result of wear over time. Things like corrosion or dirt accumulation could make slight but nonnegligible changes to the mass, which is represented by the normal curve revolving around each denomination. If our vending machine had a weight sensor, we would create a reasonable range of weights (in grams) that each coin could fall into and group the inserted coin into one of these ranges based on its measured weight. 

**Question 2. We can shine light on the coin and measure the reflected amount of light, which should be proportional (directly or in some non-linear way) to the size/area of the coin. Can you guess which sensor on the Grove Pi Kit can be used for this purpose?**

In order to measure the reflected light, we can use the light sensor that we used in our previous GrovePi lab. The light sensor is the most suitable sensor for measuring anything related to light and reflection. 

**Question 3: Which of the following datasets are linearly separable? Justify your answer.**

Dataset A and C are very clearly linearly separable, as there is a strong divide between data points in different classes. Dataset D can also be linearly separable, but it is not a very strong linear separation, as data samples from both class lie very close to the decision boundary. However, all three of these datasets can be separated with a linear decision boundary. Dataset B, E, and F are not linearly separable because there is no singular decision boundary that can completely separate both classes.

**Question 4. Sometimes we need more than a simple hyperplane to separate the datasets of the two classes. What are some other simple geometric entities other than a simple plane/line that can be used to separate some of the data points that were not linearly separable?**

Some alternatives to a linear decision boundary are circles or ellipses, parabolas or hyberbolas, and rational functions with horizontal, vertical, or slant asymptotes. For example, Dataset E can be separated by a rational function that has a slant asymptote ((x-h)(y-k)=c), and Dataset F can be separated by a circle or ellipse ((x-h)^2+(y-k)^2=r^2). 

**Question 5. For the example shown in the figure, what is approximately the output of the neuron? The bias is -2**

The output of the example neuron is 0.982.

Summation Node: (1 * 2) + (-2 * 1) + (3 * 2) - 2 = 4

Activation Node: 1/(1+e^(-4)) = 0.982.
