# Consecuencia lógica

$\models_{\sigma}\varphi$, $\sigma$ es un modelo de $\varphi$
$\Gamma \models \varphi$ , $\varphi$ es consecuencia lógica de $\Gamma$
$\Gamma \vdash \varphi$, info $\vdash$ conclusión 
$\land \Gamma \rightarrow \varphi$, Si $I_{\sigma}(\Gamma) = 1$ entonces $I_{\sigma}(\varphi) = 1$, cada modelo de $\Gamma$ también satisface a $\varphi$
$I_{\sigma}(\Gamma) = 0$ "$\Gamma$ es inconsistente" cuando al menos una $\gamma_{i}$ es falsa en $\sigma$

## Propiedades
- Si $\varphi \in \Gamma$ entonces $\Gamma \models \varphi$
- Método de demostración por refutación: $\Gamma \models \varphi$ sii buscar que $\Gamma' = \Gamma \cup \{\neg \varphi\}$ no tiene un modelo (es insatisfacible)
- $\Gamma \models \varphi_{1} \rightarrow \varphi_{2}$ sii $\Gamma \cup \{\varphi_{1}\} \models \varphi_{2}$
- Si $\Gamma$ es insatisfacible, se puede cumplir cualquier $\varphi$    $0 \implies 1 / 0$
- $\varnothing \models \varphi$, $\varphi$ es una tautología
- $\varphi_{1} \models \varphi_{2}$ y $\varphi_{2} \models \varphi_{1}$ entonces $\varphi_{1} \equiv \varphi_{2}$ 

#### Ejemplo
uncurry:
$f:A \times B \rightarrow C$
$f(a,b)=c$

curry:
$g : A \rightarrow B \rightarrow C$
$f$ ~ $g$

P.D $(\varphi_{1} \land \varphi_{2}) \rightarrow \varphi_{3} \equiv \varphi_{1} \rightarrow (\varphi_{2} \rightarrow \varphi_{3})$
Dem
$\Rightarrow) (\varphi_{1} \land \varphi_{2}) \rightarrow \varphi_{3} \models \varphi_{1} \rightarrow (\varphi_{2} \rightarrow \varphi_{3})$
$\Leftarrow) \varphi_{1} \rightarrow (\varphi_{2} \rightarrow \varphi_{3}) \models (\varphi_{1} \land \varphi_{2})\rightarrow \varphi_{3}$


$\Rightarrow)$ Usando la prop 3 de consecuencia lógica
$\varphi_{1} \land \varphi_{2} \rightarrow \varphi_{3} \models \varphi_{1} \rightarrow \varphi_{2} \rightarrow \varphi_{3}$ es equivalente (x2)
$\varphi_{1} \land \varphi_{2} \rightarrow \varphi_{3}, \varphi_{1}, \varphi_{2} \models \varphi_{3}$
Suponer que hay un $\sigma$ estado que satisface al contexto

a) $I_{\sigma}(\varphi_{1} \land \varphi_{2} \rightarrow \varphi_{3}) = 1$
b) $I_{\sigma}(\varphi_{1})=1$
c) $I_{\sigma}(\varphi_{2})=1$

PD  
$I_{\sigma}(\varphi_{3})=1$
Se cumple por def

$\Leftarrow)...$
