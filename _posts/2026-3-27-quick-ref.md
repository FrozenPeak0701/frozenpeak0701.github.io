---
title: "Commutations and Formulae"
date: 2026-3-27T6:00:00-05:00
categories:
  - notes
tags:
  - Math
excerpt: "Quick reference"
---
# Commutations

\begin{align\*}
[x_i,p_j] = i \hbar \delta_{ij}
\end{align\*}

$$
a = \sqrt{\frac{m\omega}{2\hbar}} \left( x + \frac{i p}{m\omega} \right), \qquad
a^\dagger = \sqrt{\frac{m\omega}{2\hbar}} \left( x - \frac{i p}{m\omega} \right),
$$

$$
[a, a^\dagger] = \left( \frac{1}{2\hbar} \right) \left( -i[x,p] + i[p,x] \right) = 1.
$$

### Pauli Matrices

$$
\sigma_x=\begin{pmatrix}0&1\\1&0\end{pmatrix},\qquad
\sigma_y=\begin{pmatrix}0&-i\\i&0\end{pmatrix},\qquad
\sigma_z=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

$$
\{\sigma_i,\sigma_j\} = 2\delta_{ij}
$$

$$
[\sigma_i,\sigma_j] = 2i \epsilon_{ijk}\sigma_k
$$

$$
(\boldsymbol{\sigma}\cdot\mathbf{a})(\boldsymbol{\sigma}\cdot\mathbf{b}) = \mathbf{a}\cdot\mathbf{b} + i\boldsymbol{\sigma}\cdot(\mathbf{a}\times \mathbf{b})
$$

# Formulae

**Baker–Hausdorff lemma**
$$
\begin{aligned}
\exp(iG\lambda)\, A\, \exp(-iG\lambda)
=& A + i\lambda[G,A] + \frac{i^2\lambda^2}{2!}[G,[G,A]] + \\
&\cdots + \frac{i^n \lambda^n}{n!}[G,[G,[G,\dots[G,A]]]\dots] + \cdots
\end{aligned}
$$

Special case where $[G,A] = \pm A$,  $ \exp(iG\lambda)\, A\, \exp(-iG\lambda) = A \exp(\pm i\lambda) $.

Let $ x \in \mathbb{R} $ and $ \hat{A}^2 = \mathbb{I} $:
\begin{equation}
  \exp(i \hat{A} x) = \cos(x) \mathbb{I} + i\, \sin(x) \hat{A} \label{expiax}
\end{equation}

One useful substitution of eq.(\ref{expiax}):

$$
  \exp(-\frac{i\vec{\sigma}\cdot\hat{\bf{n}}\phi}{2}) =\mathbb{I} \cos(\frac{\phi}{2}) - i\vec{\sigma}\cdot \hat{\bf{n}} \sin(\frac{\phi}{2})
$$