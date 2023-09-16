---
fecha : 23-08-2023
---
## Definición
Dados dos alfabetos $\Sigma$ y $\Gamma$, una función parcial en $(\Sigma^*)^k$ con val en $\Sigma^*$ es una función $f$ tal que $dom(f) \subseteq (\Sigma^{*})^{k}$ y $im(f) \subseteq \Gamma^{*}$.

## Definición
Sean $f$ una función parcial sobre $(\Sigma^*)^*$ con valores en $\Gamma^*$ y $M$ una máquina de Turing.
Diremos que $M$ computa a $f$, sí y solo sí, $L(M) = dom(f)$ y para toda $(x_{1},...,x_{k}) \in dom(f)$ se tiene que $q_{0}x_{1}\square x_{2}\square ... \square x_{k} \vdash^{*} q_af(x_{1},...,x_{k})$   
## Definición
Dada una función parcial $f$, se dice que $f$ es Turing-computable sí y solo sí existe una MT $M$ que computa a $f$.