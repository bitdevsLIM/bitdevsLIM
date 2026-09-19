+++
title = "BITDEVSLIM Seminario Socrático #07"
template = "post.html"
[extra]
luma_id = "l0561n87"
cover = "/covers/007.avif"
+++

### Fecha y horario

Jueves 24 de septiembre de 2026, de **19:00 a 21:00** (hora de Lima, UTC-5).

### Lugar

Este evento se realizará de forma presencial en **Av. Paseo de la República 6334, Miraflores 15074**.

[Ver ubicación en Google Maps](https://www.google.com/maps/search/?api=1&query=Av.%20Paseo%20de%20la%20Rep%C3%BAblica%206334%2C%20Miraflores%2015074).

### Contacto

- Si quieres exponer algún tema en BitDevs, escríbenos a [40230@pm.me](mailto:40230@pm.me).

### Sugerencias

- Sé cortés y amable: el objetivo es la búsqueda de una comprensión más profunda. Respeta ideas y argumentos diferentes.
- Si preparas una intervención de más de 3 minutos, apóyala con imágenes o enlaces a recursos web, y procura no extenderte más de 10 minutos.

### Recordatorios

- No fotos.
- No videos.
- Se permite grabar audio.

### ¿Cómo funciona el BitDevs?

**BitDevs** es un encuentro socrático técnico para discutir Bitcoin y tecnologías relacionadas. Revisamos propuestas, investigaciones e incidentes de seguridad mediante una conversación abierta. Puedes revisar los recursos antes de asistir y traer preguntas para los expositores.

### Temas de esta edición

1. **Hack de Coldcard**

   Revisaremos el incidente de seguridad de Coldcard y las lecciones que deja sobre la generación de semillas en una hardware wallet. Discutiremos por qué mantener las claves fuera de línea no basta si su generación es predecible, cómo evaluar el alcance de una vulnerabilidad y qué diferencia hay entre corregir el firmware y reemplazar una semilla comprometida. Recurso: [estado de seguridad de Coldcard](https://coldcard.com/security/status).

2. **Vulnerabilidades en Lightning**

   Analizaremos las superficies de ataque de los canales de pago: bloqueo de liquidez, denegación de servicio y problemas al resolver pagos pendientes en cadena. La discusión se centrará en distinguir fallas del protocolo de errores de implementación, entender qué condiciones necesita cada ataque y evaluar las mitigaciones para operadores de nodos. Recursos: [discusión técnica sobre replacement cycling y OP_EXPIRE](https://delvingbitcoin.org/t/op-expire-mitigating-replacing-cycling-attacks/1282) y [mitigaciones en el sweeper de LND](https://delvingbitcoin.org/t/lnds-deadline-aware-budget-sweeper/1512).

3. **Fork de BIP110**

   Exploraremos las reglas y decisiones técnicas del fork asociado a BIP110 y cómo se diferencia una propuesta de cambio de una red que aplica sus propias reglas de consenso. Conversaremos sobre compatibilidad entre nodos, separación de cadenas, protección contra la repetición de transacciones y las implicaciones para usuarios, mineros y desarrolladores. Recurso: [referencia técnica de la red Bitcoin BIP110](https://bitcoinbip110.org/technicals/).

4. **Autocustodia y entropía**

   La entropía es la aleatoriedad que hace impredecible una semilla. Veremos cómo se relaciona con las palabras de recuperación, por qué inventar palabras o usar patrones humanos debilita la seguridad y cómo pensar en la generación, el respaldo y la recuperación de claves. También discutiremos los límites de las passphrases y los riesgos de introducir pasos manuales sin comprenderlos. Recurso: [BIP39: generación de frases mnemónicas](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

5. **Arkade, extensión de Bitcoin**

   Conoceremos cómo Arkade utiliza el protocolo Ark y salidas virtuales de transacción (VTXOs) para realizar operaciones fuera de cadena y liquidarlas en Bitcoin. Debatiremos qué permite construir, qué función cumple el operador y bajo qué condiciones un usuario puede salir unilateralmente a la cadena principal. Recurso: [documentación de Arkade](https://docs.arkadeos.com/).

6. **Primera transacción de Bitcoin resistente a ataques cuánticos: QSB de Avihu Levy**

   Analizaremos la demostración realizada por Avihu Levy, investigador de StarkWare, con Quantum Safe Bitcoin (QSB): el gasto en mainnet de una salida de 10,000 sats, confirmado en el bloque 964,199, mediante una construcción resistente al algoritmo de Shor y sin modificar las reglas de consenso de Bitcoin. Veremos cómo QSB extiende Binohash con firmas de un solo uso basadas en hashes y un acertijo *hash-to-signature* cuya seguridad depende de la resistencia de preimagen de RIPEMD-160, en vez de la dificultad del logaritmo discreto de ECDSA. También discutiremos sus límites prácticos: requiere horas de cómputo en GPU, cuesta aproximadamente USD 150–200, produce una transacción no estándar que debió enviarse directamente a MARA mediante Slipstream y funciona como solución de emergencia, no como sustituto de una actualización escalable del protocolo. Recursos: [reporte de la transacción en mainnet](https://es.tradingview.com/news/coinpedia:d1dd776b1094b:0-bitcoin-completes-first-quantum-resistant-transaction-says-starkware/), [Quantum-Safe Bitcoin Transactions](https://github.com/avihu28/Quantum-Safe-Bitcoin-Transactions) y [paper de QSB](https://raw.githubusercontent.com/avihu28/Quantum-Safe-Bitcoin-Transactions/main/paper/QSB.pdf).

7. **Hackeo de Liquid Network**

   Revisaremos el incidente reportado en Liquid Network para discutir cómo se valida el respaldo de una sidechain y qué responsabilidades tiene su federación. El análisis abordará la relación entre BTC y L-BTC, los controles de entrada y salida de fondos y las lecciones para detectar fallas, contener incidentes y verificar la recuperación del sistema. Recurso: [comunicado de Liquid Network sobre el incidente](https://x.com/Liquid_BTC/status/2096696272447218108).

8. **Bug en Alby Hub**

   Analizaremos el bug reportado en Alby Hub y sus implicaciones para quienes operan una wallet Lightning propia. Revisaremos el comportamiento esperado frente al observado, las condiciones que permiten reproducir el problema y cómo evaluar una corrección. La conversación incluirá la exposición de servicios, los permisos de las aplicaciones conectadas y la diferencia entre una falla de la wallet y una del protocolo Lightning. Recursos: [aviso de seguridad de Alby](https://x.com/getAlby/status/2097574956049498150) y [notas de versiones de Alby Hub](https://github.com/getAlby/hub/releases).

9. **LLMs y la seguridad de Bitcoin**

   Analizaremos cómo el uso de modelos de lenguaje para analizar código, descubrir vulnerabilidades y desarrollar exploits modifica las capacidades de los atacantes y los desafíos de defensa del protocolo y sus implementaciones. Discutiremos las implicaciones para Bitcoin a partir de investigaciones sobre explotación automatizada, distinguiendo los resultados experimentales de la evidencia de ataques reales, y exploraremos su uso defensivo en auditorías y revisión de código. Recursos: [LLM Agents can Autonomously Exploit One-day Vulnerabilities](https://arxiv.org/abs/2404.08144) y [CVE-Bench: evaluación de agentes de IA ante vulnerabilidades reales](https://arxiv.org/abs/2503.17332).
