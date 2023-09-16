---
fecha : 30-08-2023
---

$\Sigma = \{a,b\}$

$M_{1} = (Q_{1}, \Sigma, q_{0}, \delta_{1}, A_{1})$


![[Pasted image 20230830102341.png | 550]]


$M_{2} = (Q, \Sigma, p_{0}, \delta_{2}, A_{2})$


![[Pasted image 20230830104107.png | 550]]

###### $M = (Q, \Sigma, r_{0}, \delta, A)$

$Q = Q_{1}\times Q_{2} = \{(q_{i},p_{j}):i,j \in \{0,...,3\}\}$
$r_{0} = (q_{0},p_{0})$
$\delta = Q \times \Sigma \rightarrow Q$
$\delta((q_{i},p_{j}), \sigma) = (\delta_{1}(q_{i},\sigma),\delta_{2}(p_{j}, \sigma))$
$A = \{(q_{i},p_{j}) \in Q : q_{i} \in A_{1} \lor p_{j} \in A_{2}\}$

![[Pasted image 20230830105522.png | 550]]