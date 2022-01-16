# Assignment 1a: Implementing new distribution in D3 and contributing to Opensource
## Implementation details and workflow
I have made both pdf and cdf for chi-square distribution and have visaulised it through pachinko function for random values of x and Chart for continuous graph. 
First I wrote Gamma function which was computed using Lanczos approximation. As written in observable notebook itself Chi-square function uses Gamma function for computation. <br>
```math
SE = \frac{\sigma}{\sqrt{n}}
```
There is a way to define chi square function as:<br>
If Z is a standard normal random variable, the distribution of U =   is called the chi-square distribution with 1 degree of freedom.<br>
If U1, U2, . . . ,Un are independent chi-square random variables with 1 degree of freedom, the distribution of V = U1 + U2 + ・ ・ ・ + Un is called the chi-square distribution with n degrees of freedom. <br>
For chart, Samples were taken which are defined in the array named "data". Then a library was imported whose link is https://d3js.org/d3.v5.min.js.<br>
For pachinko, random values were generated using Math.random.
All the things about Chi-square are stated in Observable notebook.<br>
For better understanding I have also included an example based on the same distribution.<br>

The link for my observable notebook is : https://observablehq.com/d/828cb6afa0941dda
### Reference links
- https://observablehq.com/@dswalter/normal-distribution
- https://observablehq.com/@herbps10/gamma-distribution
