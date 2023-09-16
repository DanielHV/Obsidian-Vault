---
fecha: 8-09-2023
---

# Algoritmo de minimización

I: $M=\{Q,\Sigma,q_{0},\delta,A\}$ un AFD
O: Un AFD $M'$ tal que $L_{M}=L_{M'}$ y $M'$ es mínimo 

1. Genera todas las parejas $\{p,q\}$ con $p \neq q$
2. Marca cada pareja $\{p,q\}$ en la que exactamente una de $p$ y $q$ esté en $A$
3. Mientras se marque al menos una pareja, repite
4. Para cada pareja $\{r,s\}$, si existe $\sigma \in \Sigma$ tal que $\{\delta(r,\sigma),\delta(s,\sigma)\}$ está marcado, marca $\{r,s\}$
5. Para cada estado $p$ de $M$.
	6. Si $\{p,q\}$ está marcado para cada $q$ ya revisado,  crea un nuevo estado $\{p\}$
	7. Si no, sea $X$ el nuevo estado que contiene al primer $q$ tal que $\{p,q\}$ no está marcado, y agrega $p$ a $X$.
8. Agrega una transición de $X$ a $Y$ con el símbolo $\sigma$ si existen $p \in X, q \in Y$ tales que $\delta(p,\sigma) = q$
9. Marca como estado de aceptación a $X$ si cada elemento de $X$ está en $A$.


Dado $M = \{Q,\Sigma,q_{0},\delta,A\}$ ¿Es $L_{M}$ vacío?
Dado $M = \{Q,\Sigma,q_{0},\delta,A\}$ ¿Es $L_{M}$ infinito?