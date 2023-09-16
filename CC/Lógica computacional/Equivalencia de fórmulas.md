---
fecha: 6-09-2023
---

# Equivalencia de fórmulas

Dado un conjunto de fórmulas $\Gamma = \{\gamma_{1}, \gamma_{2},...,\gamma_{n}\}$ (base de conocimiento/contexto) decidir si otra (una) fórmula se sigue/se obtiene como conclusión.

Del contexto $\Gamma$ se puede concluir/deducir $\varphi$
Se puede pensar como $\gamma_{1} \land \gamma_{2}\land...\land \gamma_{n} \rightarrow \varphi$

Usando semántica formal buscar un modelo para $\Gamma$ ($\Gamma$ es consistente)y que ese mismo modelo satisfaga a $\varphi$.
Dado un estado de las variables $\sigma$, si $I_{\sigma}(\Gamma) = 1$ entonces $I_{\sigma}(\varphi) = 1$

Obs:
$I_{\sigma}(\Gamma) = 0$ i.e al menos hay una $\gamma_{i}$ tal que $I_{\sigma}(\gamma_{i})=0$
$\therefore$ el argumento es correcto

- formula (tautología/contradicción/contingencia)
- conjunto de fórmulas (consistente/inconsistente)
- argumento (correcto/incorrecto)

Correctitud: Para todo modelo de $\Gamma$ ese también es modelo de $\varphi$
