---
fecha: 4-09-2023
---
# Conceptos semánticos

## Propiedades de las fórmulas considerando estados de las variables
- $\varphi$ es una tautología sii su valor de verdad es `true` para todos los estados $\sigma$
- $\varphi$ es una contradicción sii su valor de verdad es `false`para todos los estados $\sigma$
- $\varphi$ es una contingencia sii su valor de verdad es `true` en algún estado y es `false` en otro estado.

Extendiendo estas definiciones a conjuntos de fórmulas:
$\Gamma = \{\varphi_{1}, \varphi_{2},...,\varphi_{n}\}$

Se dice que $\varphi$ o $\Gamma$ tiene un modelo cuando un estado $\sigma$: $I_{\sigma}(\Gamma) = 1$, i.e, para toda $\varphi_{i} \in \Gamma, I_{\sigma}(\varphi_{i}) = 1$ 
																						$I_{\sigma}(\varphi) = 1$

#### Ejemplo
Sea $\Gamma = \{p \lor q, \ p \rightarrow r, \ q \rightarrow \neg(r \rightarrow p)\}$
			$\gamma_{1}$         $\gamma_{2}$                     $\gamma_{3}$
¿$\Gamma$ tiene un módulo? i.e ¿$\Gamma$ es satisfacible?

Usar la definición de $I_{\sigma}$
Sup. que hay un estado/asignación de las variables $\sigma$ tal que:
a) $I_{\sigma}(\gamma_{1}) = 1$
b) $I_{\sigma}(\gamma_{2}) = 1$
c) $I_{\sigma}(\gamma_{3}) = 1$

Tomando a) hay dos casos ajenos
a.1) $I_{\sigma}(p) = 1$
	$\therefore \sigma(p) = 1$ 
	Entonces para cumplir b) $I_{\sigma}(p \rightarrow r) = 1$ 
	$\therefore \sigma(r) = 1$
	Entonces $I_{\sigma}(r \rightarrow p) = 1$
	$\therefore I_{\sigma}(\neg(r \rightarrow p)) = 0$
	$\therefore$ Para que $I_{\sigma}(\gamma_{3}) = 1$ debe suceder $\sigma(q) = 0$
	Es un modelo para $\Gamma$
ó
a.2) $I_{\sigma}(q) = 1$
	i.e $I_{\sigma}(\gamma_{1}) = 1$
	Entonces para $I_{\sigma}(\gamma_{3}) = 1$
	por def $(r \rightarrow p) = 0$
	por def $I_{\sigma}(r) = 1$ y $I_{\sigma}(p) = 0$
	$\sigma(r) = 1$ y $\sigma(p) = 0$
	Se cumple $I_{\sigma}(\gamma_{2}) = 1$ con $\sigma$
	Es un modelo para $Gamma$
	
a.3) $I_{\sigma}(q) = I_{\sigma}(q) = 1$
	No puede suceder

$\Gamma$ es satisfacible si:
- $\sigma_{1}(p) = 1$, $\sigma_{1}(r) = 1$, $\sigma_{1}(q) = 0$
- $\sigma_{2}(p) = 0$, $\sigma_{2}(r) = 1$, $\sigma_{2}(q) = 1$

##### ¿Que conclusión se puede obtener de $\Gamma$ satisfacible?

$\Gamma = \{p \lor q, \ p \rightarrow r, \ q \rightarrow \neg(r \rightarrow p), \ r, \ r \lor t, \ t \rightarrow r\}$
