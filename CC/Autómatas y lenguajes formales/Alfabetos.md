---
fecha: 15-08-2023
---
### Cardinalidad
$|\mathbb{N}| = \aleph_0$
$|\mathbb{N} \times \mathbb{N}| = \aleph_{0} = |\mathbb{Z}|$
$\mathbb{N}^{2}= \mathbb{N}\times\mathbb{N}$
$|\mathbb{N}^{3}| = |\mathbb{N}\times\mathbb{N}\times\mathbb{N}| = \aleph_0$
$|\mathbb{N}^{\mathbb{N}}| = 2^{\aleph_0}$

#### Proposición
Un conjunto es numerable si es biyectable con $\mathbb{N}$.

#### Proposición
Un conjunto es contable si es finito o numerable.

#### Proposición
(Participación)
Toda unión numerable de conjuntos contables es contable.

##### CSB (Teorema de Cantor)
Sean $A$ y $B$ conjuntos, si existen funciones inyectivas de $A$ en $B$ y de $B$ en $A$, entonces $A$ y $B$ son biyectables.

$|\mathbb{N}| = |\mathbb{Z}| = |\mathbb{Q}| \neq |\mathbb{R}|$


# Alfabetos

## Definición
Un **[[Problemas de decisión, alfabetos y lenguajes|alfabeto]]** es un conjunto finito no vacío.
Un **símbolo** es un elemento de un alfabeto.

## Definición
Una **cadena** sobre un alfabeto $\Sigma$ es una sucesión finita de elementos de $\Sigma$.
i.e. $w : \{0,...,n\} \rightarrow \Sigma$
o $w \cdot \emptyset \rightarrow \Sigma$ 

Hay una única cadena vacía que denotamos por $\epsilon$.
Si $w:s \rightarrow \Sigma$ es una cadena, entones la longitud de $w$, $|w|$, se define por $|w|=|s|$, i.e., es la longitud de $w$ como sucesión.

###### Ejemplo
$\Sigma = \{a,b\}$
$w=\mathrm{baba} = w_0w_1w_2w_3$
$w_{0}= w(0) = b = w(2) =w_2$
$w:1 = w(1) = a = w(3) = w_3$

## Definición
Si $w_1$ y $w_2$ son cadenas sobre el alfabeto $\Sigma$, la **concatenación** de $w_1$ y $w_2$ es la cadena $w_{1}\circ w_{2}$ ($w_1w_2$) e
$(w_1w_2)_j = (w_1)_j$  si $j\in\{0,...,|w_1|-1\}$ 
$(w_1w_2)_{|w_{1|+j}} = (w_2)_j$ si $j \in \{0,...,|w_2|-1\}$

## Definición
Si $v$ y $w$ son cadenas sobre $\Sigma$ decimos que:
1. $v$ es subcadena de $w$ si existen cadenas $x$ y $y$ sobre $\Sigma$ tales que $w=xuy$ ($x$ y $y$ pueden ser $\epsilon$).
2. $v$ es sufijo de $w$ si existe una cadena $x$ sobre $\Sigma$ tal que $w=xv$.
3. $v$ es prefijo de $w$ si existe $y$ una cadena sobre $\Sigma$ tal que $w=vy$.