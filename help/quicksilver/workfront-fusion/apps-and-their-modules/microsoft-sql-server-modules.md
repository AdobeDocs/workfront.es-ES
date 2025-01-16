---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Microsoft SQL Server
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 82%

---

# Módulos de [!DNL Microsoft SQL Server]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Módulos de Microsoft SQL Server](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-sql-server-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

Puede usar [!DNL Adobe Workfront Fusion] para conectarse a [!UICONTROL Microsoft SQL Server].

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Conexión con el servicio [!DNL Microsoft SQL Server] a [!DNL Workfront Fusion]

Para obtener instrucciones sobre cómo conectar su cuenta de [!DNL Microsoft SQL Server] a [!UICONTROL Workfront Fusion], consulte [Crear una conexión a [!UICONTROL Adobe Workfront Fusion]: instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra los permisos que se otorgaron previamente a la conexión de este usuario, además de cualquier nuevo permiso que sea necesario para la aplicación actual.
>
>Por ejemplo, si a un usuario se le han otorgado permisos de &quot;Leer tabla&quot; a través del conector de Excel y luego crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya otorgado como el nuevo permiso requerido de &quot;Escribir correo electrónico&quot;.

## Uso de módulos [!DNL Microsoft SQL Server]

Puede ejecutar la lógica personalizada directamente en el servidor de base de datos mediante procedimientos almacenados. [!DNL Adobe Workfront Fusion] carga dinámicamente la interfaz de parámetros de entrada/salida y el conjunto de registros para que cada parámetro o valor se pueda asignar individualmente. Antes de comenzar a configurar el escenario, asegúrese de que la cuenta que está utilizando para conectarse a la base de datos tiene acceso de lectura a las vistas `INFORMATION_SCHEMA.ROUTINES` y `INFORMATION_SCHEMA.PARAMETERS`.

Cuando [!DNL Fusion] establece la conexión con el destino [!DNL SQL server], el usuario [!DNL Fusion] identifica el host (el nombre de dominio o la dirección IP donde está alojado el servidor) y el puerto. [!DNL Fusion] puede conectarse a cualquier host y puerto disponible.

Para obtener información acerca de las direcciones IP específicas que usa [!DNL Workfront Fusion], consulte [Direcciones IP para acceder a [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Para obtener más información acerca de cómo crear un procedimiento almacenado, consulte la documentación de [!DNL Microsoft SQL Server].

>[!NOTE]
>
>[!DNL Workfront Fusion] no admite varios conjuntos de registros. Solo se procesa el primero.

## Error de solución de problemas [!UICONTROL ER_LOCK_WAIT_TIMEOUT: tiempo de espera de bloqueo superado; intente reiniciar la transacción]

Este error se produce cuando se modifican los mismos datos utilizando varios módulos. Se debe a transacciones SQL.

Cuando se ejecuta cualquier módulo SQL, se inicia una transacción. La transacción finaliza después de que el escenario se ejecute completamente.

Si otro módulo intenta acceder a los mismos datos, debe esperar hasta que finalice la transacción anterior. Dado que la primera transacción finalizará después de que finalice el escenario, la segunda transacción nunca podrá comenzar.

### Solución:

Activar la confirmación automática. La confirmación automática finaliza (confirma) todas las transacciones inmediatamente después de que se haya completado la ejecución del módulo.

1. Haga clic en el icono [!UICONTROL Scenario settings] ![](assets/scenario-settings-icon.png)en la parte inferior de la pantalla.
1. Haga clic en la casilla de verificación **[!UICONTROL Auto commit]**.
1. Haga clic en **[!UICONTROL OK]** para guardar la configuración del escenario.
