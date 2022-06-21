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
Given two independent Gaussian variables X and Y, with probability density functions pdf1 and pdf2, 
then the task ist to calculate the total PDF of the sum of the two gaussian random variables: 

Z = X + Y ~ PDF(Z)

Dataset:
--------
Data source: Beerwings.csv

Result:
-------
A)
The claim that men eat more hot wings than women is a real effect.

B)
The probability density function of Z was calculated by the convolution of pdf1 and pdf2. 
The test was based on mean=0 and sigma²=1 for both pdf1 and pdf2 and provided the correct solution for the Gaussian PDF of Z with 

E(Z)=E(X)+E(Y)=0 and Var(Z)=Var(X)+Var(Y)=2

1. Sum of standard Gaussian random variables: 
	- Correct solution: Result was E(Z)=E(X)+E(Y)=0 and Var(Z)=Var(X)+Var(Y)=2
2. Sum of Gaussian random variables - confined grid size:
	- approximate solution with large errors: Result was E(Z)=E(X)+E(Y)=3.21 and Var(Z)=Var(X)+Var(Y)=12.21 but expected was E(Z)=E(X)+E(Y)=4.0 and Var(Z)=Var(X)+Var(Y)=16.0.
3. Sum of Gaussian random variables - enlarged grid size

