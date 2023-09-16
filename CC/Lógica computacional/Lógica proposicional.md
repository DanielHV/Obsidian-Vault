---
fecha : 22-08-2023
---
[Lógica proposicional](onenote:https://comunidadunammx-my.sharepoint.com/personal/daniel278_comunidad_unam_mx/Documents/4º%20semestre/Lógica%20computacional.one#Lógica%20proposicional&section-id={C7134C4D-60FD-FA47-A79F-D3FCAB68C528}&page-id={F05A5C3E-E869-2F4C-AE9D-C64AB51F9BD3}&end)  ([Vista web](https://comunidadunammx-my.sharepoint.com/personal/daniel278_comunidad_unam_mx/_layouts/OneNote.aspx?id=%2Fpersonal%2Fdaniel278_comunidad_unam_mx%2FDocuments%2F4%C2%BA%20semestre&wd=target%28L%C3%B3gica%20computacional.one%7CC7134C4D-60FD-FA47-A79F-D3FCAB68C528%2FL%C3%B3gica%20proposicional%7CF05A5C3E-E869-2F4C-AE9D-C64AB51F9BD3%2F%29))

# Lógica proposicional

## Sintaxis (gramática BNF / Inductiva)

$P ::= Var  \ | \  \top \ | \ \bot \ | \ \neg \mathbb{P} \ | \ \mathbb{P}\diamond\mathbb{P} \ | \ (\mathbb{P})$} 
$Var ::= p \ | \ q \ | \ r \ | \ s \ | \ t \ | ... | \ p_{1}\ | \ p_{2} \ | ...$
Símbolos binarios  $\diamond ::= \land \ | \ \lor \ | \ \rightarrow \ | \ \leftrightarrow$
## Semántica
1. Cualquier variable proposicional $p \in Var$ puede ser verdadera o falsa.
2. Las constantes de verdad ($\top$ verdadera, $\bot$ falsa).
3. Si $\mathbb{P}$ y $\mathbb{P'}$ son fórmulas:
	* $\mathbb{P} \land \mathbb{P'}$ es verdadera sí y solo sí $\mathbb{P}$ y $\mathbb{P'}$ son verdaderas.
	* $\mathbb{P} \lor \mathbb{P'}$ es falsa sí y solo sí $\mathbb{P}$ y $\mathbb{P'}$ son falsas.
	* $\mathbb{P} \rightarrow \mathbb{P'}$ es falsa sí y solo sí $\mathbb{P}$ es verdadera y $\mathbb{P'}$ es falsa.
	* $\mathbb{P} \leftrightarrow \mathbb{P'}$ es verdadera sí y solo sí $\mathbb{P}$ y $\mathbb{P'}$ tienen el mismo valor.
4. $\neg\mathbb{P}$ es verdadera sí y solo sí $\mathbb{P}$ es falsa.
## Precedencia y asociatividad de operadores
Se define la siguiente precedencia de operadores de mayor a menor:
* $\neg$
* $\land$, $\lor$
* $\rightarrow$
* $\leftrightarrow$
Obsérvese que los operadores $\land$, $\lor$ tienen la misma precedencia de manera que expresiones como $p \land q \lor r$ son ambiguas y no pueden ni deben ser utilizadas.
Acerca de la asociatividad, los operadores $\land$, $\lor$, $\leftrightarrow$ son asociativos de manera que expresiones como $p \lor q \lor r$, o $\neg p \leftrightarrow p \lor s \leftrightarrow t$ están libres de ambigüedades.
Por otra parte el operador $\rightarrow$ no es asociativo pero se adopta la convención usual de asociarlo a la derecha, es decir expresiones del estilo $\varphi_{1} \rightarrow \varphi_{2} \rightarrow \varphi_{3}$ se entenderán como $\varphi_{1} \rightarrow (\varphi_{2} \rightarrow \varphi_{3})$.