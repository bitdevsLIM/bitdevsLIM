+++
title = "BITDEVSLIM Seminario Socrático #08"
template = "post.html"
[extra]
luma_id = "qa7f3iid"
cover = "/covers/008.avif"
+++

### Temas de esta edición

1. **Protocolo Mostro: P2P no custodial sobre Lightning y Nostr**

   Revisaremos cómo funciona el escrow con *hold invoices* y por qué el nodo Mostro no controla los fondos. También veremos el protocolo v2 con NIP-44, la publicación de órdenes mediante NIP-69 y *kinds* propios, y la competencia entre operadores independientes.

   **Ángulo:** cómo configurar y operar un nodo Mostro; qué confianza residual existe en el operador; privacidad de mensajes y ratings; diferencias con lnp2pBot; y posibilidades de escalar un marketplace P2P descentralizado, especialmente en Latinoamérica.

2. **Bitchat + Cashu: malla Bluetooth sin conexión y ecash**

   Analizaremos la arquitectura híbrida de Bitchat: malla BLE con Noise Protocol y respaldo mediante Nostr. Revisaremos la integración de Cashu para transferir sats sin conexión con `/pay` y los límites de privacidad de la malla, incluidos los identificadores persistentes y la observabilidad local.

3. **Ataque a la cadena de distribución de hardware wallets Ledger (octubre de 2026, CryptoBilis)**

   Revisaremos el ataque reportado: un grupo habría comprado dispositivos genuinos, instalado un implante de hardware que capturaba la semilla durante la configuración y la transmitía por LTE, y reintroducido los dispositivos en la cadena de distribución, principalmente mediante el reseller CryptoBilis en el sudeste asiático. No habría sido un ataque a la fábrica ni al *secure element*. Las pérdidas estimadas son de aproximadamente USD 90–100 millones.

4. **Privacidad en Bitcoin L1: Silent Payments multiparty y Shielded Bitcoin**

   - **Silent Payments multiparty (Optech #429):** cómo generar transacciones Silent Payment de forma colaborativa desde wallets multiparty.
   - **Shielded Bitcoin (paper de [[alloc] init], septiembre de 2026):** un metaprotocolo que publica notas cifradas, *nullifiers* y pruebas ZK en Bitcoin sin un *soft fork*. Los indexers reconstruyen el estado fuera de cadena y las entradas y salidas (*peg-in/peg-out*) se realizan mediante PIPEs.

5. **Hack de Binance (29 de octubre de 2026): seguridad operacional de custodios y autocustodia**

   Analizaremos la salida de aproximadamente 18.270 BTC y otros activos desde las *hot wallets* de Binance. Según los reportes, no se filtraron las claves privadas: una campaña de ingeniería social —entrevistas falsas y malware en las laptops de ingenieros— comprometió la infraestructura interna de firma y permitió usar firmas válidas. También revisaremos el uso de EIP-7702 en otras cadenas y las lecciones para custodios y usuarios de autocustodia.
