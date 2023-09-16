---
fecha : 25-08-2023
---
# Sustitución en LPROP

Cambiar una variable en una fórmula $\varphi_1$ por una formula $\varphi_2$
$\varphi_1[p:=\varphi_2]$
$\varphi_1[\varphi_2/p]$
## Estrategia
- Revisar paréntesis en $\varphi$
- Buscar la variable a cambiar

`sust`
$p[q:=\varphi] = p=q \ \ \varphi$ 
				$p \neq q \ \ p$
$\top[q:=\varphi]=\top$
$\bot[q:=\varphi]=\bot$
$(\varphi_{1} \diamond \varphi_{2})[q:=\varphi]=\varphi1[q=\varphi]\diamond \varphi_{2}[q:=\varphi] \ \ \ \ \diamond \in \{\land, \lor, \rightarrow, \leftrightarrow\}$
$\neg \varphi_{1}[q:=\varphi] = \neg(\varphi_1[q:=\varphi])$
$((\varphi_1))[q:=\varphi] = (\varphi_{1}[q:=\varphi]))$

###### Ejemplo
$\varphi_{1} = ((p \rightarrow q) \rightarrow r) \rightarrow (r \land t)$
$(\varphi_{1})[r:=q \lor t]$ 
$=$
$((p \rightarrow q) \rightarrow r)[r:= q \lor t] \rightarrow (r \land t)[r:=q \lor t] =$
$((p \rightarrow q)[r:=q \lor t] \rightarrow r[r:=q \lor t]) \rightarrow (r[r:=q \lor t]\land t[r:=q \lor t]) =$
$((p[r:=q \lor t] \rightarrow q[r:=q \lor t]) \rightarrow r[r:=q \lor t]) \rightarrow (r[r:=q \lor t] \land t[r:=q \lor t]) =$
$((p \rightarrow q) \rightarrow q \lor t) \rightarrow (q \lor t) \land t$

## Definición
$\varphi[p:=\uppsi][q:=\upchi] = \varphi[q:=\upchi][p:=\uppsi[q:=\upchi]]$
si $p \neq q$ & $p \notin \textrm{vars}(\upchi)$

 

