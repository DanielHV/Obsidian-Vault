---
fecha : 21-08-2023
---

Si $M$ es una MT, una configuración para $M$ consta de tres componentes:
1. El estado actual de $M$
2. Los contenidos actuales de $M$
3. La posición de la cabeza lectora

Si $q \in Q, u,v \in \Gamma^*$ denotamos por $uqv$ a la configuración que está en el estado $q$, el contenido de la cinta es $uv$ y el cabezal apunta a la primera entrada de $v$. 
 
Decimos que una configuración **da lugar a** otra si la segunda se puede obtener en un paso en una ejecución legal de la MT a partir de la primera, i.e, si $u,v \ \in \Gamma^*$, $a,b,c \in \Gamma$, $q_{i},q_{j} \in Q$, entonces $uaq_ibv$ da lugar a $uq_{j}acv$  denotado $uaq_{i}bv$ da lugar a $uq_{j}acv$

La configuración inicial de $M$ con entrada $w$ es $q_{0}w$. 
Un configuración es de aceptación si el estado es $q_{a}$ y de rechazo si el estado es $q_{r}$.

Decimos que $M$ acepta (o rechaza) la entrada $w$ si existen $C_{0},...,C_{k}$ tales que:
1. $C_{0}$ es $q:0 w$
2. $C_i$ da lugar a $C_{i+1}$
3. $C_{z}$ es de aceptación (rechazo)

Si existe una sucesión infinita $C_{i}, i \in \mathbb{N}$ tal que $C_{0}$ es $q_0w$, $C_i$ da lugar a $C_{i+1}$ y $C_i$ no es de aceptación ni de rechazo para cada $i \in \mathbb{N}$, decimos que $M$ se cicla con entrada $w$.

Las configuraciones de aceptación y de rechazo se llaman configuraciones de paro.


El conjunto de cadenas aceptadas por una MT $M$ es el lenguaje de $M$ o el lenguaje reconocido por $M$ denotado $L_{M}$ o $L(M)$.

* ## Definición
	Un lenguaje $L$ es Turing-reconocible o reconocible si existe una MT $M$ tal que $L_{M} = L$.

Una MT $M$ es un decididor si no se cicla con entrada alguna.

* ## Definición
	Un lenguaje $L$ es Turing-decidible si existe un decididor $M$ tal que $L_{M}=L$.

