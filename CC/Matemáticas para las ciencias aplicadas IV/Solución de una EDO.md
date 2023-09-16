---
fecha : 18-08-2023
---

La solución de una EDO es una función que satisface la ecuación
Al sustituir esta función en la EDO, se tiene una afirmación de la respuesta
$\frac{dB}{dt}=KB$
$K>0$ constante

### Problema
Un saldo bancario al cabo de $t$ años a un interés compuesto.

$B(t)?$
$ae^{kt}$ solución general propuesta
$\implies \frac{d(ae^{kt})}{dt}$
$= ake^{kt}$
$= k (ae^{kt})$
$B(t) = (ae^{kt})$

Si $t=0 \implies B(0) = ae^{k(0)} = a$ (monto inicial)
$\implies B(t) = B(0)e^{kt}$

Hay tantas soluciones para la ecuación diferencial como $t$, y como $a$
 
## Una solución de EDO
$F(x,y,y',y'',y''',...,y^{n-1},y^{n})=0$ (Solución en general)
$y^{n}= G(x,y,xy',...,y^{n-1})$

en un intervalo $(a,b)$ es una función real $y=y(x)$ tal que existen todas las derivadas necesarias de $y(x)$ en ese intervalo
Entonces $y(x)$ satisface la ecuación para cada valor de $x$ en el intervalo.

Resolver una EDO es encontrar todas las soluciones posibles de la misma.


Hernández Vela Daniel
#### Actividad 1
$x(t) = 5e^{3t}-7e^{2t}$
$x' = 15e^{3t}-14e^{2t}$
$x'' = 45e^{3t} -28e^{2t}$

$\textrm{sustituyendo en x''-5x'+6x=0:}$

$(45e^{3t} -28e^{2t}) - 5(15e^{3t}-14e^{2t}) + 6(5e^{3t}-7e^{2t}) = 0$
$45e^{3t} -28e^{2t} + 75e^{3t}-70e^{2t} + 30e^{3t}-42e^{2t} = 0$
$(45e^{3t}-75e^{3t}+30e^{3t}) + (-28e^{2t} + 70e^{2t} -42e^{2t})$ = 0
$(75e^{3t}-75e^{3t}) + (70e^{2t} - 70e^{2t}) = 0$
$0 + 0 = 0$
$\therefore \textrm{se cumple la igualdad}$ 

