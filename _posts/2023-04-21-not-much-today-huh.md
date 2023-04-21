---
title: Not much studying today
date: 2023-04-21 20:00:00 +0700
category: [Study]
tags: [math]
math: true
---
# Not much studying today, huh

I started this day a bit badly, though I gave a nice resolution in the previous blog. I wasn't as productive as I thought. I get distracted a lot. Maybe it's time to use the pomodoro, welp, I guess let's try that tomorrow. But now, let's recap what I have done for today.

## Basic logarithms

I started to forget what I actually studied today, but I can faintly remembers.

### Logarithm rules/identities

$$ a^{\log _a n} = n $$  
$$ \log _a a = 1 $$  
$$ \log _a 1 = 0 $$  
$$ \log _a xy = \log _a x + \log _a y $$  
$$ \log _a \frac{x}{y} = \log _a x - \log _a y $$  
$$ \log _a x^k = k \cdot \log _a x $$  
$$ \log _{a^k} x = \frac{1}{k} \cdot \log _a x $$  
$$ \log _a x = \frac{\log _k x}{\log _k a} $$  
$$ \log _a x \cdot \log _k a = \log _k x $$  
$$ \log _a x = \frac{1}{\log _x a} $$  
$$ a^{\log _b c} = c^{\log _b a} $$  

Welp, the proofs are mostly based on exponents/indices  
The key is to view the log equations as indices

### Nice problems
Much thanks to CaptainTimmy and ChawinKN who gave me their past works and sheets so that I can study off of that

1. Getting used to basic rules
$$ \log _2 (\log _3 10^{12}) - \log _2 (\log _3 10^3) $$
: We could use all the rules we know and something will show, probably
$$ \log _2 (12 \cdot \log _3 10) - \log _2 (3 \cdot \log _3 10) $$

$$ \log _2 \frac{12 \cdot \log _3 10}{3 \cdot \log _3 10} $$

$$ \log _2 \frac{12 \cdot \cancel{\log _3 10}}{3 \cdot \cancel{\log _3 10}} $$

$$ \log _2 4 $$

Which the answer is 2! You just have to work out small things first, then it will become very obvious!

2. Can you really remember the rules?
: these are two quick problems

$$
\log _3 81 \cdot \log _5 125 + \log _{27} 81 \cdot \log _{\frac{1}{2}} 64 \\
$$

$$\begin{align*}
    &= (4)(3) + (4 \cdot \log _{3^3} 3)(6 \cdot \log _{2^{-1}} 2) \\
    &= 12 + \frac{4}{3}(1) \cdot {-6}(1) \\
    &= 12 - \frac{12}{3}
\end{align*}$$

$$
\log _2 3 \cdot \log _3 4 \cdot \log _4 5 \cdot \dotso \cdot \log _{255} 256
$$

$$\begin{align*}
    &= \frac{\log 3}{\log 2} \cdot \frac{\log 4}{\log 3} \cdot\frac{\log 5}{\log _4} \cdot \dotso \cdot \frac{\log {256}}{\log {255}} \\
    &= \frac{\cancel \log 3}{\log 2} \cdot \frac{\cancel \log 4}{\cancel \log 3} \cdot\frac{\cancel \log 5}{\cancel \log 4} \cdot \dotso \cdot \frac{\log {256}}{\cancel \log 255} \\
    &= \frac{\log 256}{\log 2} = \log _2 256 \\
    &= 8
\end{align*}$$

That's all for logarithms for today (I'm giving up)

## Some POSN problems

### Factor problem
Find the smallest $n$ if $n + (n+1) + (n+2) + \dotso + (n+k) = 10,000$ and $k, n \in \mathbb{I}$  
Solution  
: Let's simplify the question

$$\begin{align*}
(k+1)n + \frac{(k + 1)k}{2} &= 10,000 
\\ (k+1)2n + (k+1)k &= 20,000 = 2 \cdot 10^4 = 2 \cdot (2\cdot 5)^4
\\ (k+1)(2n + k) &= 20,000 = 2^5 \cdot 5^4
\end{align*}$$

We want the smallest possible $n$ which means we have to find the biggest possible $k$ (from the question)  
: This means that $k + 1$ should be less than $\sqrt{20000}$ because $(k + 1)(2k + 1) = 20000$  

$$\begin{align*}
k + 1 &\lt \sqrt{20000} &(\sqrt{20000}\approx 141)\\
&\le 141 \\
20,000 &= 2^5 \cdot 5^4 \\
5^3 &\lt 141 \\
k + 1 &= 125 &(\text{k + 1 is a factor of 20,000 that's less than 141})
\end{align*}$$

Substitute to find n

$$\begin{align*}
(k+1)(2n+k) &= 20,000 \\
2n+k &= \frac{20,000}{125} \\
2n + k &= 2^5 \cdot 5 \\
2n &= 2^5 \cdot 5 - 124 \\
n &= 2^4 \cdot 5 - 62 \\
n &= 80 - 62 = 18
\end{align*}$$

The answer is 18!  

### Nice, easy, but rare  
If $N$ is a number in decimal which has 10 digits, and the digits are $a_9 a_8 a_7 a_6 \dotso a_2 a_1 a_0$ such that $a_9 = 6$ and $a_8 a_7 a_6 \dotso a_2 a_1 a_0 = \frac{N}{25}$  
Find $a_9+a_8+a_7+a_6+\dotso+a_2+a_1+a_0$

Solution
: $ a_9 a_8 a_7\dotso $ means a number which digits are $a_9$ and so on. Not a product
$$\begin{align*}
N &= a_9 \cdot 10^6 + a_8 a_7 a_6 \dotso a_2 a_1 a_0 \\
N &= 6\cdot 10^6 + \frac{N}{25} \\
25N &= 25\cdot 6\cdot 10^6 + N \\
24N &= 5^2 \cdot 6 \cdot 2^6 \cdot 5^6 \\
N &= 5^8 \cdot 2^4 \\ &= 10^4 \cdot 5^4
\end{align*}$$

This means that the digits that aren't zero comes from $5^4$ therefore, the sum of all digits are sum of all digits from $5^4$  
: $5^4 = 625$ which the sum is 13

The anser is 13!