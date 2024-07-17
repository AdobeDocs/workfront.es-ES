---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Crear tareas y problemas desde el Slack
description: Una vez que haya instalado y configurado  [!DNL Adobe Workfront] for Slack, puede crear tareas y problemas desde Slack y asociarlos a proyectos en Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Crear tareas y problemas a partir de [!DNL Slack]

Después de instalar y configurar [!DNL Adobe Workfront for Slack], puede crear tareas y problemas a partir de [!DNL Slack] y asociarlos a proyectos en [!DNL Workfront].

Para obtener más información sobre la configuración de [!DNL Workfront] con [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Debe tener acceso para crear tareas y problemas en su nivel de acceso y debe tener permisos de [!UICONTROL Contribute] en el proyecto con el que los asocia.

Para obtener más información sobre los niveles de acceso, vea [Información general sobre los niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Para obtener más información acerca de los permisos de los objetos, vea [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].\

## Requisitos previos

Para poder crear tareas y problemas a partir de [!DNL Slack], debe

* Configurar [!DNL Workfront] para el Slack\
   Para obtener instrucciones sobre cómo configurar [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Crear tareas a partir de [!DNL Slack]

1. Inicie sesión en la instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre cómo iniciar sesión en Workfront desde [!DNL Slack], consulte la sección &quot;Iniciar sesión en [!DNL Workfront] desde [!DNL Slack]&quot; en [Acceso [!DNL Adobe Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo de mensaje:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Los comandos distinguen entre mayúsculas y minúsculas. Puede iniciar el comando con `/wf` en lugar de `/workfront`.
   >  
   >Se debe escribir el nombre de tarea tal como aparecerá en la interfaz [!DNL Workfront], sin corchetes ni comillas.

1. (Opcional) Comience a escribir el nombre del proyecto con el que desea asociar la nueva tarea y selecciónela cuando aparezca en la lista.\
   Recibirá una confirmación que indica que la tarea se ha agregado al proyecto seleccionado.
1. (Opcional) Haga clic en el nombre de la tarea en el mensaje de confirmación para abrirla en [!DNL Workfront], en una nueva pestaña del explorador.

## Crear problemas a partir de [!DNL Slack]

1. Inicie sesión en la instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre el inicio de sesión en [!DNL Workfront] desde [!DNL Slack], consulte la sección &quot;Inicio de sesión en [!DNL Workfront] desde [!DNL Slack]&quot; en [Acceso [!DNL Adobe Workfront] desde [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo de mensaje:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Los comandos distinguen entre mayúsculas y minúsculas. Puede iniciar el comando con &#39;/wf&#39; en lugar de &#39;/workfront&#39;. \
   >Se debe escribir el nombre del problema tal como aparecerá en la interfaz [!DNL Workfront], sin corchetes ni comillas.

1. (Opcional) Empiece escribiendo el nombre del proyecto con el que desea asociar el nuevo problema y selecciónelo cuando aparezca en la lista.\
   Recibirá una confirmación que indica que el problema se agregó al proyecto seleccionado.
1. (Opcional) Haga clic en el nombre del problema en el mensaje de confirmación para abrirlo en [!DNL Workfront], en una nueva pestaña del explorador.
