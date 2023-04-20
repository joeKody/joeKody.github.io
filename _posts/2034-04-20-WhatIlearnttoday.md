---
title: What I learnt today (real)
date: 2023-04-20 19:30:39 +0700
categories: [Study]
tags: [math]
math: true
---

# What I have learnt today, so far.

So far, I have *ZERO* thing learnt, but except this one thing.

## Find the last three digits of $7^{9999}$

This is a problem from POSN number theory book

### Solution
$$
\begin{align*}
&\text{Observe } &7^4 &= 2401 \newline
&\text{Then } &7^{4n} &= (2400 + 1)^n \newline
&&7^{4n} &= 1^n + (n \cdot 2400 ) + \dots \newline
\end{align*}
$$

$\text{This means that the last three digit of } 7^{4n} \text{comes from } 1 + (n \cdot 2400)$
> $1 + (n \cdot 24 \cdot 100)$ so, the last digits of $24n$ is the hundredths digit 
{: .prompt-info}

$$
\begin{align*}
\text{Let }n &= 2499 \newline
7^{4 \cdot 2499} &= 7^{9996} \newline
\end{align*}
$$

$\text{Therefore the last three digits of }7^{9996} \text{ is from } 1 + (n \cdot 2400)$

$$
\begin{align*}
&{1 + (2499) \cdot (2400)} \newline
&{1 + (\dots 600)} \newline
\end{align*}
$$

$\text{The last three digits are } 601$

$$
\begin{align*}
7^{9999} &= 7^{9996} \cdot 7^{3} \newline
(\dots 601) \cdot 343 &= \dots 143 &7^{3} = 343& \newline
\end{align*}
$$

$\text{Answer : } 143$