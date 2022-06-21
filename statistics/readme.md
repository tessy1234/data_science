Goal:
-----
The purpose of this section is to show examples of hypothesis testing and statistical analysis.

Problem Statement:
------------------
A)
Observational study, in which researchers observe participants. 
In this case the number of hot wings eaten and beer consumed by patrons of a bar.

Observation: On average men eat more hot wings than women. Is this difference a random or real effect?

B)
Given two independent Gaussian variables X and Y, with probability density functions PDF1 and PDF2, 
then the task ist to calculate the total PDF of the sum of the two gaussian random variables: 

&emsp; Z = X + Y ~ PDF(Z)

Dataset:
--------
A)
Data source: Beerwings.csv

C)
Data source: 

Result:
-------
&ensp; Observational study, in which researchers observe participants. In this case the number of hot wings eaten and beer consumed by patrons of a bar.
  
A)
The claim that men eat more hot wings than women is a real effect.

B)
The probability density function of Z was calculated by the convolution of PDF1 and PDF2 with mean and variance of PDF(Z): 

&emsp; E(Z)=E(X)+E(Y) and Var(Z)=Var(X)+Var(Y)

&emsp; It should be pointed out that a confined grid size can cause out-of-range error. Therefore be careful to set up the grid size correctly!

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

