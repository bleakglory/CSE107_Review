# 1. CSE107 Discrete Mathematics and Statistics

<!-- TOC -->

- [1. CSE107 Discrete Mathematics and Statistics](#1-cse107-discrete-mathematics-and-statistics)
  - [1.1. Numbers Systems and Proof Techniques](#11-numbers-systems-and-proof-techniques)
    - [1.1.1. Types of Numberss](#111-types-of-numberss)
  - [1.2. Proof Techniques](#12-proof-techniques)
    - [1.2.1. Proof by contradiction](#121-proof-by-contradiction)
    - [1.2.2. Proof by induction](#122-proof-by-induction)

<!-- /TOC -->

## 1.1. Numbers Systems and Proof Techniques

### 1.1.1. Types of Numberss

* Natural Numbers
  - **Closed under addition**
* Integer
* Relational Numbers
  - Can be expressed as $\frac{x}{y}$ where $x,y\in Q$ and $y \ne 0$
  
* Real Numbers
* Prime Numbers  *质数*

## 1.2. Proof Techniques

### 1.2.1. Proof by contradiction

Example: Use proof by contracdition to prove $\sqrt{2}$ is a irrational number:

> * If $\sqrt{2}$ were rational, then it can be written as $\sqrt{2}= \frac{x}{y}$ where $x,y\in Q$ and $x,y \ne 0$
> * By repeatedly cancelling common factors, we can make sure that $x,y$ have no common factors so they are not both even.
> * Since $2=\frac{x^2}{y^2}$, so $x^2$ is even, then $x$ is even.
> * Let $x = 2w$, $w \in N$.
> * Then $x^2 =4w^2$ so$4w^2 =2y^2$, $y^2 =2w^2$ so $y^2$ is even then so is $y$.
> * This contradicts the fact that x and y are not both even, so 2 being rational, must have been wrong.

### 1.2.2. Proof by induction

Normal steps:

1. Prove the first number holds the property.
2. Prove that if $n = m$ holds the property, then so is $n=m+1$.

Examples:

* For every natural number $n$, $2^{n+2} + 3^{2n+1}$ is divisible by $7$
