---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Microsoft SQL Server
description: Puede utilizar [!DNL Adobe Workfront Fusion] para conectarse a Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] módulos

Puede utilizar [!DNL Adobe Workfront Fusion] para conectarse a [!UICONTROL Microsoft SQL Server].

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
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Conexión del [!DNL Microsoft SQL Server] servicio a [!DNL Workfront Fusion]

Para obtener instrucciones acerca de cómo conectar su [!DNL Microsoft SQL Server] cuenta a [!UICONTROL Workfront Fusion], consulte [Cree una conexión con [!UICONTROL Adobe Workfront Fusion] - Instrucciones básicas](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Algunas aplicaciones de Microsoft utilizan la misma conexión, que está vinculada a permisos de usuario individuales. Por lo tanto, al crear una conexión, la pantalla de consentimiento de permisos muestra todos los permisos que se hayan concedido anteriormente a la conexión de este usuario, además de los nuevos permisos necesarios para la aplicación actual.
>
>Por ejemplo, si un usuario tiene permisos de &quot;Leer tabla&quot; concedidos a través del conector de Excel y, a continuación, crea una conexión en el conector de Outlook para leer correos electrónicos, la pantalla de consentimiento de permisos mostrará tanto el permiso de &quot;Leer tabla&quot; ya concedido como el permiso de &quot;Escribir correo electrónico&quot; recién requerido.

## Uso de [!DNL Microsoft SQL Server] módulos

Puede ejecutar la lógica personalizada directamente en el servidor de base de datos mediante procedimientos almacenados. [!DNL Adobe Workfront Fusion] carga dinámicamente la interfaz de parámetros de entrada/salida y el juego de registros para que cada parámetro o valor se pueda asignar individualmente. Antes de comenzar a configurar el escenario, asegúrese de que la cuenta que está utilizando para conectarse a la base de datos tiene acceso de lectura a `INFORMATION_SCHEMA.ROUTINES` y `INFORMATION_SCHEMA.PARAMETERS` vistas.

Cuándo [!DNL Fusion] establece la conexión con [!DNL SQL server] destino, el [!DNL Fusion] El usuario identifica el host (el nombre de dominio o la dirección IP donde está alojado el servidor) y el puerto. [!DNL Fusion] puede conectarse a cualquier host y puerto disponible.

Para obtener información acerca de las direcciones IP específicas que utiliza [!DNL Workfront Fusion], consulte [Direcciones IP para acceder a [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

Para obtener más información acerca de cómo crear un procedimiento almacenado, vea la [!DNL Microsoft SQL Server] documentación.

>[!NOTE]
>
>[!DNL Workfront Fusion] no admite varios conjuntos de registros. Solo se procesa la primera.

## Error de resolución de problemas [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Se ha superado el tiempo de espera de bloqueo; intente reiniciar la transacción]

Este error se produce cuando se modifican los mismos datos utilizando varios módulos. Se debe a transacciones SQL.

Cuando se ejecuta cualquier módulo SQL, inicia una transacción. La transacción finaliza después de que el escenario se ejecute completamente.

Si otro módulo intenta acceder a los mismos datos, debe esperar hasta que finalice la transacción anterior. Dado que la primera transacción finalizará después de que finalice el escenario, la segunda transacción nunca puede comenzar.

### Solución:

Active la confirmación automática. La confirmación automática finaliza (confirma) todas las transacciones inmediatamente después de que se haya completado la ejecución del módulo.

1. Haga clic en [!UICONTROL Configuración de escenarios] icono ![](assets/scenario-settings-icon.png)en la parte inferior de la pantalla.
1. Haga clic en **[!UICONTROL Confirmación automática]** casilla de verificación
1. Clic **[!UICONTROL OK]** para guardar la configuración del escenario.
