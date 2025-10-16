---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Crear tareas y problemas desde Slack
description: Una vez que haya instalado y configurado  [!DNL Adobe Workfront]  para Slack, puede crear tareas y problemas desde Slack y asociarlos a proyectos en Workfront.
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 99%

---

# Crear tareas y problemas desde [!DNL Slack]

Después de instalar y configurar [!DNL Adobe Workfront for Slack], puede crear tareas y problemas desde [!DNL Slack] y asociarlos a proyectos en [!DNL Workfront].

Para obtener más información sobre la configuración de [!DNL Workfront] con [!DNL Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Debe tener acceso para crear tareas y problemas en su nivel de acceso y debe tener permisos de [!UICONTROL Contribute] en el proyecto con el que los asocia.

Para obtener más información sobre los niveles de acceso, vea [Información general sobre los niveles de acceso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). Para obtener más información sobre los permisos a objetos, vea [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Cualquiera</p>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para poder crear tareas y problemas desde [!DNL Slack], debe

* Configurar [!DNL Workfront] para Slack\
   Para obtener instrucciones sobre cómo configurar [!DNL Workfront for Slack], consulte [Configurar [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Crear tareas desde [!DNL Slack]

1. Inicie sesión en la instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre cómo iniciar sesión en Workfront desde [!DNL Slack], consulte la sección “Iniciar sesión en [!DNL Workfront] desde [!DNL Slack]” en [Acceso a  [!DNL Adobe Workfront]  desde  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo de mensaje:

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >Los comandos distinguen entre mayúsculas y minúsculas. Puede comenzar el comando con `/wf` en lugar de `/workfront`.
   >  
   >Se debe escribir el nombre de tarea tal como aparecerá en la interfaz de [!DNL Workfront], sin corchetes ni comillas.

1. (Opcional) Comience a escribir el nombre del proyecto con el que desea asociar la nueva tarea y selecciónela cuando aparezca en la lista.\
   Recibirá una confirmación que indica que la tarea se ha añadido al proyecto seleccionado.
1. (Opcional) Haga clic en el nombre de la tarea del mensaje de confirmación para abrirla en [!DNL Workfront], en una nueva pestaña del explorador.

## Crear problemas desde [!DNL Slack]

1. Inicie sesión en su instancia de [!DNL Slack] e inicie sesión en [!DNL Workfront] desde [!DNL Slack].\
   Para obtener más información sobre el inicio de sesión en [!DNL Workfront] desde [!DNL Slack], consulte la sección “Inicio de sesión en [!DNL Workfront] desde [!DNL Slack]” en [Acceso a  [!DNL Adobe Workfront]  desde  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Desde cualquier canal, empiece a escribir el siguiente comando en el campo de mensaje:

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >Los comandos distinguen entre mayúsculas y minúsculas. Puede comenzar el comando con &#39;/wf&#39; en lugar de &#39;/workfront&#39;. \
   >Se debe escribir el nombre del problema tal como aparecerá en la interfaz [!DNL Workfront], sin corchetes ni comillas.

1. (Opcional) Empiece escribiendo el nombre del proyecto con el que desea asociar el nuevo problema y selecciónelo cuando aparezca en la lista.\
   Recibirá una confirmación que indica que el problema se añadió al proyecto seleccionado.
1. (Opcional) Haga clic en el nombre del problema del mensaje de confirmación para abrirlo en [!DNL Workfront], en una nueva pestaña del explorador.
