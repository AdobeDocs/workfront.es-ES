---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Información general sobre Conexiones
description: Para la mayoría de las aplicaciones, es necesario crear una conexión a través de la cual [!DNL Adobe Workfront Fusion] puede comunicarse con el servicio de terceros proporcionado según la configuración del escenario específico.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Información general sobre Conexiones

<!-- Audited: 3/2024-->

Para la mayoría de las aplicaciones, [!DNL Workfront Fusion] requiere una conexión, a través de la cual puede comunicarse con el servicio de terceros proporcionado según la configuración del escenario específico.

Por ejemplo, si desea crear un escenario que recupere información de [!DNL Workfront], debe conceder permiso de acceso para [!DNL Workfront Fusion] para acceder a su [!DNL Workfront] cuenta.

Una conexión representa la autorización y los permisos que Fusion utiliza para acceder a la aplicación. Puede crear una o más conexiones para cada aplicación y puede utilizar la misma conexión en varios módulos o escenarios.

La mayoría de las conexiones se utilizan solo para una aplicación. Por ejemplo, una [!DNL Workfront] no se puede usar la conexión en un [!UICONTROL Salesforce] módulo. Algunos [!DNL Adobe] Las aplicaciones de pueden compartir conexiones. Para obtener más información, consulte los artículos de esas aplicaciones, enumerados en [Aplicaciones y sus módulos](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

Las conexiones se administran en el equipo. Todos los miembros de un equipo tienen acceso a las conexiones del equipo y los usuarios que no pertenecen a un equipo no tienen acceso a las conexiones del equipo.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p><p>O</p><p>Actual: [!UICONTROL Work] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Heredado: cualquiera </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Nuevo:</p> <ul><li>[!UICONTROL Seleccionar] o [!UICONTROL Prime] [!DNL Workfront] Plan: su organización debe comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] está incluido.</li></ul>
   <p>O</p>
   <p>Actual: Su organización debe comprar [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Derechos de acceso

Para cada conexión, [!DNL Workfront Fusion] requiere solo los derechos de acceso necesarios para completar correctamente un escenario determinado. Por ejemplo, si crea un escenario a partir del cual enumerar documentos [!DNL Google Docs], [!DNL Workfront Fusion] no pide permiso para obtener el contenido de los documentos. Posteriormente, si descubre que necesita acceder al contenido de los documentos, puede actualizar la conexión o crear una nueva que pueda acceder a dicho contenido.

No todos los servicios permiten limitar el acceso a tareas específicas. En estos casos, [!DNL Workfront Fusion] debe requerir derechos de acceso completos. Para obtener más información sobre cómo restringir [!DNL Workfront Fusion] acceso a su cuenta registrada en esos servicios, consulte la documentación específica de la aplicación que se enumera en [Aplicaciones y sus módulos](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Administrar conexiones

Puede administrar todas las conexiones desde el [!UICONTROL Conexiones] área.

>[!NOTE]
>
>Las conexiones son propiedad de los equipos. Si no encuentra la conexión que busca, compruebe que está viendo el equipo correcto.
>
>Para seleccionar un nuevo equipo:
>
>* Haga clic en el nombre del equipo en el panel de navegación izquierdo y seleccione un nuevo equipo.
>
>    O
>
>* Haga clic en Información general del equipo en el panel de navegación izquierdo y, a continuación, haga clic en la flecha desplegable situada junto al nombre del equipo, en la parte superior de la página. Seleccione un nuevo equipo.

1. Para abrir [!UICONTROL Conexiones] , haga clic en <b>[!UICONTROL Conexiones]</b> en el panel de navegación izquierdo.
1. (Opcional) Indique el entorno y el tipo de conexión haciendo clic en la lista desplegable Entorno y tipo y seleccionando una opción.
1. (Opcional) Para ver qué permisos se han concedido a [!DNL Workfront Fusion] para una conexión, haga clic en el icono Ver ![Ver permisos de conexión](assets/view-connection-permissions.png) para esa conexión.
1. (Opcional) Para cambiar el nombre de una conexión, resalte el nombre de la conexión y escriba el nuevo nombre.
1. (Opcional) Para volver a autorizar una conexión, haga clic en **Volver a autorizar** para esa conexión.
1. (Opcional) Para eliminar una conexión, haga clic en **Eliminar** para esa conexión.
1. (Opcional) Para comprobar que la conexión con el servicio se ha establecido correctamente, haga clic en **Verificar** para la conexión.



## Renovación de una conexión

[!DNL Workfront Fusion] generalmente obtiene derechos de acceso a un servicio determinado durante un período de tiempo ilimitado. Algunas aplicaciones requieren que el permiso de acceso se renueve después de un período de tiempo determinado. En estos casos, [!DNL Workfront Fusion] le notifica por correo electrónico poco antes de que caduquen sus derechos de acceso.

Para renovar una conexión:

1. Haga clic en **[!UICONTROL Volver a autorizar]** botón en el **[!UICONTROL Conexiones]** área.
