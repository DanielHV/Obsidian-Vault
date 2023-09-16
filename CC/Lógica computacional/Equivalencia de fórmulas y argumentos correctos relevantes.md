---
fecha: 11-09-2023
---

# Equivalencia de fórmulas

$\varphi_{1} \equiv \varphi_{2} \iff \varphi_{1} \models \varphi_{2} \ \& \ \varphi_{2} \models \varphi_{1}$

$\varphi_{1} \rightarrow \varphi_{2} \equiv \neg \varphi_{1} \lor \varphi_{2}$

$\neg \varphi_{1} \lor \neg \varphi_{2} \equiv \neg(\varphi_{1} \land \varphi_{2})$

$\neg \varphi_{1} \land \neg \varphi_{2} \equiv \neg(\varphi_{1} \lor \varphi_{2})$


# Argumentos correctos relevantes
Esquemas deductivos bien conocidos
###### Modus ponens
$\varphi_{1} \rightarrow \varphi_{2}$
$\varphi_{1}$
$\therefore \varphi_{2}$

###### Modus tollens
$\varphi_{1} \rightarrow \varphi_{2}$
$\neg \varphi_{2}$
$\therefore \neg \varphi_{1}$

###### Dilema constructivo
$\varphi_{1} \rightarrow \varphi_{2}$
$\varphi_{3} \rightarrow \varphi_{4}$
$\varphi_{1} \lor \varphi_{3}$
$\therefore \varphi_{2} \lor \varphi_{4}$

###### Resolución binaria
$\varphi_{1} \lor \varphi_{2}$
$\neg \varphi_{2} \lor \varphi_{3}$
$\therefore \varphi_{1} \lor \varphi_{3}$

##### Formas normales
Toda fórmula se puede transformar en cláusulas (conjunciones de disyunciones de literales ($ATOM$ o $\neg ATOM$))

# Equivalencia de fórmulas para lógica clausular
Obtener equivalencias en cierto orden para obtener cláusulas.

1. Transformar cualquier fórmula $\varphi$ en una que tenga el patrón Forma Normal Negativa
	$FNN(\varphi)$ cumple con:
	- $\varphi$ no tiene $\rightarrow$ ni $\leftrightarrow$
	- Las negaciones solo aparecen a fórmulas atómicas.
	Equivalencias usadas para obtener $FNN$
	$\varphi_{1} \rightarrow \varphi_{2} \equiv \neg \varphi_{1} \lor \varphi_{2}$
	$\varphi_{1} \leftrightarrow \varphi_{2} \equiv (\varphi_{1} \lor \varphi_{2}) \land (\neg \varphi_{2} \lor \varphi_{1}) \equiv (\varphi_{1} \land \varphi_{2}) \lor (\neg \varphi_{1} \land \neg \varphi_{2})$
	$\neg (\neg \varphi) \equiv \varphi$
	$\neg (\varphi_{1} \land \varphi_{2}) \equiv \neg \varphi_{1} \lor \neg \varphi_{2}$
	$\neg (\varphi_{1} \lor \varphi_{2}) \equiv \neg \varphi_{1} \land \neg \varphi_{2}$
	$\neg(\varphi_{1} \rightarrow \varphi_{2}) \equiv \varphi_{1} \land \neg \varphi_{2}$
	 XOR $\neg(\varphi_{1} \leftrightarrow \varphi_{2}) \equiv (\varphi_{1} \land \neg \varphi_{2}) \lor (\neg \varphi_{1} \land \varphi_{2})$

2. Obtener cláusulas (disyunción de literales ($ATOM$ o $\neg ATOM$))
	Transformar cualquier fórmula $\varphi$ en una que contenga cláusulas.
	Forma Normal Clausular

	$ATOM ::= \top | \bot | \textrm{Vars}$
	$Lit ::= ATOM | \neg ATOM$
	$C ::= Lit | Lit \lor C$
	$LPROP \ \varphi ::= C | C \land \varphi$
	 