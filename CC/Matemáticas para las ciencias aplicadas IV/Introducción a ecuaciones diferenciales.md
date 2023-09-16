---
fecha : 16-08-2023
---
# Ecuaciones diferenciales

## Sirven para:
* Razones de cambio
* El seguimiento de la rapidez con la que llega a manifestarse el SIDA en los pacientes con VIH positivo
* La dinámica de oferta y demanda en un sistema económico
* Interacción entre 2 o más especies animales en una localidad

## EDO (Ecuación diferencial ordinaria)
###### Ejemplo:
$3\frac{dy}{dt}=y$

### Notación de Newton
$\ddot x + 3t\dot x + 3x = Sen(wt)$

### Orden de una EDO
El orden depende de la derivada de mayor grado
###### Ejemplo:
$\frac{dy}{dx}+2xy=e^{-x^{2}}$ (Primer orden)
$\ddot x(t) - 5 \dot x(t) + 6x(t) = 0$ (Segundo orden)
$\frac{d^2x}{dt}-5\frac{dx}{dt}+6x=0$ (Segundo orden)

### Forma general de una EDO
Si $y(x)$, $x$ es la variable independiente.
Entonces una EDO de orden $n$ se puede expresar:
$F(x,y,y',y'',...,y^{n-1}) = 0$
$y^n = G(x,y,y',y'',...,y^{n-1})$

### Ecuación diferencial en derivadas parciales
$\frac{\partial^2u}{\partial x^2} \cdot \frac{1}{c^2} \frac{\partial^2u}{\partial t^2} = 0$
Ecuación de onda. $U(x,t)=u$

### EDO lineales y no lineales
$a_n(x)y^n + a_{n-1}(x)y^{n-1} + ... + a_1(x)y' + a_0(x)y=f(x)$
$a_n(x)$, $a_{n-1}(x)$, ..., $a_0$ y $f(x)$ son funciones de $x$.

*Cada función coeficiente $a_i(x)$ debe depender únicamente de la variable independiente $x$ y no contiene a la variable dependiente ni cualquiera de sus derivadas.*

###### Ejemplo
$1x''+3tx'+2x=Sen(wt)$
$\downarrow$
$x''(t)+3tx'(t)+2x(t)$
Variable independiente: $t$
Variable dependiente: $x$

$\frac{d^2x}{dt} + 3t\frac{dx}{dt} + 2x = Sen(wt)$
Modelo para la infección del VIH