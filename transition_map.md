---
lecture: 2
date: 2023-09-08
type: definition
---
# Transition Map
## Motivation
Let $\mathcal{M}$ be a [topological manifold](topological_manifold). The notion of a function $f: \mathcal{M} \to \mathbb{R}$ being [continuous](continuous_mapping) makes sense, because $\mathcal{M}$ is, in particular, a [topological space](topological_space).

Unfortunately, the notion of $f$ being differentiable does not make sense. Let $\left(U, \varphi\right)$ be a [chart](chart) on $\mathcal{M}$. The natural definition would be to call $f$ differentiable on $U$ if $f \circ \varphi^{-1}$ is differentiable. Unfortunately, this does not yield a consistent definition of differentiability, as it depends on the choice of chart. Even if $f \circ \varphi^{-1}$ is differentiable on $U$, if $\left(V, \psi\right)$ is another chart on $\mathcal{M}$, and $U \cap V \neq \varnothing$, then it is not necessarily the case that $f \circ \psi^{-1}$ is differentiable on $U \cap V$.

Observe, however, that $f \circ \varphi^{-1} = f \circ \psi^{-1} \circ \left(\psi \circ \varphi^{-1}\right)$, so we may equate the differentiability of $f$ across charts depending on the differentiability of $\psi \circ \varphi^{-1}$.
## Definition
Let $\mathcal{M}$ be a topological manifold, and let $\left(U, \varphi\right)$ and $\left(V, \psi\right)$ be charts on $\mathcal{M}$. The function $\psi \circ \varphi^{-1}: \varphi\left(U \cap V\right) \to \psi\left(U \cap V\right)$ is called the *transition map* from $\varphi$ to $\psi$.
