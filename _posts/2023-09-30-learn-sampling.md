# How to sample from custom distribution 
Sampling: given a specified pdf (probability density function), i.e., the blue line in the figure below, define a processthat can generate numbers that form a histogram (orange bars in the figure) that agrees with the pdf.

![image](https://github.com/qiangt/skills-github-pages/assets/20675558/76fa711b-96c1-464f-bb0d-a024bfbb55c2)

## We need to generate some random numbers from known distributions
Normal distribution is widely used and we can assume it's given. I am sloppy here but you can find many materials covering this part, e.g., the first link I gave in the acknowledge section.
- sample a load of numbers from a known continuous probability distribution
- get the value of the cdf for all of these samples
- inverse the cdf 

# Acknowledge
- Many materias are borrowed from the blog wrote by Mark Jamison [https://towardsdatascience.com/random-sampling-using-scipy-and-numpy-part-i-f3ce8c78812e](https://towardsdatascience.com/random-sampling-using-scipy-and-numpy-part-i-f3ce8c78812e). I am not going as detailed as Mark but it's sufficient for my own understanding. However, it's strongly recommended to read his blog yourself. 
