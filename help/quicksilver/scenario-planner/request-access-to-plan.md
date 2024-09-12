---
product-area: enterprise-scenario-planner-product-area
keywords: plan, permisos, compartir, iniciativas, escenarios, escenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Solicitar acceso a un plan en el Scenario Planner
description: Puede solicitar acceso a un plan en el planificador de escenarios de Adobe Workfront cuando el vínculo al plan se comparta con usted.
author: Alina
feature: Workfront Scenario Planner
exl-id: fa47cb8c-a3ca-4748-b67d-2d8ed34b9b4a
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# Solicitar acceso a un plan en [!DNL Scenario Planner]

Puede solicitar acceso a un plan en [!DNL Adobe Workfront Scenario Planner] cuando el vínculo al plan se comparta con usted.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nuevo: Ultimate </p></li>
   <p>El planificador de escenarios no está disponible para el nuevo plan Workfront Select o Workfront. </p>
   <li><p>Actual: [!UICONTROL Empresa] o superior</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licencia*</p> </td> 
   <td> <p>Nuevo: claro o superior</p> 
   <p>Actual: [!UICONTROL Review] o superior</p> </td> 
  </tr> 
  <tr> 
   <td>Producto* </td> 
   <td> <ul><li><p>Para los nuevos planes de Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Para los planes actuales de Workfront: </p>
   <p>Adobe Workfront</p> <p>Planificador de escenarios de Adobe Workfront</p></li></ul>

<p>Para obtener más información, consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acceso necesario para utilizar [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nivel de acceso </td> 
   <td>  <p>[!UICONTROL View] o acceso superior al [!DNL Scenario Planner]</p>  </td> 
  </tr>
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso a la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder solicitar acceso a un plan en [!DNL Scenario Planner], debe contar con lo siguiente:

* Un vínculo al plan.

>[!NOTE]
>
>Si no tiene derechos de nivel de acceso a [!DNL Scenario Planner] y trata de obtener acceso a un plan desde un vínculo, no puede solicitar acceso al plan. En su lugar, aparece una pantalla que le informa de que debe ponerse en contacto con el administrador de [!DNL Workfront].

## Solicitar acceso para planes en [!DNL Workfront Scenario Planner]

Si todavía no tiene permisos de un plan y navega a él desde un vínculo compartido con usted, se muestra una pantalla para informarle de que no tiene permisos para ver el plan. Se le pedirá que solicite permisos al creador del plan.

>[!TIP]
>
>Solo puede solicitar permisos al propietario o al creador de un plan. No puede solicitar permisos a otros usuarios que también tengan acceso al plan.

Para solicitar permisos:

1. Haga clic en un vínculo a un plan.

   ![](assets/request-access-to-plan-350x277.png)

1. En el menú desplegable **[!UICONTROL Solicitar acceso a]**, indique qué nivel de permisos desea que se le concedan. Seleccione una de las siguientes opciones:

   * [!UICONTROL Vista]
   * [!UICONTROL Administrar]

   No puede solicitar un permiso superior a su nivel de acceso a [!DNL Scenario Planner]. Por ejemplo, no puede solicitar los permisos de [!UICONTROL Administrar] si cuenta con acceso de visualización para [!DNL Scenario Planner].

   Para obtener información acerca de los diferentes niveles de permisos, vea [Compartir un plan en [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

   Para obtener información sobre cómo un administrador de Workfront puede administrar el acceso a [!DNL Scenario Planner], consulte [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Opcional) Escriba un comentario o una solicitud en el **[!UICONTROL cuadro Dejar comentario]** y, a continuación, haga clic en **[!UICONTROL Solicitar acceso]**.

   Lo siguiente sucede:

   * [!DNL Workfront] envía una notificación por correo electrónico al propietario del plan para que conceda los permisos solicitados.\
     ![](assets/request-access-to-plan-email-350x156.png)

   * Una vez que el propietario del plan conceda los permisos solicitados, recibirá un mensaje de correo electrónico informándole de que los permisos se han concedido si el administrador de [!DNL Workfront] tiene habilitada la notificación de uso compartido de objetos a usuarios en su sistema y si habilita la notificación de correo electrónico [!UICONTROL Alguien comparte un objeto conmigo] en su perfil.

     ![](assets/access-granted-to-plan-email-350x172.png)

   * También puede conceder permisos a planes del área [!UICONTROL Hogar] y de la aplicación móvil [!DNL Workfront].

   Para obtener información acerca de cómo habilitar las notificaciones del sistema, vea [Configurar notificaciones de eventos para todos los usuarios del sistema](../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Para obtener información acerca de cómo habilitar las notificaciones en el perfil, vea [Notificaciones: Información diversa](../workfront-basics/using-notifications/notifications-misc-information.md).
