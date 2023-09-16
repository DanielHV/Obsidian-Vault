---
fecha : 18-08-2023
---
# Introducción

## Triada de la seguridad

### Confidencialidad
La información solo puede ser visualizada por aquellos con permisos de visualizarla.

### Integridad
La información no sufre alteraciones desde su generación hasta su consumo.

### Disponibilidad
La información debe estar disponible cuando se requiera.


## El papel de la criptografía en la actualidad
Cubre un amplio campo de necesidades básicas
* Autenticación
* No repudio
* Firmas digitales
* Integridad
* Confidencialidad

La base en divergencias tecnológicas
* Blockchains
* Votación electrónica
* Adversarial Machine Learning


## ¿De donde viene la criptografía?
* Ocultar información es una necesidad humana
	* Guerras, persecución política, secretos de estado, información financiera, entre otros.

###### Ejemplo
* Atbash: se invierte el abecedario
* ROT13: se utiliza para "censurar" información en foros, TV, radio, etc.
	* Dado un mensaje $M=\{m_1,m_2,m_3,...m_n\}$
	* $C=\{m_i+13mod26 | m_{i} \in M \}$

> Google dorks

## Distintos tipos de cifrado
* Simple substitution
* Key addition
* Codebook
* Transposition
* Electromechanical machine

### Estandarización de la criptografía
* NIST
* Chinese State Cryptographic Authority
* National Standard of the Russian Federation


# Principio de Kerckhoffs
*Auguste Kerckhoffs (1883) - La Cryptographie Militaire*
1. Si el sistema no es teóricamente irrompible, al menos debe serlo en la práctica.
2. La efectividad del sistema no debe depender de que su diseño permanezca en secreto.
3. La clave debe ser fácilmente memorizable de manera que no haya que recurrir a notas escritas.
4. Los criptogramas deberán dar resultados alfanuméricos.
5. El sistema debe ser operable por una única persona.
6. El sistema debe ser fácil de utilizar.


## Modelos de ataque
* KPA (Known Plaintext Attack)
* KCA (Known Ciphertext Attack)
* CPA (Chosen Ciphertext Attack)
* CCA (Chosen Ciphertext Attack)
* Differential cryptanalysis
* Side Channel Attacks
* Code Analysis


## Security Goals
### Indistiguishability (IND)
Que no exista manera de identificar la relación entre un texto y su equivalente cifrado

### Non-maleability
Dado un teto cifrado $C_1$ debe ser imposible tener un texto cifrado $C_2$ que se relacione de manera alguna a $P_1$

### Nociones de seguridad
* Se suele mostrar un modelo de tipo GOAL-MODEL
* El algoritmo g...............


> Cyberchef
