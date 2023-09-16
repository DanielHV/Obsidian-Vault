---
fecha : 17-08-2023
---

$L_1 = \{w\#w \ | \ w \in \{a,b\}^*\}$

$M_1 =$ Con entrada unan cadena $w$.
1. Recorre hacia adelante y hacia atrás los caracteres de $w$ comparando aquellos a la izquierda de $\#$ y en la misma posición a la derecha de $\#$. Si no encuentra $\#$ o los símbolos no coinciden, rechaza. De otro modo los marca con un símbolo especial.
2. Cuando todos los símbolos a la izquierda de $\#$ hayan sido marcados, revisa si todos los símbolos a la derecha han sido marcados. En caso positivo, acepta $w$, y en otro caso, rechaza.

# Máquina de Turing

## Definición
Una **máquina de Turing** (MT) es una septeta ordenada $(Q,\Sigma,\Gamma,\delta,q_0,q_a,q_r)$ donde:
1. $Q$ es un conjunto finito y no vacío de "estados".
2. $\Sigma$ es un alfabeto tal que $\square \notin \Sigma$, llamado el alfabeto de entrada.
3. $\Gamma$ es un alfabeto tal que $\square \in \Gamma$, y $\Sigma \subseteq \Gamma$, llamado el alfabeto de cinta.
4. $\delta:Q\times \Gamma \rightarrow Q \times \Gamma \times \{L,R\}$ (la función de transición).
5. $q_0 \in Q$ es el estado inicial.
6. $q_a \in Q$ es el estado de aceptación.
7. $q_r \in Q, q_r \neq q_a$, es el estado de rechazo.

Una MT recibe su entrada $w$ en una cinta infinita donde las primeras $|w|$ celdas contienen a $w$ y el resto de la cinta contiene $\square$, es decir, está en blanco. Tiene un cabezal de lectura y escritura que inicialmente apunta a la primera posición de la cinta (la más a la izquierda) y se mueve de acuerdo a la función de transición. Si el cabezal se encuentra en la primera posición y la función de transición indica $L$ (moverse hacia la izquierda), el cabezal se queda en la misma posición.