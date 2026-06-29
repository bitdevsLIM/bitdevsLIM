+++
title = "BitdevsLIM Seminario Socrático #06"
template = "post.html"
[extra]
meetup_id = "u981b1fi"
+++

### Lugar

Este evento se realizará de forma virtual. Participan del espacio en [https://x.com/i/spaces/1nJOLLOVAZOxR](https://x.com/i/spaces/1nJOLLOVAZOxR).

### Contacto

- Si quieres exponer algún tema en BitDevs, escríbenos a [40230@pm.me](mailto:40230@pm.me).

### Sugerencias

- Sé cortés y amable: el objetivo es la búsqueda de una comprensión más profunda. Respeta ideas y argumentos diferentes.
- Si preparas una intervención de más de 3 minutos, apóyala con imágenes o enlaces a recursos web, y procura no extenderte más de 10 minutos.

### Recordatorios

- No fotos.
- No videos.
- Audio recording = OK.

### ¿Cómo funciona el BitDevs?

**BitDevs** es un encuentro socrático técnico para revisar los avances más relevantes del ecosistema Bitcoin. En cada sesión seleccionamos varios temas clave de las últimas semanas (propuestas de mejora, papers, actualizaciones de protocolos, etc.). Los participantes revisan los temas con anticipación y la reunión se convierte en una discusión abierta, profunda y sin presentaciones largas.

Esta comunidad se inició en Nueva York en 2018 y hoy se celebra en varias ciudades del mundo como uno de los encuentros técnicos más respetados de Bitcoin.

El foco de BitDevs es **100% técnico**. Si recién estás comenzando a conocer Bitcoin, te recomendamos observar primero y asistir más adelante.

### Temas de esta edición

- **Lightning 2026: BOLT12, splicing, Ark y seguridad operacional**

  **Ángulo:** Lightning está pasando de "canales manuales" a una capa más modular: offers, splicing, LSPs, Ark, wallets híbridas y mejores mitigaciones de DoS.

  **Razón:** En junio, Optech reportó avances relacionados con BOLT12 en LND, fixes de splicing en Eclair, Ark/Bark corriendo en mainnet y wallets Ark en desarrollo. También hubo divulgación responsable de una vulnerabilidad DoS que afectaba versiones antiguas de LND, lo cual abre buen debate sobre fuzzing, seguridad de gossip y responsabilidad de operadores de nodos.

- **Bitcoin post-quantum: BIP360, BIP361 y migración de UTXOs expuestos**

  **Ángulo:** Separar hype de ingeniería real: qué partes de Bitcoin están expuestas, qué propone P2MR, qué implica una migración y qué tradeoffs tendría.

  **Razón:** BIP360 propone Pay-to-Merkle-Root como output type para reducir exposición de claves públicas al remover el key-path spend estilo Taproot; BIP361 plantea una migración/sunset de firmas legacy. Optech también cubrió ideas para hacer BIP324 quantum-secure y cambios recientes al propio BIP360.

- **Captura social de Bitcoin Core: ¿ataque real, paranoia o mecanismo normal de OSS?**

  **Ángulo:** Bitcoin no solo puede ser atacado por fallas técnicas, censura minera o presión regulatoria. También podría ser influenciado desde su capa social: funding, reputación, moderación, acceso a eventos, grants, poder de merge y formación de consenso informal alrededor de Bitcoin Core.

  **Razón:** A partir del artículo de hodlonaut sobre una posible red de influencia alrededor de Bitcoin Core, revisaremos si existe un riesgo real de captura institucional o si estas dinámicas son simplemente parte normal del desarrollo open-source. El caso abre una discusión importante: aunque las reglas de consenso no cambien, los defaults del software, las políticas de relay, la narrativa técnica y la confianza en los maintainers pueden afectar la dirección práctica de Bitcoin.
