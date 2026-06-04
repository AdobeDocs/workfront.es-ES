---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop no puede establecer una conexión
description: Cuando intenta conectar Tableau Desktop a Data Connect, aparece un error.
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 253
ht-degree: 5%

---

# Tableau Desktop no puede establecer una conexión

## Problema

Cuando intente conectar Tableau Desktop a Data Connect, verá el siguiente error:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Causa

Este error se debe a una configuración de proxy en el equipo local que impide que se carguen datos desde Data Connect.

Data Connect se proporciona a través de servicios en la nube de Snowflake de terceros. Tableau requiere una red abierta para comunicarse con Snowflake.

## Solución

Puede intentar lo siguiente para resolver este problema:

* **Solucionar problemas deshabilitando la herramienta de seguridad**: Desactive la herramienta de seguridad, como Zscaler o Cisco, para ver si resuelve el problema de conectividad. Si esto resuelve el problema de conexión, asegúrese de que la herramienta de seguridad esté actualizada a la versión más reciente y agregue la dirección IP de Data Connect (Snowflake) a la lista de permitidos VPN con el equipo de red interna.

* **Agregar direcciones IP a la Lista de permitidos**: Asegúrese de que la configuración del firewall permita las direcciones IP que usa Data Connect. Utilice el comando `SYSTEM$ALLOWLIST()` para obtener la dirección IP, que puede lista de permitidos en la VPN.

* **Comprobar la configuración del servidor de seguridad y del proxy**: Compruebe si alguna configuración de servidor de seguridad o proxy de la red está bloqueando el acceso a los extremos de Snowflake. Es posible que deba ponerse en contacto con el administrador de red para agregar los puertos y las direcciones IP de Snowflake necesarios a la lista de permitidos de su empresa.

* **Opción de solución alternativa**: cree un extracto desde la pantalla de una hoja de cálculo en lugar del panel Data Source en Tableau. La conexión no se pierde y el proceso de extracción se completa.
