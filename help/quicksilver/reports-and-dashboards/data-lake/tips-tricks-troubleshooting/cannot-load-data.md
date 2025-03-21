---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop no puede establecer una conexión
description: Cuando intenta conectar Tableau Desktop a Data Connect, aparece un error.
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 1%

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

