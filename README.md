# Assignment 1a: Implementing new distribution in D3 and contributing to Opensource
## Implementation details and workflow
I have made both pdf and cdf for chi-square distribution and have visulaised it through pachinko function for random values of x and Chart for continuous graph. 
First I wrote Gamma function which was computed using Lanczos approximation. As written in observable notebook itself Chi-square function uses Gamma function for computation. 
${tex.block`
\mathrm{\chi^2}(x | k) = \frac{1}{{2^\frac{k}{2}} \Gamma(\frac{k}{2})} x^{\frac{k}{2}-1} e^{-\frac{x}{2}},\hspace{1em} x\in(0,\infty)
`}
