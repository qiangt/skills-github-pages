# How to sample from custom distribution 
Sampling: given a specified pdf (probability density function), i.e., the blue line in the figure below, define a processthat can generate numbers that form a histogram (orange bars in the figure) that agrees with the pdf.

![image from [1]](https://miro.medium.com/v2/format:webp/1*KSgUJJ3SbNyKNc3soNT7eA.png)

## We need to generate some random numbers from known distributions
Normal distribution is widely used and we can assume it's given. I am sloppy here but you can find many materials covering this part, e.g., the first link I gave in the acknowledge section.
- sample a load of numbers from a known continuous probability distribution
- get the value of the cdf for all of these samples
- inverse the cdf 

# Acknowledge
- [1] Many materias are borrowed from the blog wrote by Mark Jamison [https://towardsdatascience.com/random-sampling-using-scipy-and-numpy-part-i-f3ce8c78812e](https://towardsdatascience.com/random-sampling-using-scipy-and-numpy-part-i-f3ce8c78812e). I am not going as detailed as Mark but it's sufficient for my own understanding. However, it's strongly recommended to read his blog yourself. 
