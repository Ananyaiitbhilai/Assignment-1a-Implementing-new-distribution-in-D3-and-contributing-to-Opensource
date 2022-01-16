# Assignment 1a: Implementing new distribution in D3 and contributing to Opensource
## Implementation details and workflow
I have made both pdf and cdf for chi-square distribution and have visaulised it through pachinko function for random values of x and Chart for continuous graph with values of x defined in an array having 8000 values of in range[0,20]. 
First I wrote Gamma function which was computed using Lanczos approximation. As written in observable notebook itself Chi-square function uses Gamma function for computation.<br><br>
![](https://math.info/image/32/chi-sqaure_pdf.gif)<br><br>
There is a way to define chi square function as:<br>
If Z is a standard normal random variable, the distribution of U =  is called the chi-square distribution with 1 degree of freedom.<br>
If U1, U2, . . . ,Un are independent chi-square random variables with 1 degree of freedom, the distribution of V = U1 + U2 + ・ ・ ・ + Un is called the chi-square distribution with n degrees of freedom. <br><br>
![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQCYWMp3ikBKN8juzmVF3vrBmviSdABYgsSgw&usqp=CAU)<br><br>
                                                                                                                
For Chart, Samples were taken which are defined in the array named "domain". Then a library was imported whose link is https://d3js.org/d3.v5.min.js.<br>
For pachinko, random values were generated using Math.random.<br>
All the things about Chi-square are stated in Observable notebook.<br>
For better understanding I have also included an example based on the same distribution.<br>
In chi-square distribution when x=0 and degree of freedom = 1, the function goes to infinity hence the graph can't be plotted at that point.<br>
y is Chi-square function with parameter x and n, n is degree of freedom. <br>
This table is for degree of freedom=1
|Value of x|Value of y|
|-----|--------|
|0.0000000000001|1261566.2610100168|
|0.000000000001|398942.2804012331|
|0.00000000001|126156.62610037724|
|0.0000000001|39894.22803814855|
|0.000000001|12615.662603792965|
|0.00000001|3989.422784067213|
|0.0000001|1261.5661979317683|
|0.000001|398.94208093034234|
|0.00001|126.15599531945442|
|0.0001|39.8922333786082|
|0.001|12.609356355490782|
|0.01|3.969525474770117|
|0.1|1.2000389484301357|
|0.1390|0.9982037549037381|
|0.140|0.9941351606919718|

### Comparing Pachinko and Chart 
#### Degree of freedom= 1
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.33.22%20AM.png)<br>
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.32.16%20AM.png)<br>
#### Degree of freedom = 2
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.25.02%20AM.png)<br>
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.42.39%20AM.png)<br>
#### Degree of freedom = 3
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.28.17%20AM.png)<br>
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.42.53%20AM.png)<br>
#### Degree of freedom = 4
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.29.39%20AM.png)<br>
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.43.07%20AM.png)<br>
#### Degree of freedom = 5
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.30.18%20AM.png)<br>
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.43.18%20AM.png)<br>
#### Degree of freedom = 6
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.31.29%20AM.png)<br>
![](https://github.com/Ananyaiitbhilai/Assignment-1a-Implementing-new-distribution-in-D3-and-contributing-to-Opensource/blob/main/local%20images/Screenshot%202022-01-17%20at%201.43.37%20AM.png)<br>
The link for my observable notebook is : https://observablehq.com/d/828cb6afa0941dda
### Reference links
- https://observablehq.com/@dswalter/normal-distribution
- https://observablehq.com/@herbps10/gamma-distribution
