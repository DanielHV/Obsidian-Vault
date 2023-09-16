---
fecha : 23-08-2023
---

NEGS :: LPROP -> N
PARENTESIS :: LPROP -> N
###### Función `vars`:
Cuenta / calcula el número de variables proposicionales en una fórmula.
$\textrm{vars} :: LPROP \rightarrow \mathbb{N}$
$\textrm{vars}(p) = 1, p \in \textrm{vars}$
$\textrm{vars}(\top) = \textrm{vars}(\bot) = 0$
$\textrm{vars}((\mathbb{P})) = \textrm{vars}(\mathbb{P})$
$\textrm{vars}(\neg \mathbb{P}) = \textrm{vars}(\mathbb{P})$
$\textrm{vars}(\mathbb{P} \diamond \mathbb{P}) = \textrm{vars}(\mathbb{P}_{1})+ \textrm{vars}(\mathbb{P}_{2})$
###### Función `vars'`:
Devuelve el conjunto de variables proposicionales en una fórmula.
$\textrm{vars}' :: LPROP \rightarrow \textrm{Var}$
$\textrm{vars'}(p) = {p}, \ p \in \textrm(Var)$
$\textrm{vars}'(\top) = \textrm{vars}'(\bot) = \varnothing$
$\textrm{vars}'((\mathbb{P})) = \textrm{vars}'(\mathbb{P})$ 
$\textrm{vars}'(\neg\mathbb{P}) = \textrm{vars}'(\mathbb{P})$
$\textrm{vars}'(\mathbb{P}\diamond\mathbb{P}) = \textrm{vars}'(\mathbb{P}_{1})\cup\textrm{vars}'(\textrm{P}_{2})$

## Asociatividad
- $\neg$ izq
- $\land$, $\lor$ izq
- $\rightarrow$ der
- $\leftrightarrow$ izq

