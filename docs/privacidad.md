---
id: privacidad
title: Privacidad
sidebar_label: Privacidad
---

La privacidad en LatamLink se centra en hacer que los datos solo estén disponibles para una lista específica de participantes. Para lograr esto, se debe implementar un mecanismo que garantice que las transacciones se distribuyan solo a una lista de participantes que pueden enviar transacciones privadas entre ellos.

Esto trae unas cuantas de preguntas:

- ¿Qué cuentas pueden ver la transacción?
- ¿Qué nodos pueden ver la transacción?
- ¿Qué nodos pueden ver el contrato inteligente?
- ¿Quién maneja la lista de actores permitidos? (en cadena vs. fuera de cadena)

## Propuesta LatamLink ZKP

La tecnología Blockchain proporciona las herramientas necesarias para descentralizar la información de una manera segura e inquebrantable. La introducción de Bitcoin hizo posible que miles de nodos de todo el mundo compartan y mantengan la misma información. Sin embargo, en la mayoría de Blockchains, la idea central es mantener esta información pública para que todos puedan acceder a ella y verificarla, sin la necesidad de ninguna entidad central controladora, es por eso que definimos a las  blockchains públicas como redes *trust-less* (no hace falta confiar).

Es así cómo muchas empresas y entidades privadas que desean utilizar la tecnología blockchain se encuentran con un importante interrogante: ¿cómo puedo mantener la información privada y al mismo tiempo lograr mantener la seguridad y la transparencia de una blockchain pública?

Aquí es donde entran en juego los Protocolos de Cero Conocimiento, también conocidos como ZKP por sus siglas en inglés Zero Knowledge Proof: ZKP es el método por el cual los operadores de nodos pueden probar que una transacción es válida sin revelar realmente los valores de esa transacción.

El hecho de que este valor agregado de privacidad se puede obtener a través de la criptografía es muy útil para las personas y entidades privadas que se benefician del uso de la tecnología blockchain sin temor a compartir información confidencial.

LatamLink apunta a integrar primitivas (intrinsics) para verificación de pruebas de cero conocimiento disponibles de forma nativa a los smart-contracts (Dapps) para la construcción de aplicación con requerimientos de privacidad y que al mismo tiempo sean validadas por lo mismos agentes de la red (BPs + Full Nodes), sin necesidad de agregar agentes nuevos a la Red.


### Soluciones existentes de privacidad de datos en EOSIO
https://github.com/EOSIO/eosjs-ecc/issues/19#issuecomment-392941963

https://github.com/GetScatter/ScatterDesktop/issues/43

### Orion Layer
 
**Hyperledger Besu** tiene una extensión del cliente ethereum de pre-compilado que utiliza claves de orion para canalizar transacciones privadas a través de nodos de orion para evitar que los datos sean visibles en la red pública.
