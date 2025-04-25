+++
date = '2025-04-25T16:16:55-06:00'
draft = true
title = 'Solved exercises of Commutiative Algebra's Atiyah'
+++


# Chaper 1


## Let be $x$ a nilpotent element of a ring $A$. Show that $1+x$ is a unit of $A$. Deduce that the sum of a nilpotent element and a unit is a unit.

Let be $k>1$ the smallest integer such that $x^k=0$, then we see that

\begin{equation}
    (1+x)(1-x+\ldots+(-1)^{k-1}x^{k-1})=1+(-1)^{k-1}x^k=1.
\end{equation}

Analogous we see that for a unit $u\in A$ with $uv=1$ then

\begin{equation}
    (u+x)=u(1+vx).
\begin{equation}
Noticing that $(vx)^k=$, then
\beging{equation}
    (u+x)v(1+vx+\ldots+(-1)^{k-1}v^{k-1}x^{k-1})=(1+vx)(1+vx+\ldots+(-1)^{k-1}v^{k-1}x^{k-1})=1.
\end{equation}

## Let $A$ be a ring and let $A[x]$ be the ring of polynomials in an inderteminate $x$, with coefficients in $A$. Let $f=a_0+a_1x+\ldots+a_nx^n$. Prove that
### f is a unit iff $a_0$ is a unit in $A$ and $a_1,\ldots,a_n$ are nilpotent.
