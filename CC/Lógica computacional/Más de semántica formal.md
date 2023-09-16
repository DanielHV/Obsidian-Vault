---
fecha : 30-08-2023
---
# Semántica formal

## Estado de variables
$\sigma : \textrm{Var} \rightarrow Bool \{0,1\}$
$\sigma(p) = v$
$p \in \textrm{Var}$
## Interpretación
$I_{\sigma} : LPROP \rightarrow Bool$
def recursiva $I_{\sigma}(\varphi)$

$\sigma[p/v](q)= \sigma(p)$ si $p \neq q$
			   $v$ si $p = q$
$p \in \textrm{Var}$
$v \in \{0,1\}$

## Lema de sustitución
$I_{\sigma}(\varphi[p:=\uppsi]) = I_{\sigma[p/v]}(\varphi)$

