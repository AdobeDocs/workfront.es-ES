---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Microsoft SQL Server
description: Puede usar [!DNL Adobe Workfront Fusion] para conectarse a Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '502'
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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Conectando el servicio [!DNL Microsoft SQL Server] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar tu cuenta de [!DNL Microsoft SQL Server] a [!UICONTROL Workfront Fusion], consulta [Crear una conexión a [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra todos los permisos que se hayan concedido anteriormente a la conexión de este usuario, además de los nuevos permisos necesarios para la aplicación actual.
>
>Por ejemplo, si un usuario tiene permisos de &quot;Leer tabla&quot; concedidos a través del conector de Excel y, a continuación, crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya concedido como el permiso de &quot;Escribir correo electrónico&quot; recién requerido.

## Usando módulos de [!DNL Microsoft SQL Server]

Puede ejecutar la lógica personalizada directamente en el servidor de base de datos mediante procedimientos almacenados. [!DNL Adobe Workfront Fusion] carga dinámicamente la interfaz de parámetros de entrada/salida y el conjunto de registros para que cada parámetro o valor se pueda asignar individualmente. Antes de comenzar a configurar el escenario, asegúrese de que la cuenta que está utilizando para conectarse a la base de datos tiene acceso de lectura a las vistas `INFORMATION_SCHEMA.ROUTINES` y `INFORMATION_SCHEMA.PARAMETERS`.

Cuando [!DNL Fusion] establece la conexión con el destino [!DNL SQL server], el usuario [!DNL Fusion] identifica el host (el nombre de dominio o la dirección IP donde está alojado el servidor) y el puerto. [!DNL Fusion] puede conectarse a cualquier host y puerto disponible.

Para obtener información acerca de las direcciones IP específicas que usa [!DNL Workfront Fusion], vea [Direcciones IP para obtener acceso a [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Para obtener más información acerca de cómo crear un procedimiento almacenado, consulte la documentación de [!DNL Microsoft SQL Server].

>[!NOTE]
>
>[!DNL Workfront Fusion] no admite varios conjuntos de registros. Solo se procesa la primera.

## Error de solución de problemas [!UICONTROL ER_LOCK_WAIT_TIMEOUT: tiempo de espera de bloqueo superado; intente reiniciar la transacción]

Este error se produce cuando se modifican los mismos datos utilizando varios módulos. Se debe a transacciones SQL.

Cuando se ejecuta cualquier módulo SQL, inicia una transacción. La transacción finaliza después de que el escenario se ejecute completamente.

Si otro módulo intenta acceder a los mismos datos, debe esperar hasta que finalice la transacción anterior. Dado que la primera transacción finalizará después de que finalice el escenario, la segunda transacción nunca puede comenzar.

### Solución:

Active la confirmación automática. La confirmación automática finaliza (confirma) todas las transacciones inmediatamente después de que se haya completado la ejecución del módulo.

1. Haga clic en el icono [!UICONTROL Configuración de escenario] ![](assets/scenario-settings-icon.png)en la parte inferior de la pantalla.
1. Haga clic en la casilla de verificación **[!UICONTROL Confirmación automática]**.
1. Haga clic en **[!UICONTROL Aceptar]** para guardar la configuración del escenario.
