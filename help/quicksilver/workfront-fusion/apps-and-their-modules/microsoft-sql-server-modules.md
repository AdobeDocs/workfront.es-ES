---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Módulos de Microsoft SQL Server
description: Puede usar [!DNL Adobe Workfront Fusion] para conectarse a Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] módulos

Puede usar [!DNL Adobe Workfront Fusion] para conectarse a [!UICONTROL Microsoft SQL Server].

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Uso [!DNL Microsoft SQL Server] módulos

Puede ejecutar la lógica personalizada directamente en el servidor de la base de datos mediante procedimientos almacenados. [!DNL Adobe Workfront Fusion] carga la interfaz de parámetros de entrada/salida y el conjunto de registros de forma dinámica, de modo que cada parámetro o valor se pueda asignar individualmente. Antes de empezar a configurar el escenario, asegúrese de que la cuenta que está utilizando para conectarse a la base de datos tenga acceso de lectura a `INFORMATION_SCHEMA.ROUTINES` y `INFORMATION_SCHEMA.PARAMETERS` vistas.

When [!DNL Fusion] establece la conexión con la variable [!DNL SQL server] destino, la variable [!DNL Fusion] el usuario identifica el host (el nombre de dominio o la dirección IP donde se aloja el servidor) y el puerto. [!DNL Fusion] puede conectarse a cualquier host y puerto disponibles.

Para obtener información sobre las direcciones IP específicas que utiliza [!DNL Workfront Fusion], consulte [Direcciones IP para acceder [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Para obtener más información sobre la creación de un procedimiento almacenado, consulte la [!DNL Microsoft SQL Server] documentación.

>[!NOTE]
>
>[!DNL Workfront Fusion] no admite varios conjuntos de registros. Solo se procesa el primero.

## Solución de problemas de error [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Se ha superado el tiempo de espera de bloqueo; intente reiniciar la transacción]

Este error se produce cuando se modifican los mismos datos mediante varios módulos. Está causado por transacciones SQL.

Cuando se ejecuta cualquier módulo SQL, se inicia una transacción. La transacción finaliza después de que el escenario se ejecute completamente.

Si otro módulo intenta acceder a los mismos datos, tiene que esperar hasta que finalice la transacción anterior. Dado que la primera transacción finaliza una vez finalizado el escenario, la segunda transacción nunca puede comenzar.

### Solución:

Active la confirmación automática. La confirmación automática finaliza (confirma) cada transacción inmediatamente después de que se haya realizado la ejecución del módulo.

1. Haga clic en el [!UICONTROL Configuración del escenario] icono ![](assets/scenario-settings-icon.png)en la parte inferior de la pantalla.
1. Haga clic en el **[!UICONTROL Compromiso automático]** casilla de verificación.
1. Haga clic en **[!UICONTROL OK]** para guardar la configuración del escenario.
