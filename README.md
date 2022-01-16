# Assignment 1a: Implementing new distribution in D3 and contributing to Opensource
## Implementation details and workflow
I have made both pdf and cdf for chi-square distribution and have visaulised it through pachinko function for random values of x and Chart for continuous graph with values of x defined in an array having 8000 values of in range[0,20]. 
First I wrote Gamma function which was computed using Lanczos approximation. As written in observable notebook itself Chi-square function uses Gamma function for computation.<br>
![Chi-square pdf function](https://math.info/image/32/chi-sqaure_pdf.gif)<br><br>
There is a way to define chi square function as:<br>
If Z is a standard normal random variable, the distribution of U =  is called the chi-square distribution with 1 degree of freedom.<br>
If U1, U2, . . . ,Un are independent chi-square random variables with 1 degree of freedom, the distribution of V = U1 + U2 + ・ ・ ・ + Un is called the chi-square distribution with n degrees of freedom. <br>
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQCYWMp3ikBKN8juzmVF3vrBmviSdABYgsSgw&usqp=CAU)<br>
For chart, Samples were taken which are defined in the array named "data". Then a library was imported whose link is https://d3js.org/d3.v5.min.js.<br>
For pachinko, random values were generated using Math.random.
All the things about Chi-square are stated in Observable notebook.<br>
For better understanding I have also included an example based on the same distribution.<br>
### Comparing Pachinko and Chart 
- **Degree of freedom = 2**
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.25.02%20AM.png)<br>
The link for my observable notebook is : https://observablehq.com/d/828cb6afa0941dda
### Reference links
- https://observablehq.com/@dswalter/normal-distribution
- https://observablehq.com/@herbps10/gamma-distribution
