---
fecha : 17-08-2023
---
# Lenguajes

Si $w$ es una cadena sobre $\Sigma$ y $\sigma \in \Sigma$, el número de ocurrencias de $\sigma$ en $w$ se denota por $n_\sigma(w)$.

Si $\Sigma$ es un alfabeto, un lenguaje $L$ sobre $\Sigma$ es un subconjunto de $\Sigma^*$. 

Si $\Sigma$ es un alfabeto, e $i \in \mathbb{N}$, el lenguaje $\Sigma^*$ consta de todas las cadenas de longitud $i$ sobre $\Sigma$.

El orden canónico para un lenguaje $L$ es aquel que enumera a todas las cadenas en $\Sigma^i$ antes que todas las cadenas en $\Sigma^j$ si $i<j$ y las cadenas de $\Sigma^i$ son enumeradas lexicográficamente.
$\{a,b\}^* = \{ \epsilon, a, b, aa, ab, ba, bb, aaa, aab, ...\}$

Si $\Sigma$ es un alfabeto, $\emptyset$, $\Sigma$ y $\Sigma^*$ siempre son lenguajes sobre $\Sigma$.
$\Sigma^i = \{w \in \Sigma^* \ | \ |w|=i\}$ 
$L_i=\{w \in \{a,b\}^*|n_a(w)=n_b(w)\}$ 

$|\Sigma^i| = |\Sigma|^i$ 
Como $\Sigma^*= \bigcup_{i \in \mathbb{N}} \Sigma^i$, concluimos que $|\Sigma^*|=\aleph_0$

¿Cuantos lenguajes sobre $\Sigma$ hay? 
$|\mathcal{P}(\Sigma^*)| = 2^{\aleph_0}$ 


Como los lenguajes son conjuntos podemos aplicar operaciones conjuntistas sobre lenguajes, en particular si $L_1$ y $L_2$ son lenguajes sobre $\Sigma$, $L_1 \cup L_2$, $L_1 \cap L_2$, $L_1 \setminus L_2$ también lo son.
Podemos definir $L_1 \circ L_2 = L_1L_2$ de la siguiente manera:
$$
L_1L_2=\{w_1w_2|w_1 \in L_1, w_2\in L_2 \}
$$
## Definición
Si $L$ es un lenguaje sobre $\Sigma$, definimos
1. $L^0 = \{\epsilon\}$
Si $L^n$ está definido para $n \in \mathbb{N}$,
2. $L^{n+1}=L^nL$

##### Nota
$\varnothing \neq \{\epsilon\}$ 
$\varnothing L = L \varnothing = \varnothing$ 

## Definición
Si $L$ es un lenguaje sobre $\Sigma$, la estrella de Kleene de $L$, $L^*$ está dada por
$$
L^* = \bigcup_{i \in \mathbb{N}} L^i
$$
$L^+ = L^*L$ 
$\varnothing^* = \{\epsilon\} = \varnothing L^0$  
