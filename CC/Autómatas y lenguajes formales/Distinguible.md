---
fecha : 31-08-2023
---
## Definición
Si $L \subseteq \Sigma^{*}, \ x,y \in \Sigma^{*}$ decimos que $x$ y $y$ son $L-$distinguibles si existe $z$ tal que exactamente una de las cadenas $xz$ y $yz$ está en $L$.
Si $L/x=\{z \in \Sigma^{*} | xz \in L\}$ entonces $x$ y $y$ son $L-$distinguibles.
Decimos que $x$ y $y$ son $L-$indistinguibles si $L/x = L/y$.

Si $S \subseteq \Sigma^{*}$ decimos que las cadenas en $S$ son $L-$distinguibles dos a dos si para cada $x,y \in S$,  $x \neq y$, $x$ y $y$ son $L-$distinguibles sí y solo sí $L/x \neq L/y$.

## Proposición
Sea $L \subseteq \Sigma^{*}$ un lenguaje, si $x,y \in \Sigma^{*}$ son $L-$distinguibles y $M = (Q,\Sigma,q_0,\delta,A)$ es un AFD que reconoce a $L$, entonces $\delta^{*}(q_{0},x) \neq \delta^{*}<(q_{0},y)$. Por lo tanto, para cada $n \in \mathbb{Z}^{+}, n≥z$, si existe un subconjunto $S$ de $\Sigma^{*}$ tal que sus cadenas son $L-$distinguibles dos a dos y $|S|=n$, entonces $M$ tiene al menos $n$ estados.

### Demostración
Como $x$ y $y$ son $L-$distinguibles entonces existe $z \in \Sigma^{*}$ tal que solo una de $xz$ y $yz$ está en $L$. Es decir, solo uno de los estados $d^{*}(q_{0},x)$ y $\delta^({*}q_0,yz)$ está en $A$. Así, $\delta^{*}(q_{0},xz) \neq \delta^{*}(q_0,yz)$.
Pero, $\delta^{*}(q_{0},xz) = \delta^{*}(\delta^{*}(q_{0},x),z) \neq \delta^{*}(q_{0},xy) = \delta^{*}(\delta^*(q_{0},y),z)$. Se sigue de la primera obs por el principio de la pichonera.
Por lo tanto $\delta^{*}(q_{0},x) \neq \delta^{*}(q_{0},y)$

## Corolario
Sea $L \subseteq \Sigma^{*}$, si existe un subconjunto $S$ de $\Sigma^{*}$ infinito de cadenas $L-$distinguibles 2 a 2, entonces no existe un AFD que la reconozca.
### Demostración
Para cada $n \in \mathbb{Z}^{+}, \ n≥z$, existe un subconjunto de $S$ de cardinalidad $n$ de cadenas $L-$distinguibles dos a dos. Por la proposición anterior si existe un AFD que reconozca a $L$, tendrá al menos $n$ estados para cada $n \in \mathbb{Z}^{+}$, lo que resulta imposible.
