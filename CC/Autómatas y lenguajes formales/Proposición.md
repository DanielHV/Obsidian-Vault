---
fecha : 29-08-2023
---

## Proposición
Sean $M_1 = (Q_1,\Sigma,q_1,\delta_1,A_1)$ y $M_2=(Q_2,\Sigma,q_2,\delta_2,A_2)$ AFD con lenguajes $L_1$ y $L_2$ respectivamente.
Si $M=(Q,\Sigma,q_0,\delta,A)$ dado por:
- $Q=Q_{1} \times Q_2$
- $q_{0}=(q_1,q_2)$
- $\delta((p,q),\sigma) = (\delta_1(p,\sigma),\delta_2(q,\sigma))$
1) y $A = \{(p,q) \in Q | p \in A_{1} \lor q \in A_{2}\}$, entonces $L_{M}=L_{1} \cup L_{2}$
2) y $A = \{(p,q) \in Q | p \in A_{1} \& q \in A_{2}\}$, entonces $L_{M}=L_{1} \cap L_{2}$
3) y $A = \{(p,q) \in Q | p \in A_{1} \& q \notin A_{2}\}$, entonces $L_{M}=L_{1} - L_{2}$

### Demostración
Verifiquemos que $\delta^{*}((p,q),w) = (\delta_{1}^*(p,w),\delta_{2}^*(q,w))$
- Si $w = \epsilon$, entonces:
	$\delta^{*}((p,q),\epsilon) = (p,q) = (\delta_{1}^{*}(p,\epsilon),\delta_{2}^{*}(q,\epsilon))$
- Si $w=x\sigma$ con $x \in \Sigma^{*}$ y $\sigma \in \Sigma$
	$\delta^{*}((p,q),w) = \delta^{*}((p,q),x\sigma) = \delta(\delta^{*}((p,q),x)\sigma)$
	$= \delta((\delta_{1}^{*}(p,x),\delta_{2}^{*},(q,x)),\sigma)$
	$= (\delta_{1}(\delta_{1}^{*}(p,x),\sigma),\delta_{2}(\delta_{2}^{*}(q,x),\sigma))$
	$= \delta_{1}^{*}(p,x\sigma),\delta_{2}^{*}(q,x\sigma)$
	$= (\delta_{1}^{*}(p,w),\delta_{2}^{*}(q,w))$

	Por lo tanto, si $w = L_M$, entonces $\delta^{*}((q_{1},q_{2}),w)\in A$, i.e, $(\delta_{1}^{*}(q_{1},w),\delta_{2}^{*}(q_{2},w) \in A$.
	Luego $\delta_{1}^{*}(q,w) \in A_{1}$ y $\delta_{2}^{*}(q_{2},w) \notin A_{2}$. Concluimos que  $w \in L_{1}$ y $w \notin L_{2}$, o bien, $w \in L_{1} - L_{2}$.

Si $w \in L_{1} - L_{2}$, entonces:
$\delta_{1}^{*}(q_{1},w) \in A_{1}$ y $\delta_{2}^{*}(q_{2},w) \notin A_{2}$, por lo tanto $(\delta_{1}^{*}(q_1,w),\delta_{2}^{*}(q_{2},w)) \in A$.
Luego $\delta^{*}((q_{1},q_{2}),w = (\delta_{1}^{*}(q_{1},w),\delta_{2}^{*}(q_{2},w)) \in A$, o equivalente $w \in L_{M}$.
$\blacksquare$






