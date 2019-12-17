# 1. CSE107 Discrete Mathematics and Statistics

<!-- TOC -->

- [1. CSE107 Discrete Mathematics and Statistics](#1-cse107-discrete-mathematics-and-statistics)
  - [1.1. Numbers Systems and Proof Techniques](#11-numbers-systems-and-proof-techniques)
    - [1.1.1. Types of Numberss](#111-types-of-numberss)
    - [1.1.2. Proof Techniques](#112-proof-techniques)
      - [1.1.2.1. Proof by contradiction](#1121-proof-by-contradiction)
      - [1.1.2.2. Proof by induction](#1122-proof-by-induction)
  - [1.2. Set Theory](#12-set-theory)
    - [1.2.1. Notation](#121-notation)
    - [1.2.2. Important Sets](#122-important-sets)
    - [1.2.3. Subset](#123-subset)
    - [1.2.4. Equality](#124-equality)
    - [1.2.5. Operations on sets](#125-operations-on-sets)
      - [1.2.5.1. Union](#1251-union)
      - [1.2.5.2. Intersection](#1252-intersection)
      - [1.2.5.3. Relative complement](#1253-relative-complement)
      - [1.2.5.4. Complement](#1254-complement)
      - [1.2.5.5. Symmetric difference](#1255-symmetric-difference)
    - [1.2.6. Algebra of sets](#126-algebra-of-sets)
      - [1.2.6.1. Commutative laws](#1261-commutative-laws)
      - [1.2.6.2. Associative laws](#1262-associative-laws)
      - [1.2.6.3. Identity laws](#1263-identity-laws)
      - [1.2.6.4. Distributive laws](#1264-distributive-laws)
      - [1.2.6.5. Complement laws](#1265-complement-laws)

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

### 1.1.2. Proof Techniques

#### 1.1.2.1. Proof by contradiction

Example: Use proof by contracdition to prove $\sqrt{2}$ is a irrational number:

* If $\sqrt{2}$ were rational, then it can be written as $\sqrt{2}= \frac{x}{y}$ where $x,y\in Q$ and $x,y \ne 0$
* By repeatedly cancelling common factors, we can make sure that $x,y$ have no common factors so they are not both even.
* Since $2=\frac{x^2}{y^2}$, so $x^2$ is even, then $x$ is even.
* Let $x = 2w$, $w \in N$.
* Then $x^2 =4w^2$ so$4w^2 =2y^2$, $y^2 =2w^2$ so $y^2$ is even then so is $y$.
* This contradicts the fact that x and y are not both even, so 2 being rational, must have been wrong.

#### 1.1.2.2. Proof by induction

Normal steps:

1. Prove the first number holds the property.
2. Prove that if $n = m$ holds the property, then so is $n=m+1$.

Examples:

* For every natural number $n$, $2^{n+2} + 3^{2n+1}$ is divisible by $7$

## 1.2. Set Theory

### 1.2.1. Notation

* $B = \{1,3,5\}$
* $\Rightarrow$ $1 \in B, 2 \notin B$
* For inexplicit set:  $S = \{x | P(x)\}$  e.g. 
    * $S = \{x|x$ is an odd positive integer$\}$
    * $C = \{n^2|n$ is an integer$\}$

### 1.2.2. Important Sets

* Natural Numbers $N = \{0,1,2…\}$ 
* Integers $Z = \{…-1,0,1…\}$
* Positive Integers $Z^+ = \{1,2,3…\}$
* Rationals $Q = \{\frac{x}{y}|x,y\in Z , y \ne 0\}$
* Real numbers $R = Z + Q$

### 1.2.3. Subset

* If **every** element of B is an element of A, then B is the subset of A. Notation: $B\subseteq A$

### 1.2.4. Equality

If $B\subseteq A$ and $A\subseteq B$, then $A=B$ 

### 1.2.5. Operations on sets

First of all, the sets to be operated must have **the same data type**.

#### 1.2.5.1. Union

  $A\bigcup B = \{x|x\in A \bigvee x \in B\}$
  
#### 1.2.5.2. Intersection

  $A\bigcap B = \{x|x\in A \bigwedge x \in B\}$

#### 1.2.5.3. Relative complement
  
  $A-B= \{x|x\in A \bigwedge x \notin B\}$
  
#### 1.2.5.4. Complement

  $\sim A=\{x\notin A\}$

#### 1.2.5.5. **Symmetric difference**

  $A\triangle B=\{x|(x\in A \bigwedge x\notin B)\bigvee(x\notin A \bigwedge x\in B)\}$

### 1.2.6. Algebra of sets

 Suppose $A,B,C \subseteq U$ in all the situations below.

#### 1.2.6.1. Commutative laws

  $A\bigcup B=B\bigcup A,A\bigcap B = B \bigcap A$

#### 1.2.6.2. Associative laws

  $A\bigcup(B\bigcup C)= (A\bigcup B)\bigcup C, A\bigcap(B\bigcap C)= (A\bigcap B)\bigcap C$

#### 1.2.6.3. *Identity laws*

  $A\bigcup \empty=A,A\bigcup U = U, A\bigcap U = A, A\bigcap \empty= \empty$

#### 1.2.6.4. **Distributive laws**

  $A\bigcap (B \bigcup C)= (A\bigcap B)\bigcup(A\bigcap C), A\bigcup(B\bigcap C)=(A\bigcup B)\bigcap(A\bigcap C)$

#### 1.2.6.5. *Complement laws*