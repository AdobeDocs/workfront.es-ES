---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Acerca de conectar [!DNL Adobe Workfront Fusion] a una aplicación o servicio
description: Para la mayoría de las aplicaciones, es necesario crear una conexión a través de la cual [!DNL Adobe Workfront Fusion] puede comunicarse con el servicio de terceros proporcionado según la configuración del escenario específico.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Acerca de conectar [!DNL Adobe Workfront Fusion] a una aplicación o servicio

Para la mayoría de las aplicaciones, es necesario crear una conexión a través de la cual [!DNL Adobe Workfront Fusion] puede comunicarse con el servicio de terceros proporcionado según la configuración del escenario específico.

Por ejemplo, si desea crear un escenario que recupere información de [!DNL Workfront], debe conceder permiso de acceso para [!DNL Workfront Fusion] para acceder a su [!DNL Workfront] cuenta.

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

## Derechos de acceso

Para cada conexión, [!DNL Workfront Fusion] requiere solo los derechos de acceso necesarios para completar correctamente un escenario determinado. Por ejemplo, si crea un escenario a partir del cual enumerar documentos [!DNL Google Docs], [!DNL Workfront Fusion] no pide permiso para obtener el contenido de los documentos.

Lamentablemente, no todos los servicios permiten limitar el acceso a tareas específicas. Por lo tanto, [!DNL Workfront Fusion] debe requerir derechos de acceso completos. Para obtener más información sobre cómo restringir [!DNL Workfront Fusion] acceso a su cuenta registrada en esos servicios, consulte la documentación específica de la aplicación.

## Acerca de la administración de conexiones

Puede administrar todas las conexiones desde el [!UICONTROL Conexiones] área. Aquí puede:

* Ver los permisos otorgados a [!DNL Workfront Fusion] para cada conexión
* Cambiar nombre de conexiones
* Volver a autorizar conexiones existentes
* Eliminar conexiones existentes
* Compruebe que la conexión al servicio se ha establecido correctamente

Para abrir [!UICONTROL Conexiones] , haga clic en <b>[!UICONTROL Conexiones]</b> en el panel de navegación izquierdo.

## Renovación de una conexión

[!DNL Workfront Fusion] generalmente obtiene derechos de acceso a un servicio determinado durante un período de tiempo ilimitado. Sin embargo, no siempre es así. Con algunos servicios, el permiso de acceso debe renovarse después de un período de tiempo determinado. En estos casos, [!DNL Workfront Fusion] le notifica por correo electrónico poco antes de que caduquen sus derechos de acceso.

Para renovar una conexión:

1. Haga clic en **[!UICONTROL Volver a autorizar]** botón en el **[!UICONTROL Conexiones]** área.
