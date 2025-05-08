+++
title = "BitdevsLIM Seminario Socrático #02"
template = "post.html"
[extra]
meetup_id = "imyvfrfs"
+++

### Cronograma

19:00hrs Seminario Socrático  
20:30hrs Cierre y Networking

### Lugar

Este evento se llevará a cabo en [meet.jit.si/bitdevs-lima-002](https://meet.jit.si/bitdevs-lima-002)

Si quieres que BitDevs sea en tu espacio: [40230@pm.me](mailto:40230@pm.me)

### Sugerencias

- Sé cortés y amable. El objetivo es la búsqueda de una comprensión más profunda. Respeta los diferentes pensamientos e ideas.

- Complementa con imágenes or websites las intervenciones verbales preparadas de más de 3 min, recuerda no extenderte más de 10 min, todas las presentaciones incluyendo preguntas son de 10 min, como máximo.

### Recordatorios

No fotos, no videos, pero audio recoding = OK


### Qué es un seminario socrático de BitDevs?

El seminario socrático de BitDev o Bitcoin developers es un evento mensual diseñado para promover el debate, el intercambio de información y la discusión sobre temas técnicos relacionados con Bitcoin y su ecosistema. Estos seminarios siguen un formato participativo, en el que se discuten y se hacen preguntas sobre temas recopilados por los miembros del grupo antes del evento.
Los temas provienen de varias fuentes, como bitcoinops Optech, pull requests en repositorios populares de proyectos como Bitcoin.


- Los Seminarios Socráticos se celebran bajo la Regla de **[Chatham House](https://www.chathamhouse.org/about-us/chatham-house-rule)**:
- Puedes compartir la información recibida, pero no reveles la identidad de quien la ha dicho.
- Cuando una reunión, o parte de ella, se celebra bajo la Regla de Chatham House, los participantes son libres de utilizar la información recibida, pero no se puede revelar ni la identidad ni la afiliación del orador u oradores, ni dónde se escuchó la información, ni la de ningún otro participante.


[Source](https://bitdevs.org/running-a-great-socratic-seminar/)

#### Estadísticas de la Red
- [mempool.space](https://mempool.space/)
- [clarkmoody.com](https://bitcoin.clarkmoody.com/dashboard/)
- [Block Fee Rates](https://mempool.space/graphs/mining/block-fee-rates#1m)
- [Block Rewards 1m](https://mempool.space/graphs/mining/block-rewards#1m)

### 1. Against Allowing Quantum Recovery of Bitcoin

**Descripción:**
Un argumento a favor de quemar bitcoin en direcciones vulnerables para evitar que los fondos sean tomados por quienes ganen la carrera de la computación cuántica.

**Puntos de discusión:**
- Inflación: Permitir gastar monedas vulnerables podría aumentar la oferta de bitcoin y alterar su valor.
- Propiedad: Quemarlas protege a los dueños originales frente a robos cuánticos.
- Confianza: Evitar que se gasten ayuda a mantener la integridad y seguridad de la red.
---

### 2. DATUM
*** Descripción ***
DATUM (Decentralized Alternative Templates for Universal Mining) es un protocolo desarrollado por OCEAN con el objetivo de devolver a los mineros el control sobre la construcción de bloques en la red de Bitcoin, contrarrestando la creciente centralización en los grandes pools de minería

** Puntos de discusión: **
- La descentralización real en la construcción de bloques puede entrar en tensión con la eficiencia operativa.
- Reducción del riesgo de censura por parte de pools centralizados.
- DATUM representa una apuesta por soluciones prácticas frente al enfoque más estandarizado de Stratum V2.

Link: https://www.ocean.xyz/docs/datum

### 3. OP_CAT

**Descripción:**  
Reactivación de un antiguo opcode eliminado por razones de seguridad. OP_CAT permitiría concatenar elementos en la pila y habilitaría contratos inteligentes más expresivos, acercando a Bitcoin a funcionalidades de scripting más complejas.

**Puntos de discusión:**  

- ¿Es OP_CAT seguro de implementar hoy?  
- ¿Qué tipo de contratos inteligentes permitiría?  
- ¿Cuál es la oposición o cautela en la comunidad?

---

### 4. Covenants

**Descripción:**  
Covenants son restricciones en cómo se puede gastar un UTXO en el futuro. Propuestas como CheckTemplateVerify (CTV), APO o OP_VAULT buscan implementar esta lógica. Permitirían vaults, recuperación de fondos y aplicaciones tipo “smart wallet”.

**Puntos de discusión:**  

- ¿Qué casos de uso resuelven los covenants?  
- Comparación entre CTV, OP_VAULT y alternativas.  
- ¿Cómo afectan a la fungibilidad de Bitcoin?

---

### 5. RUNES y Tokens BRC-20

**Descripción:**  
RUNES es un nuevo protocolo para emitir tokens fungibles en Bitcoin, propuesto como alternativa eficiente y nativa frente al actual estándar BRC-20 que funciona sobre Ordinals. Busca simplicidad y menor carga sobre la red.

**Puntos de discusión:**  

- ¿Qué ventajas tiene RUNES sobre BRC-20?  
- ¿Cuál es el impacto real de los tokens en la red de Bitcoin?  
- ¿Deben los nodos filtrar o censurar estos usos?

### 6. OP_RETURN size limit

**Descripción:**  
El campo OP_RETURN permite almacenar datos arbitrarios en una transacción de Bitcoin. Su límite actual es de 80 bytes. Recientemente ha resurgido el debate sobre si este límite debería incrementarse para facilitar casos de uso como identidad descentralizada, timestamps o protocolos como OpenTimestamps.

**Puntos de discusión:**  

- ¿Aumentar el límite afecta el tamaño de los bloques y la descentralización?  
- ¿Qué casos de uso justifican este cambio?  
- ¿Se pueden lograr objetivos similares fuera de la cadena?