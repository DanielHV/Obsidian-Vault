# Resolución binaria
Método de demostración para decidir la correctitud de argumentos lógicos.

### Refutación 
Buscar un modelo de $\Gamma \cup \{\neg \varphi\}$

### Resolución
$C_{1}\lor l$
$C_{2}\lor l^{c}$
$C_{1}\lor C_{2}$

$l$ una literal (atómica, negación de atómica)
$l^{c}$ la misma literal contraria (negada)
$C_{i}$ cláusula: disyunción de literales usando equivalencias
1. FNN
2. FNC


##### Ejemplo
$\gamma_{1} \ \neg(p \rightarrow r)$
$\gamma_{2} \ p \rightarrow q \rightarrow r$
$\neg \varphi \ \therefore q \rightarrow p \land r$

1. Transformar las formulas del argumento en cláusulas
	FNN
	$\gamma_{1} \equiv p \land \neg r$
	$\gamma_{2} \equiv \neg p \lor (\neg q \lor r)$
	$\neg \varphi \equiv q \land (\neg p \lor \neg r)$
2. Aplicar resolución de las cláusulas
	FNC
	Obs. separar conjunciones
	$\eta_{1} \ p$
	$\eta_{2} \ \neg r$ 
	$\eta_{3} \ \neg p \lor \neg q \lor r$
	$\eta_{4} \ q$
	$\eta_{5} \ \neg p \lor \neg r$
	$_{6} \ \neg p \lor \neg q$ Res 3,5
	$_{7} \ \neg q$ Res 1,6
	$_{8} \ \blacksquare$ Res 4,7

¿Qué pasa cuando no se llega a la cláusula vacía?
No sabemos si $\Gamma \cup \{\neg \varphi\}$ tiene un modelo.

Entonces hay que programarlo (Saturación (aplicar resolución sobre todas las cláusulas)).


