---
title: "Notes for Complex Analysis"
date: 2024-3-10T11:00:00-04:00
categories:
  - notes
tags:
  - Math
image: /assets/images/2024-3-10-complex-analysis-notes_1.jpg
excerpt: "Notes for reading Complex Analysis (Princeton Lectures in Analysis, No. 2)"
---

<img src="/assets/images/2024-3-10-complex-analysis-notes_1.jpg" alt="book cover">

From this day forward, I'll be reading the book $\textit{Complex Analysis (Princeton Lectures in Analysis, No. 2)}$ for at least 1 hour
per day until I finish the book. I'll put anything I thought interesting/important on this page.

Ch1 \\
A $\textbf{holomorphic}$ function (defined to be a function with a first derivative) is infinitely many times complex differentiable.
i.e. the existence of the first derivative will guarantee the existence of derivatives of any order.

$\textbf{Cauchy-Riemann}$ equations: 
$$\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y} \ and
 \ \frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}$$ (equivalent to $\frac{\partial f}{\partial \overline{z}} = 0$)\\
$f = u + iv$, f is complex differentiable at a complex point iff(if and only if) the partials of u and v satisfy the Cauchy-Riemann equations at that point.

A function that is $\textbf{analytic}$ i.e. has a power series expansion at every point on $\Omega$ is also holomorphic here. The reverse is also true.

A $\textbf{primitive}$ for $f$ on $\Omega$ is a functioin $F$ that is holomorphic on $\Omega$ and such that $F'(z)=f(z)$ for all $z \in \Omega$. \\
If a continuous function $f$ has a primitive $F \in \Omega$ and $\gamma$ is a curve in $\Omega$ that begins at $\omega_1$ and ends at $\omega_2$, then

$$\int_\gamma f(z) dz = F(\omega_2) - F(\omega_1)$$

Thus, it follows naturally that if $\gamma$ is a closed curve in an open set $\Omega$, and $f$ is continuous and has a primitive in $\Omega$, then

$$\int_\gamma f(z)dz = 0$$

Ch2 \\
Updates on Oct. 31 2024: So I quit reading the book as I feel I have pretty much got what I need as a physicist, for now at least. If I found something 
useful I'll put it up here.

$\textbf{Cauchy's integral formula}$:

$$f(a) = \frac{1}{2 \pi i} \oint_{\gamma} \frac{f(z)}{z - a} \, dz.$$

$f$ being holomorphic.