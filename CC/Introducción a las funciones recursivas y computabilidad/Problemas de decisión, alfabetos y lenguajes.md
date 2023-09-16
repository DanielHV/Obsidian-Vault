---
fecha : 15-08-2023
---
# Problema de decisión
1. Definir una entrada
2. Pregunta sobre la entrada cuya respuesta sea sí o no.
##### Ejemplo
###### Primo:
I) Un número entero positivo $n$.
Q) ¿Es un número primo?

###### Stable:
I) Una gráfica $G$ y un entero $k≥0$.
Q) ¿Existe un conjunto independiente de al menos $k$ vértices en $G$.

###### MaxStable:
I) Una gráfica $G$.
Q) Encontrar un conjunto independiente máximo en $G$.

## Definición
Un **[[Alfabetos|alfabeto]]** es un conjunto finito no vacío. Si $\Sigma$ es un alfabeto, cada elemento de $\Sigma$ es un **símbolo**.

## Definición
Si $\Sigma$ es un alfabeto, una cadena $w$ sobre $\Sigma$ es una sucesión finita de elementos de $\Sigma$.
i.e. para algún $n\in\mathbb{N}$, $w:\{0,...,n\}\rightarrow \Sigma$.
La longitud de la cadena $w$, $|w|$, es la cardinalidad de su dominio.
Hay una única cadena de longitud 0, la cadena vacía, que se denota por $\epsilon$.

##### Ejemplo
Si $\Sigma=\{a,b\}$
$w=\textrm{baba}$ 
$w:\{0,1,2,3\} \rightarrow \{a,b\}$ 
$w_{0}= w(0) = b = w(2) = w_{2}$
$w_{1}= w(1) = a = w(3) = w_{3}$

## Definición
Si $\Sigma$ es un alfabeto, el conjunto de todas las cadenas sobre $\Sigma$ se denota por $\Sigma^*$.

## Definición
Un lenguaje sobre el alfabeto $\Sigma$ es un subconjunto de $\Sigma^*$.

Los problemas de decisión son subconjuntos de $\Sigma *$
Los algoritmos son elementos de $\Sigma^*$

Existen problemas de decisión que no se pueden resolver algorítmicamente.

