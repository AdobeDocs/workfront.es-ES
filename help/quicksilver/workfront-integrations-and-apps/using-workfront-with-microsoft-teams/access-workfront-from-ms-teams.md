---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: Acceso [!DNL Adobe Workfront] de [!DNL Microsoft] Equipos
description: Puede acceder a [!DNL Adobe Workfront] de [!DNL Microsoft Teams] y realizar varias acciones en [!DNL Workfront] escribiendo comandos en el canal de bots de Workfront o en cualquier otro canal del equipo.
author: Becky
feature: Workfront Integrations and Apps
exl-id: a12277e8-2c2e-4b53-990f-6ee9a6541492
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 1%

---

# Acceso [!DNL Adobe Workfront] de [!DNL Microsoft Teams]

<!--Audited: 01/2024-->

>[!NOTE]
>
>Actualmente, la integración de Adobe Workfront para Microsoft Teams solo es compatible con la experiencia clásica de Microsoft Teams.

Puede acceder a [!DNL Adobe Workfront] de [!DNL Microsoft Teams] y realizar varias acciones en [!DNL Workfront] escribiendo comandos en el [!DNL Workfront] canal de bots o cualquier otro canal de equipo.

Puede hacer lo siguiente en [!DNL Workfront] de [!DNL Microsoft Teams]:

* Buscar proyectos, tareas o problemas
* Creación de tareas personales
* Responder a notificaciones
* Administrar aprobaciones de documentos

Los comandos que se utilizan en [!DNL Microsoft Teams] realizar estas acciones es diferente en función del canal al que desee acceder [!DNL Workfront] de.

>[!NOTE]
>
>[!DNL Microsoft Teams] ya no es compatible [!DNL Internet Explorer]. Para usar la variable [!DNL Adobe Workfront for Microsoft Teams integration], debe utilizar un explorador web distinto de [!DNL Internet Explorer].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p>
   <p>Actual: [!UICONTROL Trabajo], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Información general sobre los requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Puede crear tareas personales en [!DNL Adobe Workfront] de [!DNL Microsoft Teams] si se cumplen las siguientes condiciones:

* El propietario de un equipo ha instalado y configurado [!DNL Workfront for Microsoft Teams] para su equipo.
* Ha iniciado sesión en [!DNL Workfront] de [!DNL Microsoft Teams].

## Acceso [!DNL Workfront] desde el [!DNL Workfront] canal de chat de bots

Debe iniciar sesión en Workfront.

1. Abra el **[!DNL Workfront]** canal de chat de bots.
1. Haga clic en **[!DNL Workfront]** debajo del campo de texto para mostrar el cuadro de búsqueda.

   ![team_search_box_in_the_bot_channel.PNG](assets/teams-search-box-in-the-bot-channel-350x456.png)

1. Empiece a escribir el nombre de un proyecto, tarea o problema.

   Para obtener información sobre cómo buscar elementos, consulte la sección [Buscar y compartir [!DNL Adobe Workfront] elementos en [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) in the article [Search for and share [!DNL Adobe Workfront] elementos en [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md).

1. Haga clic en **[!UICONTROL Escriba sus preguntas aquí]** field.

   ![ms_team_type_your_questions_here_and_what_can_I_do_fields.png](assets/ms-teams-type-your-questions-here-and-what-can-i-do-fields-350x71.png)

1. Realice una de las siguientes acciones:

   * Clic **[!UICONTROL ¿Qué puedo hacer?]**, entonces **[!UICONTROL Iniciar sesión]** o **[!UICONTROL Cerrar sesión]** de [!DNL Workfront], cree un **[!UICONTROL Nueva tarea]** (tarea personal) en [!DNL Workfront], o consiga **[!UICONTROL Ayuda]** enumerando los comandos disponibles.

   * Acceso [!DNL Workfront] directamente escribiendo un comando en la **[!UICONTROL Escriba sus preguntas aquí]** field.

     Los comandos no distinguen entre mayúsculas y minúsculas.

     El [!DNL Workfront] bot responde con su solicitud en el [!DNL Workfront] canal de chat de bots.

## Acceso [!DNL Workfront] desde un canal de equipo

Debe iniciar sesión en Workfront.

1. Abra un canal de equipo y escriba **@[!DNL Workfront]**, luego seleccione **[!DNL Workfront].**

1. Clic **[!UICONTROL Buscar]** para buscar un proyecto, tarea o problema.

   Para obtener información sobre la búsqueda de elementos, consulte la [Buscar y compartir [!DNL Adobe Workfront] elementos en [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) section in the [Search for and share [!DNL Adobe Workfront] elementos en [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/search-for-and-share-wf-items-in-ms-teams.md) artículo.

1. Escriba cualquiera de los siguientes comandos para realizar estas acciones en Workfront.\
   Los comandos no distinguen entre mayúsculas y minúsculas:

   * **[!UICONTROL Iniciar sesión]** para iniciar sesión en [!DNL Workfront]
   * **[!DNL Log out]** para cerrar la sesión de Workfront
   * **[!DNL New task]** para crear una nueva tarea personal

     Para obtener información sobre cómo crear tareas desde [!DNL Microsoft Teams], consulte [Crear [!DNL Adobe Workfront] tareas de [!DNL Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/create-workfront-tasks-from-ms-teams.md).

   * **[!UICONTROL Ayuda]** para ver una lista de todos los comandos disponibles.

     El [!DNL Workfront] bot responde con su solicitud en el [!DNL Workfront] canal de chat de bots.

1. Vaya a la [!DNL Workfront] canal de chat de bots para acceder a [!DNL Workfront] y complete su solicitud.
