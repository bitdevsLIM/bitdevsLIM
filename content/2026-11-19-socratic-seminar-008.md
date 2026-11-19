+++
title = "BITDEVSLIM Seminario Socrático #08"
template = "post.html"
[extra]
luma_id = "qa7f3iid"
cover = "/covers/008.avif"
+++

### Fecha y horario

Jueves 19 de noviembre de 2026, de **19:00 a 21:00** (hora de Lima, UTC-5).

### Lugar

Este evento se realizará de forma presencial en **Av. Paseo de la República 6334, Miraflores 15074**.

[Ver ubicación en Google Maps](https://www.google.com/maps/search/?api=1&query=Av.%20Paseo%20de%20la%20Rep%C3%BAblica%206334%2C%20Miraflores%2015074).

### Contacto

- Si quieres exponer algún tema en BitDevs, escribe a [40230@pm.me](mailto:40230@pm.me).

### Sugerencias

- Sé cortés y amable: el objetivo es la búsqueda de una comprensión más profunda. Respeta ideas y argumentos diferentes.
- Revisa los recursos antes de asistir. Si preparas una intervención de más de 3 minutos, apóyala con imágenes o enlaces y procura no extenderte más de 10 minutos.

### Recordatorios

- No fotos.
- No videos.
- Se permite grabar audio.

### ¿Cómo funciona el BitDevs?

**BitDevs** es un encuentro socrático técnico para discutir Bitcoin y tecnologías relacionadas. Revisamos propuestas, investigaciones e incidentes de seguridad mediante una conversación abierta. Puedes revisar los recursos antes de asistir y traer preguntas para los expositores.

### Temas de esta edición

1. **Protocolo Mostro: P2P no custodial sobre Lightning y Nostr**

   Revisaremos cómo funciona el escrow con *hold invoices* y por qué el nodo Mostro no controla los fondos. También veremos el protocolo v2 con NIP-44, la publicación de órdenes mediante NIP-69 y *kinds* propios, y la competencia entre operadores independientes.

   **Ángulo:** cómo configurar y operar un nodo Mostro; qué confianza residual existe en el operador; privacidad de mensajes y ratings; diferencias con lnp2pBot; y posibilidades de escalar un marketplace P2P descentralizado, especialmente en Latinoamérica. Las *hold invoices* bloquean temporalmente el pago hasta que se cumplan las condiciones de la operación; debatiremos qué ocurre ante disputas, desconexiones o un operador que deja de responder.

   Recursos: [documentación del protocolo Mostro](https://mostro.network/protocol/) y [código fuente](https://github.com/MostroP2P/mostro).

2. **Bitchat + Cashu: malla Bluetooth sin conexión y ecash**

   Analizaremos la arquitectura híbrida de Bitchat: malla BLE con Noise Protocol y respaldo mediante Nostr. Revisaremos la integración de Cashu para compartir tokens ecash y pagar mediante `/pay`. Un token puede circular sin conexión entre teléfonos, pero su canje depende de la casa de moneda que lo emitió; discutiremos qué metadatos pueden observar esa casa de moneda y los pares cercanos, además de los límites de privacidad de la malla.

   Recursos: [repositorio de Bitchat](https://github.com/permissionlesstech/bitchat) y [funcionalidad Cashu y `/pay`](https://github.com/permissionlesstech/bitchat-android/issues/756).

3. **Ataque a la cadena de distribución de hardware wallets Ledger (octubre de 2026, CryptoBilis)**

   Revisaremos el ataque reportado: Ledger confirmó un implante físico no autorizado en un dispositivo vinculado al incidente, y los casos confirmados se asociaron a equipos vendidos por CryptoBilis. Los reportes describen captura de la frase de recuperación mostrada en pantalla y transmisión celular. Contrastaremos qué se conoce y qué sigue siendo una estimación sobre alcance y pérdidas; el caso pone en discusión la cadena de custodia, la verificación del dispositivo y el supuesto de que el *secure element* protege frente a todos los ataques.

   Recursos: [actualización de Ledger](https://www.ledger.com/blog) y [reporte de CoinDesk](https://www.coindesk.com/tech/2026/10/13/ledger-says-spy-chip-inside-cryptobilis-ledger-devices-transmitted-wallet-keys-over-mobile-network/).

4. **Privacidad en Bitcoin L1: Silent Payments multiparty y Shielded Bitcoin**

   - **Silent Payments multiparty:** cómo generar pagos colaborativos a direcciones reutilizables que producen salidas distintas sin revelar públicamente que pertenecen al mismo receptor. Revisaremos el protocolo AggDLEQ propuesto para que una wallet multiparty pueda derivar esas salidas y el costo de escaneo para quien recibe. Recurso: [tema Silent Payments en Bitcoin Optech](https://bitcoinops.org/en/topics/silent-payments/).
   - **Shielded Bitcoin:** un metaprotocolo que publica notas cifradas, *nullifiers* y pruebas de conocimiento cero en Bitcoin sin cambios de consenso. Los indexers reproducen los datos publicados para reconstruir el estado fuera de cadena; el paper deja los mecanismos de entrada y salida (*peg-in/peg-out*) fuera de alcance. Discutiremos qué privacidad ofrece y qué supuestos introduce depender de publicación de datos e indexers. Recurso: [paper en IACR ePrint](https://eprint.iacr.org/2026/2749).

5. **Hack de Binance (29 de octubre de 2026): seguridad operacional de custodios y autocustodia**

   Analizaremos la salida reportada de aproximadamente 18.270 BTC y otros activos desde billeteras calientes de Binance. La actualización inicial de Binance atribuyó el incidente a una autorización maliciosa EIP-7702 en una billetera de Ethereum; otras reconstrucciones describen el compromiso de procesos internos de firma mediante ingeniería social. Separaremos los hechos confirmados de las hipótesis sobre el acceso inicial y discutiremos cómo límites de autorización, demoras, monitoreo y controles fuera de banda pueden reducir el impacto.

   Recursos: [actualización de Binance](https://www.binance.com/en/square/post/384328127385979) y [explicación de EIP-7702](https://eips.ethereum.org/EIPS/eip-7702).

6. **El bug de SIGHASH_SINGLE y firmas cortas para pubkeys "artificiales"**

   En scripts *legacy*, si un input firmado con `SIGHASH_SINGLE` no tiene un output con su mismo índice, `SignatureHash` devuelve la constante `1` en lugar de un hash de la transacción. Como el mensaje firmado ya no depende de nada, se puede elegir primero una firma muy corta y luego derivar una pubkey para la que esa firma es válida, sin que nadie conozca la llave privada. Revisaremos un caso real: inputs P2PK de 1.800 sats gastados el 13 de noviembre (bloque 975.743) con una firma de apenas 41 bytes.

   **Ángulo:** por qué este bug sigue en consenso desde la versión original de Satoshi; por qué SegWit v0 y Taproot no lo heredan; qué pasa con cualquier moneda enviada a una de estas pubkeys; y qué otras "rarezas" de scripts *legacy* sigue cargando el protocolo.

   Recursos: [hilo de mononaut](https://x.com/mononautical/status/2121503248263823682) y [transacción en mempool.space](https://mempool.space/tx/82d3bb7791933a0c557b8216804f82826f5172a082ccba39ea4b5cb4e45e11d5).

7. **Tres CVE de Bitcoin Core divulgados el 10 de noviembre**

   - **CVE-2025-62861 (severidad alta):** un *reorg* combinado con el *sibling eviction* de transacciones TRUC podía corromper el mempool y dejar a un minero sin poder construir plantillas de bloque hasta reiniciar. Afecta las versiones 28.0 a 29.1; está corregido en 29.2 y 30.0.
   - **CVE-2025-62860 (severidad media):** los peers entrantes por Tor recibían por error los permisos de `-whitelist`.
   - **CVE-2025-62859 (severidad media):** un peer podía retrasar el procesamiento de un *compact block*.

   Discutiremos cómo interactúan las nuevas reglas de política de mempool con los *reorgs*, y cómo funciona el proceso de divulgación responsable de Bitcoin Core.

   Recursos: [aviso de CVE-2025-62861](https://bitcoincore.org/en/2026/11/10/disclose-cve-2025-62861/) y [resumen en Bitcoin Optech](https://bitcoinops.org/en/newsletters/2026/11/13/).

8. **BIP de firmas anti-exfiltración**

   Una propuesta de protocolo de dos rondas para firmas Schnorr y ECDSA en el que el *host* aporta aleatoriedad al nonce y verifica que el dispositivo de firma realmente la usó, junto con nuevos campos PSBT. El objetivo es que un firmware malicioso no pueda filtrar la llave privada escondiéndola en los nonces de las firmas. Complementa el tema del ataque a Ledger: ¿qué ataques mitiga y cuáles no, como un implante que captura la frase de recuperación en pantalla?

   Recursos: [propuesta en la lista bitcoindev](https://mailing-list.bitcoindevs.xyz/bitcoindev/CAOuFX60em-d=JW+FmQe6G6mP58Gs6kpwuRwVLC5nwT8oO9HsXg@mail.gmail.com/) y [implementación de referencia](https://github.com/AvilaLabs/anti-exfil).

9. **Por qué fallaba la reconstrucción de *compact blocks***

   Entre julio y octubre casi ningún bloque se podía reconstruir sin pedir transacciones adicionales a los peers. Las transacciones que faltaban eran cadenas de *mints* de runas con outputs P2A que se empujaban a la red sin pasar por el flujo normal de `inv`/`getdata`. El empuje se detuvo el 18 de octubre y la tasa de reconstrucción se recuperó ese mismo día. Discutiremos qué nos dice esto sobre la propagación de bloques y la importancia de que los mempools de los nodos se parezcan a lo que minan los pools.

   Recursos: [estadísticas de 0xB10C en Delving Bitcoin](https://delvingbitcoin.org/t/stats-on-compact-block-reconstructions/1052/63) y [resumen en Bitcoin Optech](https://bitcoinops.org/en/newsletters/2026/11/13/).

10. **Testnet5 ya tiene bloque génesis (BIP 95)**

    BIP 95 pasó a estado *Deployed* el 17 de noviembre. El génesis de testnet5 se compromete con el bloque 975.744 de mainnet, no tiene la excepción de dificultad mínima que tenían testnet3 y testnet4, y activa BIP 54 (*Consensus Cleanup*) desde el bloque 1. Discutiremos qué se aprendió de las testnets anteriores y si esta vez el diseño evitará los mismos abusos.

    Recursos: [BIP 95](https://bips.dev/95/) y [anuncio en la lista bitcoindev](https://groups.google.com/g/bitcoindev/c/DmFiHeo-xRw).
