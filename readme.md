# 1. CSE107 Discrete Mathematics and Statistics

<!-- TOC -->

- [1. CSE107 Discrete Mathematics and Statistics](#1-cse107-discrete-mathematics-and-statistics)
  - [1.1. Number Systems and Proof Techniques](#11-number-systems-and-proof-techniques)
    - [1.1.1. Types of Numbers](#111-types-of-numbers)
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
      - [1.2.6.6. De Morgan's laws](#1266-de-morgans-laws)
    - [1.2.7. Power set](#127-power-set)
      - [1.2.7.1. Some laws](#1271-some-laws)

<!-- /TOC -->

## 1.1. Number Systems and Proof Techniques

### 1.1.1. Types of Numbers

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

* $B = \lbrace 1,3,5\rbrace$
* $\Rightarrow$ $1 \in B, 2 \notin B$
* For inexplicit set:  $S = \lbrace x | P(x)\rbrace$  e.g. 
    * $S = \lbrace x|x$ is an odd positive integer$\rbrace$
    * $C = \lbrace n^2|n$ is an integer$\rbrace$

### 1.2.2. Important Sets

* Natural Numbers $N = \lbrace0,1,2…\rbrace$
* Integers $Z = \lbrace …-1,0,1…\rbrace$
* Positive Integers $Z^+ = \lbrace1,2,3…\rbrace$
* Rationals $Q = \lbrace\frac{x}{y}|x,y\in Z , y \ne 0\rbrace$
* Real numbers $R = Z + Q$

### 1.2.3. Subset

* If **every** element of B is an element of A, then B is the subset of A. Notation: $B\subseteq A$.

### 1.2.4. Equality

If $B\subseteq A$ and $A\subseteq B$, then $A=B$.

### 1.2.5. Operations on sets

First of all, the sets to be operated must have **the same data type**.

#### 1.2.5.1. Union

  $A\bigcup B = \lbrace x|x\in A \bigvee x \in B\rbrace$
  
#### 1.2.5.2. Intersection

  $A\bigcap B = \lbrace x|x\in A \bigwedge x \in B\rbrace$

#### 1.2.5.3. Relative complement
  
  $A-B= \lbrace x|x\in A \bigwedge x \notin B\rbrace$
  
#### 1.2.5.4. Complement

  $\sim A=\lbrace x\notin A\rbrace$

#### 1.2.5.5. **Symmetric difference**

  $A\triangle B=\lbrace x|(x\in A \bigwedge x\notin B)\bigvee(x\notin A \bigwedge x\in B)\rbrace$

### 1.2.6. Algebra of sets

 Suppose $A,B,C \subseteq U$ in all the situations below.

#### 1.2.6.1. Commutative laws

  $A\bigcup B=B\bigcup A,A\bigcap B = B \bigcap A$

#### 1.2.6.2. Associative laws

  $A\bigcup(B\bigcup C)= (A\bigcup B)\bigcup C, A\bigcap(B\bigcap C)= (A\bigcap B)\bigcap C$

#### 1.2.6.3. *Identity laws*

  $A\bigcup \emptyset=A,A\bigcup U = U, A\bigcap U = A, A\bigcap \emptyset= \emptyset$

#### 1.2.6.4. **Distributive laws**

  $A\bigcap (B \bigcup C)= (A\bigcap B)\bigcup(A\bigcap C), A\bigcup(B\bigcap C)=(A\bigcup B)\bigcap(A\bigcap C)$

#### 1.2.6.5. *Complement laws*

  $A\bigcup \sim A=U, \sim U = \emptyset, \sim(\sim A)= A, A\bigcap \sim A=\emptyset,\sim \emptyset = U$

#### 1.2.6.6. **De Morgan's laws**
 $\sim (A \bigcup B)= \sim A\bigcap \sim B,\sim (A \bigcap B)= \sim A\bigcup \sim B$

### 1.2.7. Power set

The power set *Pow*(A) is the set of all the subsets of A, denoted by $Pow(A)=\lbrace C|C\subseteq A\rbrace$.

#### 1.2.7.1. Some laws

  $\forall A,B, Pow(A\bigcap B)= Pow(A) \bigcap Pow(B)$
  
  $\exists A,B, Pow(A\bigcup B)\not = Pow(A) \bigcup Pow(B)$