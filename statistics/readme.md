Goal:
-----
The purpose of this section is to show examples of hypothesis testing and statistical analysis.

Problem Statement:
------------------
<dl>
    <dt>A)</dt>
    <dd>
Observational study, in which researchers observe participants. 
In this case the number of hot wings eaten and beer consumed by patrons of a bar.
	</dd>
    <dd>
Observation: On average men eat more hot wings than women. Is this difference a random or real effect?
	</dd>
    <dt>B)</dt>
    <dd>
In a general social survey American were asked whether he or she favor or oppose the death penalty for murder. The question to be answered is, does support for death penalty depends on education. 	
	</dd>
    <dd>
In this example two categorical variables, Education and DeathPenalty, are tested for independence.
	</dd>
    <dt>C)</dt>
    <dd>
Given two independent Gaussian variables X and Y, with probability density functions PDF1 and PDF2, 
then the task ist to calculate the total PDF of the sum of the two gaussian random variables: 
	</dd>
    <dd>
Z = X + Y ~ PDF(Z)	
	</dd>
</dl>

Dataset:
--------
<dl>
    <dt>A)</dt>
    <dd>
Data source: &nbsp;Beerwings.csv	
	</dd>	
    <dt>B)</dt>
    <dd>
Data source: &nbsp;GSS2002.csv	
	</dd>	
</dl>

Result:
-------
<dl>
    <dt>A)</dt>
    <dd>
The null hypthesis to be tested is whether females consume as many hot wings as males.
	</dd>
    <dd>
The null hypthesis is declined.	
On average men eat more hot wings than women.
	</dd>
    <dd>
For more details see repo: <code>two_sample_permutation_test_demo.ipynb</code>
	</dd>
    <dt>B)</dt>
    <dd>
The null hypthesis to be tested is whether education and opinion about death penalty are independent.	
	</dd>
    <dd>
The null hypthesis is declined.
The p-value lies beneath the significant level of 1 percent and thus the conclusion is that education and support for death penalty are not independent.	
	</dd>
    <dd>
For more details see repo: <code>permutation_test_for_independence_of_two_variables_demo.ipynb</code>
	</dd>
    <dt>C)</dt>
    <dd>
The probability density function of Z was calculated by the convolution of PDF1 and PDF2 with mean and variance of PDF(Z): 
	</dd>
    <dd>
E(Z)=E(X)+E(Y) and Var(Z)=Var(X)+Var(Y)
	</dd>
	<dd>
It should be pointed out that a confined grid size can cause out-of-range error. Therefore be careful to set up the grid size correctly!
	</dd>
</dl>

1. Sum of standard Gaussian random variables: 
	- Given two independent gaussian variables: E(X)=E(Y)=0 and Var(X)=Var(Y)=1
	- Correct solution: Result was E(Z)=E(X)+E(Y)=0 and Var(Z)=Var(X)+Var(Y)=2
2. Sum of Gaussian random variables - confined grid size:
	- Given two independent gaussian variables: E(X)=E(Y)=2 and Var(X)=Var(Y)=8
	- Approximate solution with large errors: Result was E(Z)=E(X)+E(Y)=3.21 and Var(Z)=Var(X)+Var(Y)=12.21 but expected was E(Z)=E(X)+E(Y)=4.0 and Var(Z)=Var(X)+Var(Y)=16.0.
3. Sum of Gaussian random variables - enlarged grid size
	- Given two independent gaussian variables: E(X)=E(Y)=2 and Var(X)=Var(Y)=8
	- Correct solution: Result was E(Z)=E(X)+E(Y)=3.999 and Var(Z)=Var(X)+Var(Y)=15.991 and compare it with the exact solution E(Z)=E(X)+E(Y)=4.0 and Var(Z)=Var(X)+Var(Y)=16.0.
	The relatively small difference between the observed and exact solution arises from floating point arithmetic and the discretisation onto the grid.
<dl>
    <dd>
For more details see repo: <code>sum_of_gaussian_random_variables_test_*.ipynb</code>
	</dd>
</dl>
