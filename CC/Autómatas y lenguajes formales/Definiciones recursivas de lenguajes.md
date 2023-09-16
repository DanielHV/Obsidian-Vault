---
fecha : 18-08-2023
---
# Definiciones recursivas de lenguajes

Sea $\Sigma = \{a,b\}$

## Definición 
Sea $L_{1} \subseteq \Sigma^*$ tal que
1. $\epsilon \in L_1$
2. Si $x \in L_{1} \implies xa \in L_{1}$ y $xb \in L_{1}$

$L_{1}= \{\epsilon, a, b, ab, aa, bb, ba, ...\}$
$w = bababa \in L$
$L_{1}= \Sigma^*$


## Definición
Sea $L_{2} \subseteq \Sigma^*$ tal que 
1. $\epsilon \in L_2$
2. Si $x$ es una cadena el $L_{2}\implies axb \in L_2$

$L_{2}= \{\epsilon, ab, aabb, aaabbb, aaaabbbb, ...\}$
$L_{2}= A_{N}B_{N}= \{a^{n}b^{n}|n \in \mathbb{N}\}$


## Definición
Sea $L_{3}\subseteq \Sigma^{*}$ tal que
1. $\epsilon,a,b \in L_3$
2. Si $x \in L_{3} \implies axa \in L_3$ y $bxb \in L_3$

$L_{3}= \{\epsilon, aa, bb, aaaa, bbbb, baab, abba, a, b, aba, bab, ...\}$
$L_{3}= \textrm{Pal}$
$\textrm{Pal} = \{w \in \Sigma^{*}| w^{\mathbb{R}} = w\}$


## Definición
Sea $\Sigma = \{(, \ ), x, y\}$
Se define $L_{4}\subseteq \Sigma^*$ tal que
1. $\epsilon,x,y \in L_4$
2.  $\forall w,v \in L_4, wv \in L_{4}$
3. $\forall w \in L_{4,}(w) \in L_4$

$x,y \in L_4$
$(x), (y), xy \in L_4$
$(xy), (x)xy, xy(y) \in L_4$

$L_{4} = \textrm{Bal}$

