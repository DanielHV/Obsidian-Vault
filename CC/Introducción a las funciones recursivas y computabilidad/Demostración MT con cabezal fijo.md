---
fecha : 24-08-2023
---

## Proposición
Toda MT que puede dejar fijo su cabezal es equivalente a una MT que no puede.

#### Demostración
Sea $M = (Q,\Sigma, \Gamma, \delta, q_0,q_a,q_r)$ una MT que puede fijar su cabezal.
Proponemos a $M'=(Q',\Sigma',\Gamma',\delta',q_0',q_a',q_r')$ dada por 
$Q' = Q \cup\{q_{(qi,\sigma,\tau,q_{j})}|\delta(q_{i},\sigma) = (q_j,\tau,S)\}$
$\Sigma' = \Sigma$
$\Gamma' = \Gamma$
$$\delta' = (\delta-\{(q_i,\sigma,(q_j,\tau,S)|q_i,q_{j}\in Q;\sigma,\tau \in \Gamma\}) \ \cup \ \{((q_{i},\sigma),(q_{(q_{i},\sigma,\tau,q_{j})},\tau,R)), ((q_{q_i,\sigma,\tau,q_j}),\eta),(q_j,\eta,L)) \ | $$
$$q_{i},q_{j} \in Q, \sigma \tau, \eta \in \Gamma, \delta_{(q_i,\sigma)}=(q_j,\tau,s)\}$$
Notemos que toda la transición de $M$ también se puede realizar en $M'$ excepto aquellas que fijan al cabezal. Sin embargo, es claro que $uq_{i}\sigma v \vdash_{M'} u\tau q_{(...)}v \vdash_{M'} uq_{j}\tau v$  sustituye a $uq_{i}\sigma v \vdash_{M} uq_{j}\tau v$ en cualquier ejecución de $M'$, luego, toda ejecución de $M$ tiene una ejecución equivalente en $M'$ que termina en la misma config o se cicla si $M$ se cicla.