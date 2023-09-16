---
fecha : 23-08-2023
---
El gerente de un parque nacional determina que el parque puede sostener a 65 coyotes.
Si suponemos que la tasa de cambio de la cantidad de coyotes $N$ es directamente proporcional a la diferencia entre la población máxima y la población actual.
¿Cual es su modelo matemático?
¿Y su solución?

$\frac{dN}{dt}=K(65-N)$ 
$U = (65-N)$
$du = dN$

$$\int \frac{dN}{(65-N)} = \int kdt$$
$$\int \frac{-du}{u} = \int kdt$$
$$-ln(65-N) = KT+C$$
$$ln(65-N) = -KT-C$$
$$65-N = e^{-KT}e^{-c}$$
$$65-N = Ce^{-KT}$$
$$N = Ce^{-KT}+65$$





$$