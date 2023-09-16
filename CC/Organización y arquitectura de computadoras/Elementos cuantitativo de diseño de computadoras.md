---
fecha : 16-08-2023
---
# Elementos cuantitativo de diseño de computadoras
## Binario
Los circuitos electrónicos con los que nuestras computadoras se construyen solo son capaces de distinguir entre dos niveles de voltaje o de carga según el caso, 0 y 1 son los dígitos posibles en un sistema numérico posicional base 2 o binario así que podemos abstraer lo que realmente se almacena y fluye por los circuitos de nuestras computadoras y representar esto mediante un número y por tanto hacer operaciones aritméticas.
Podemos construir funciones lógicas como la conjunción (Y), la disyunción (O), la
implicación, y en general todas las que se expresan en tablas de verdad. A estas les llamaremos funciones de conmutación.
En general, trabajando con n dígitos decimales como variables, se tienen $10^n$ combinaciones. En binario en cambio, si se tienen $n$ variables, el número de combinaciones posibles es 2n. Como la complejidad de un circuito electrónico digital para hacer el cálculo está, en general, en función directa al número de combinaciones que pueden tener los valores de las variables independientes, resulta que la complejidad de los circuitos digitales es menor si estos trabajan en binario.

* Todo lo que queremos hacer se puede hacer en binario.
* La operación de los componentes electrónicos es más confiable.
* Es mucho más simple diseñar los circuitos.


## Transistores
Toda función de nuestro interés, es decir, toda función computable, puede representarse usando sólo ceros y unos para la entrada, para la salida y para especificar las operaciones elementales que la constituyen. Así que nos basta con el conjunto {0, 1} como alfabeto para representarlo todo. 
Usando interruptores es posible calcular cualquier operación de las que conocemos de la lógica proposicional.
Un interruptor puede estar cerrado (dejando fluir la corriente eléctrica), en cuyo caso diremos que está en posición 1, o abierto (impidiendo el paso de corriente) lo que denotaremos como 0. Diremos que un foco puede estar encendido (1) o apagado (0).

$\{\textrm{and, or, not}\} \rightarrow$ conjunto completo de operadores, cualquier función se puede escribir en términos de estos operadores.


## Generaciones de computadores
1. Válvulas de vacío (Bulbos)
2. Transistor
3. Circuitos integrados a baja escala
4. Circuitos integrados a alta escala


## Lenguajes y niveles
Lenguaje de alto nivel $\rightarrow$ Cada instrucción corresponda con varias de lenguaje de máquina
$\downarrow$
Lenguaje de bajo nivel
$\downarrow$
Lenguaje de máquina $\rightarrow$ Para el que fue construida la computadora (UCP)
Lenguaje ensamblador $\rightarrow$ Representación simbólica de lenguaje de máquina


