---
title: Short math stuff
date: 2023-04-23 13:06:35 +0700
categories: [Study]
tags: math
math: true
---

# How to deal with integers in math problems + example
The only thing to look out for math problems including integers solutions, is **factored form**. Simplify/organize the equations such that a **product of the solutions** is equal to a number. And remember the best factoring trick, **wish hard**.  
  
Well, Let's hop into the examples.  

## Factoring trick

Find the biggest value of $m - n$ if $m \ge n$ and

$$\frac{1}{m} + \frac{1}{n} = \frac{2}{33}$$

Solution  

$$
\begin{align*}
\frac{m+n}{mn} &= \frac{2}{33} \\
33(m+n) &= 2mn \\
2mn - 33(m+n) &= 0 \\
2mn - 33m -33n &= 0
\end{align*}
$$

$\text{I really wish it could be factored in the form of } (2m - k_1)(n - k_2) = c$  
$\text{But, I only have 33 as the coefficient of the variables. Which isn't easy to factor.}$  
$\text{Since the coefficient of either } m \text{ or } n \text{ is 2. } 33m \text{ or } 33n \text{ won't be easy to get.}$  
$\text{I wished so hard that 33 has factor so I will just multiply the entire equation by 2.}$  

$$4mn - 66m -66n = 0$$

$\text{I think factored form of } (2m - k_1)(2n - k_2) \text{ is nice. Let's see.}$  

$$
\begin{align*}
(2m - k_1)(2n - k_2) &= 0 \\
4mn - 2k_2m - 2k_1n + k_1k_2 &= 0
\end{align*}
$$

$\text{Compare that with } 4mn - 66m - 66n = 0$  
$k_1 = k_2 = 33 \text{ but, we don't have } k_1k_2$  
$\text{ So, let's think that we have added it to both side}$

$$
\begin{align*}
4mn - 2k_2m - 2k_1n + k_1k_2 &= k_1k_2 \\
4mn - 2(33)m -2(33)n + 33^2 &= 33^2 \\
4mn - 66(m+n) + 33^2 &= 33 ^2
\end{align*}
$$

$\text{Let's go back to the factored form to find the solutions}$

$$(2m - 33)(2n - 33) = 33^2$$

$\text{To find the biggest value of } m-n$  
$\text{We have to assume } (2m-33) \text{ is the biggest factor of } 33^2 \text{ which is } 33^2$  
$\text{This means } (2m - 33) = 1$  

$$
\begin{align}
2m &= 33^2 + 33 \\
2n &= 1 + 33 \\
2m - 2n &= 33^2 + 33 - 1 - 33 \nonumber \tag{(1) - (2)} \\
2m - 2n &= 33^2 - 1 \nonumber \\
m - n &= {(33 - 1)(33 + 1)\over2}\nonumber \\
&= {32\over 2}\cdot 34 \nonumber \\
&= 16 \cdot 34 \nonumber \\
&= 544 \nonumber
\end{align}
$$

: Ans 544

## Trial and error

If $m, n \in \mathbb{I}^+$ and $\gcd (m, n) = 20, \text{lcm}(m, n) = 50,400$. Find the smallest $m + n$  
: Solution
$$\text{from gcd}(a, b) \cdot \text{lcm}(a, b) = ab$$

$$\begin{align*}
20 \cdot 50,400 = mn
\end{align*}$$

$\text{Assume }m \ge n $  
$\text{We know  }n \text{ must be atleast 20 and we need to find smallest }m + n$  
$\text{The solution is to try plug in every possible value and hope it's the smallest}$
$\text{At least that's what I thought(I won't do it here lol.)}$  
$\text{If someone could find anybetter solition, please comment below}$