---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Crear tareas y problemas desde el Slack
description: Después de instalar y configurar [!DNL Adobe Workfront] para Slack, puede crear tareas y problemas desde Slack y asociarlos a proyectos en Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Crear tareas y problemas desde [!DNL Slack]

Después de instalar y configurar [!DNL Adobe Workfront for Slack], puede crear tareas y problemas desde [!DNL Slack] y asociarlos a proyectos en [!DNL Workfront].

Para obtener más información sobre la configuración [!DNL Workfront] con [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Debe tener acceso para crear tareas y problemas en el nivel de acceso y tener [!UICONTROL Contribute] permisos en el proyecto con el que los asocia.

Para obtener más información sobre los niveles de acceso, consulte [Información general sobre los niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Para obtener más información sobre los permisos de los objetos, consulte [Información general sobre cómo compartir permisos en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.\

## Requisitos previos

Antes de crear tareas y problemas desde [!DNL Slack], debe

* Configurar [!DNL Workfront] para Slack\
   Para obtener instrucciones sobre la configuración [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Crear tareas desde [!DNL Slack]

1. Inicie sesión en su [!DNL Slack] instancia e inicie sesión en [!DNL Workfront] from [!DNL Slack].\
   Para obtener más información sobre el inicio de sesión en Workfront desde [!DNL Slack], consulte &quot;Inicio de sesión en [!DNL Workfront] from [!DNL Slack]&quot; en [Acceso [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo del mensaje:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Los comandos distinguen entre mayúsculas y minúsculas. Puede iniciar el comando con `/wf` en lugar de `/workfront`.
   >  
   >El nombre de la tarea debe introducirse tal y como aparecerá en el [!DNL Workfront] , sin corchetes ni comillas.\
   >![add_task_to_project.png](assets/add-task-to-project-350x63.png)

1. (Opcional) Empiece a escribir el nombre de un proyecto al que desee asociar la nueva tarea y selecciónela cuando aparezca en la lista.\
   Recibe una confirmación que indica que la tarea se agregó al proyecto seleccionado.
1. (Opcional) Haga clic en el nombre de la tarea en el mensaje de confirmación para abrirla en [!DNL Workfront], en una nueva pestaña del navegador.

## Crear problemas desde [!DNL Slack]

1. Inicie sesión en su [!DNL Slack] instancia e inicie sesión en [!DNL Workfront] from [!DNL Slack].\
   Para obtener más información sobre cómo iniciar sesión en [!DNL Workfront] from [!DNL Slack], consulte &quot;Inicio de sesión en [!DNL Workfront] from [!DNL Slack]&quot; en [Acceso [!DNL Adobe Workfront] from [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo del mensaje:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Los comandos distinguen entre mayúsculas y minúsculas. Puede iniciar el comando con &#39;/wf&#39; en lugar de &#39;/workfront.&#39; \
   >El Nombre del problema debe introducirse tal y como aparecerá en el [!DNL Workfront] , sin corchetes ni comillas.\
   >![slack_add_issue_to_project.png](assets/slack-add-issue-to-project-350x88.png)

1. (Opcional) Empiece a escribir el nombre de un proyecto con el que desee asociar el nuevo problema y selecciónelo cuando aparezca en la lista.\
   Recibirá una confirmación que indica que el problema se agregó al proyecto seleccionado.
1. (Opcional) Haga clic en el nombre del problema en el mensaje de confirmación para abrirlo en [!DNL Workfront], en una nueva pestaña del navegador.
