---
fecha : 28-08-2023
---
# Semántica formal de LPROP
- ##### Tablas de verdad
	Renglones: combinaciones de los posibles estados de todas las variables de una fórmula ($2^n$).
	Observación: Hay $2^{4}= 16$ conectivos binarios diferentes.

"Recupera los renglones importantes de las tablas".

Dada unas fórmulas $\varphi_1$ y $\varphi_2$ el valor de verdad de:
- $\neg \varphi_1$ es verdadero sii $\varphi_1$ es falso.
- $\varphi_{1}\land \varphi_{2}$ es verdadero si $\varphi_1$ y $\varphi_2$ son verdaderos.
- $\varphi_{1} \lor \varphi_{2}$ es falsa sii $\varphi_{1}$ y $\varphi_2$ son falsas.
- $\varphi_{1} \rightarrow \varphi_{2}$ es falsa sii $\varphi_{1}$ es verdadera y $\varphi_{2}$ es falsa.
- $\varphi_{1}$ es verdadera sii $\varphi_1$ y $\varphi_2$ tienen el mismo valor.
- Si $\varphi_1$ es una fórmula atómica: 
	- $\bot$ es falsa.
	- $\top$ es verdadera.
	- $p \in \textrm{Var}$ puede ser verdadera o falsa (se debe establecer un estado).

El estado $\sigma :: \textrm{Var} \rightarrow \textrm{Bool}$  es una asignación de valores de verdad a cada variable de una fórmula.
###### Ejemplo
$\varphi = \neg p \land q \rightarrow (r \leftrightarrow t \lor s)$
$vars(\varphi) = 5$, $2^5$ estados diferentes.
$\sigma_{1}(p)= 1$
$\sigma_{1}(q) = 0$
$\sigma_{1}(r)=0$
$\sigma_{1}(s)=1$
$\sigma_{1}(t)=1$

Dado un estado, la interpretación $I_{\sigma_{1}}$ de una fórmula se obtiene al aplicar la definición de semántica formal.

$I_{\sigma_{1}} = 0$ sii
1) $I(\neg p \land q) = 1$  
2) $I_{\sigma_{1}}(r \leftrightarrow t \lor s) = 0$

 De 1) y por definición $I_{\sigma_{1}}(\neg p) = 1$ y y $L_{\sigma_{1}}(q) = 1$, pero no puede suceder ya que $\sigma_{1}(q) = 1$.
 $\therefore I_{\sigma_{1}}(\neg p \land q) = 0$
 $\therefore I_{\sigma_{1}}(\varphi) = 1$

**Demostración a partir de $\sigma_1$ y usando la definición de semántica formal**
$I_{\sigma_{1}}(\neg p) = 0$
$\implies I_{\sigma_{1}}(\neg p \land q) = 0$ sin importar $I_{\sigma_{1}}(q)$ para cualquier $\sigma$
$\therefore I_{\sigma_{1}}(\varphi) = 1$ 

**Análisis $\varphi$ para buscar un estado $\sigma'$ tal que $I_{\sigma_{1}}(\varphi)=0$**
Deben de suceder:
1) $I_{\sigma'}(\neg p \land q) = 1$
	Por definición $I_{\sigma'}(\neg p) = 1$ y $I_{\sigma'}(q) = 1$
	$\therefore \sigma'(p) = 0$
	$\therefore \sigma'(q) = 1$
	
2) $I_{\sigma_{1}}(r \leftrightarrow t \lor s) = 0$
	Por definición $I_{\sigma'}(r) \neq I_{\sigma'}(t \lor s) = 0$
	

..........
![[IMG_6983.heic]]
	

