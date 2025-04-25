---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Administrar su trabajo y aprobaciones desde Slack
description: Puede acceder a su Lista de trabajos en Inicio, revisar y aceptar trabajar en tareas y problemas, y revisar o tomar decisiones sobre aprobaciones directamente desde Slack.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 99%

---

# Administrar su trabajo y aprobaciones desde [!DNL Slack]

Después de instalar [!DNL Adobe Workfront for Slack], puede hacer lo siguiente:

* Acceder a listas de sus elementos de la página [!UICONTROL Inicio] desde [!DNL Slack]
* Revisar y aceptar para trabajar en tareas y problemas desde [!DNL Slack]
* Revisar y tomar decisiones sobre aprobaciones desde [!DNL Slack]

Para obtener más información sobre la configuración de [!DNL Workfront] con [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan <a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Para poder administrar su trabajo y las aprobaciones desde [!DNL Slack], debe

* Configurar [!DNL Workfront for Slack]\
  Para obtener instrucciones sobre cómo configurar [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Administrar su trabajo desde [!DNL Slack]

1. Inicie sesión en la instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre el inicio de sesión en [!DNL Workfront] desde [!DNL Slack], consulte la sección “Inicio de sesión en [!DNL Workfront] desde [!DNL Slack]” en [Acceso a  [!DNL Adobe Workfront]  desde  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo de mensaje:

   `/workfront home`

   >[!NOTE]
   >
   >* Los comandos distinguen entre mayúsculas y minúsculas.
   >* Puede iniciar el comando con `/wf` en lugar de `/workfront`.

   Se muestran los botones desde los cuales puede acceder a las listas de tareas, problemas y visualización de aprobaciones. Al hacer clic en uno de los botones, se muestran los primeros 20 elementos de cada lista en [!DNL Slack].

1. (Opcional) Haga clic en **[!UICONTROL Tareas]** para mostrar todas las tareas.

   Para obtener más información acerca de la administración de tareas en [!DNL Slack], vea [Administrar tareas desde  [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Opcional) Haga clic en **[!UICONTROL problemas]** para mostrar todos sus problemas.

   Para obtener más información sobre la administración de problemas en [!DNL Slack], consulte [Administración de problemas desde  [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Opcional) Haga clic en **[!UICONTROL Approvals]** para mostrar todas las aprobaciones que están a la espera de su decisión.\
   Para obtener más información sobre cómo administrar las aprobaciones en [!DNL Slack], consulte [Administrar las aprobaciones desde  [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Administrar sus tareas desde [!DNL Slack] {#manage-your-tasks-from-slack}

1. Inicie sesión en su instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener información sobre cómo iniciar sesión en [!DNL Workfront] desde [!DNL Slack], consulte la sección “Iniciar sesión en [!DNL Workfront] desde [!DNL Slack]” en [Acceso a  [!DNL Adobe Workfront]  desde  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir cualquiera de los siguientes comandos en el campo de mensaje:

   `/workfront home`, a continuación, haga clic en **[!UICONTROL Tasks]**

   O

   `/workfront tasks`

   >[!NOTE]
   >
   >* Los comandos distinguen entre mayúsculas y minúsculas.
   >* Puede iniciar el comando con `/wf` en lugar de `/workfront`.

   Se muestran las 20 primeras tareas de la lista.

1. Haga clic en **[!UICONTROL +`<remaining number>` more]** para mostrar tareas adicionales.
1. Considere la posibilidad de revisar la siguiente información sobre los elementos de trabajo:

   * **[!UICONTROL Nombre]**
   * **[!UICONTROL Nombre del proyecto]** o **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** del elemento de trabajo.
   * **[!DNL Assigned By Name]**: este es el nombre del usuario que le asignó la tarea.
   * **[!UICONTROL Estado]**

1. (Opcional) Haga clic en el nombre de un elemento para abrirlo en Workfront en una pestaña independiente del explorador.
1. (Opcional) En el campo **[!UICONTROL Status]**, seleccione un nuevo Estado.
1. (Opcional) Haga clic en **[!UICONTROL Log Time]** y, a continuación, seleccione un **[!UICONTROL Hour Type]** y una cantidad de horas para registrar el tiempo en el elemento.

   >[!NOTE]
   >
   >* Solo puede registrar horas en incrementos de una hora completa o media, hasta 12 horas y 30 minutos.
   >* Las horas que registre tienen una fecha de entrada de hoy. No puede registrar horas para una fecha pasada o futura desde [!DNL Slack].

   Recibirá una confirmación de que se ha registrado la hora.

1. (Opcional) Haga clic en **[!UICONTROL Work on it]** para aceptar trabajar en una tarea. El botón [!UICONTROL Work on it] desaparece.

## Administrar sus problemas desde [!DNL Slack] {#manage-your-issues-from-slack}

1. Inicie sesión en la instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre cómo iniciar sesión en [!DNL Workfront] desde [!DNL Slack], consulte [Iniciar sesión en  [!DNL Workfront]  desde  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront]  desde  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir cualquiera de los siguientes comandos en el campo de mensaje:

   `/workfront home`, a continuación, haga clic en **[!UICONTROL Issues]**.

   O

   `/workfront issues`

   >[!NOTE]
   >
   >* Los comandos distinguen entre mayúsculas y minúsculas.
   >* Puede comenzar el comando con `/wf` en lugar de `/workfront`.

   Se muestran los 20 primeros problemas de la lista.

1. Haga clic en **[!UICONTROL + remaining `<number>` more]** para mostrar elementos adicionales.
1. Considere la posibilidad de revisar la siguiente información sobre los elementos de trabajo:

   * **[!UICONTROL Nombre]**
   * Nombre del **[!UICONTROL Project]** o nombre del objeto principal
   * Fecha de **[!UICONTROL Due on]**: esta es la fecha planificada de finalización del elemento de trabajo.
   * Nombre de **[!DNL Requested by]**: este es el contacto principal (para problemas) o el usuario que realizó la asignación (para tareas).

1. (Opcional) Haga clic en el nombre del problema para abrirlo en Workfront en una pestaña independiente del explorador.
1. (Opcional) Haga clic en **[!DNL Work on it]** para comenzar a trabajar en los problemas que aún no ha aceptado.

   El botón [!UICONTROL Work on it] desaparece.

## Administrar sus aprobaciones desde [!DNL Slack] {#manage-your-approvals-from-slack}

1. Inicie sesión en su instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre el inicio de sesión en [!DNL Workfront] desde [!DNL Slack], consulte la sección “Inicio de sesión en [!DNL Workfront] desde [!DNL Slack]” en [Acceder a [!DNL Adobe Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir cualquiera de los siguientes comandos en el campo de mensaje:

   `/workfront home`, a continuación, haga clic en **[!UICONTROL Approvals]**

   O

   `/workfront approvals`

   >[!NOTE]
   >
   >* Los comandos distinguen entre mayúsculas y minúsculas.
   >* Puede iniciar el comando con `/wf` en lugar de `/workfront`.

   Se muestran los primeros 20 elementos de su lista **[!UICONTROL Approvals]**. También se muestra información adicional sobre los elementos, como el nombre del usuario que lo solicitó o el nombre del proyecto al que pertenece el elemento.

1. Haga clic en **[!UICONTROL + remaining `<number>` more]** para mostrar elementos adicionales.

1. Considere la posibilidad de administrar aprobaciones para los siguientes objetos:

   * **Proyectos**

     Haga clic en **[!UICONTROL Approve]** o **[!UICONTROL Reject]** para aceptar o rechazar el cambio de estado de un proyecto.

   * **Tareas**

     Haga clic en **[!UICONTROL Approve]** o **[!UICONTROL Reject]** para aceptar o rechazar el cambio de estado de una tarea.

   * **Problemas**

     Haga clic en **[!UICONTROL Approve]** o **[!DNL Reject]** para aceptar o rechazar el cambio de estado de un problema.

   * **Documentos**

     Haga clic en **[!UICONTROL Approve]** para aprobar un documento, en **[!UICONTROL Reject]** para rechazarlo o en **[!UICONTROL Changes]** para indicar que lo aprueba pero que el documento necesita cambios adicionales.\
     (Opcional) Pase el puntero por encima de la miniatura del documento para hacer clic en la lupa y previsualizar el documento.

   * **Pruebas** haga clic en el nombre de la revisión para abrirla en [!DNL Workfront] en una pestaña separada y administrar la aprobación.
   * **Solicitudes de acceso**

     Haga clic en **[!UICONTROL Grant Access]** para conceder permisos mejorados al objeto solicitado o en **[!UICONTROL Ignore]** para omitir la solicitud de más acceso.

1. (Opcional) Haga clic en el nombre del objeto enviado para su aprobación con el fin de abrirlo en [!DNL Workfront] en una nueva pestaña del explorador.
