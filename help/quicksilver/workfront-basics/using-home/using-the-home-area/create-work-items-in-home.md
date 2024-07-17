---
product-area: projects
navigation-topic: use-the-home-area
title: Crear elementos de trabajo desde el área de Inicio
description: Puede crear elementos de trabajo desde el área [!UICONTROL Inicio]. Puede crear tareas personales, solicitar trabajo a otros usuarios o agregar tareas a proyectos específicos.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: 9db6e509-ea6a-493a-9d86-21a163da1915
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Crear elementos de trabajo desde el área de Inicio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From Courtney: Need to rename)</p>
-->

Puede crear elementos de trabajo desde el área [!UICONTROL Inicio]. Puede crear tareas personales, solicitar trabajo a otros usuarios o agregar tareas a proyectos específicos.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Trabajo] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>[!UICONTROL Worker]</p> <p><b>NOTA</b></p> 
   <p>Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Acceso a [!UICONTROL Edit] o superior en tareas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Crear una tarea personal

Puede crear una tarea personal que solo esté disponible para usted en el área [!UICONTROL Inicio]:

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. Haga clic en **[!UICONTROL Nueva tarea]** > **[!UICONTROL Personal]**.

   ![](assets/creating-work-items-new-task-personal-nwe-350x228.png)

1. En el campo **[!UICONTROL Nombre]**, especifique un nombre para la tarea.
1. (Opcional) Haga clic en **[!UICONTROL Seleccionar fecha]** y, a continuación, seleccione la fecha en la que vence la tarea. Esto establece la [!UICONTROL fecha planificada de finalización] de la tarea.\
   Puede cambiar la **[!UICONTROL Fecha planificada de finalización]** haciendo clic en la fecha en el panel derecho o editando **[!UICONTROL Esto se completará para la fecha]** directamente en la tarea.

1. Haga clic en **[!UICONTROL Crear]** para guardar la tarea.\
   La tarea se le ha asignado y está disponible en el área [!UICONTROL Inicio].

>[!NOTE]
>
>* Cuando crea una tarea personal, se almacena en un proyecto &quot;oculto&quot; en el que no se pueden realizar búsquedas en [!UICONTROL Workfront]. El nombre del proyecto es &quot;&lt; Nombre de usuario >&#39;s Tasks&quot;. El &quot;Nombre de usuario&quot; es el nombre completo del usuario que creó la tarea. Solo puede tener acceso a este proyecto si hace clic en la tarea personal en el área [!UICONTROL Inicio], desde la ruta de exploración de la tarea, por ejemplo.
>
>* A diferencia de las tareas de proyecto normales, las tareas personales tienen un conjunto limitado de campos visibles en la interfaz de Workfront y no influyen en la cronología ni en el progreso de ningún proyecto. Reasignar una tarea personal a otro usuario agrega todos los campos de tarea a una tarea personal, pero la tarea permanece en el proyecto personal del usuario que creó la tarea.
>
>
>* Las tareas personales solo se muestran en las hojas de horas cuando se han registrado horas o cuando están ancladas en la hoja de horas. Solo puede anclar una tarea personal a una plantilla de horas cuando hay horas registradas para la tarea. Para obtener más información, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).
> 
>* Le recomendamos que cree un proyecto y le transfiera cualquier tarea personal si desea que las tareas personales formen parte del flujo de trabajo normal.
>
> ![[!UICONTROL Proyecto para tareas personales]](assets/createworkitems-personal--project-350x105.png)

## Solicitar trabajo de otro usuario

Puede solicitar trabajo a otro usuario directamente desde el área de Inicio. Cuando solicita trabajo de otro usuario como se describe en esta sección, la tarea se muestra como una solicitud en el área de Inicio del usuario hasta que el usuario haga clic en **[!UICONTROL Trabajar en ello]**.

Para solicitar trabajo de otro usuario del área [!UICONTROL Hogar]:

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. Haga clic en **[!UICONTROL Nueva tarea]** y, a continuación, seleccione **[!UICONTROL Solicitud]**.

   ![](assets/creating-work-items-new-task-request-nwe-350x283.png)

1. En el campo **[!UICONTROL Nombre]**, especifique un nombre para la tarea.
1. En el campo **[!UICONTROL Asignar a]**, empiece a escribir el nombre del usuario, equipo o rol que desea asignar y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.
1. En el menú desplegable [!UICONTROL Agregar como], seleccione si desea agregar una tarea o un problema.
1. Haga clic en **[!UICONTROL Seleccionar fecha]** y, a continuación, seleccione la fecha y la hora en que vence la tarea.
1. Haga clic en **[!UICONTROL Crear]** para guardar la tarea.\
   La tarea se muestra como una solicitud de trabajo en el área [!UICONTROL Hogar] del usuario que designó.

## Agregar una tarea o un problema a un proyecto

Puede agregar una tarea o un problema a un proyecto existente directamente desde el área de Inicio:

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **Inicio**.
1. Haga clic en **[!UICONTROL Nueva tarea]** y luego seleccione **[!UICONTROL Tarea de proyecto]**.

   ![](assets/creating-work-items-new-project-task-nwe-350x358.png)

1. En el campo **[!UICONTROL Nombre]**, especifique un nombre para la tarea o el problema.
1. En el campo **[!UICONTROL Asignar a]**, empiece a escribir el nombre del usuario, equipo o rol que desea asignar y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.
1. Empiece escribiendo el nombre del proyecto donde desea crear la tarea o el problema y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.

   >[!IMPORTANT]
   >
   >La tarea o el problema solo aparecen en la [!UICONTROL Lista de trabajos] cuando el proyecto [!UICONTROL Estado] está establecido en [!UICONTROL Actual].

1. (Condicional) Para crear un problema, selecciona **[!UICONTROL Problema]** en el menú desplegable **[!UICONTROL Agregar como]**. De manera predeterminada, **[!UICONTROL Tarea]** está seleccionada.

1. Haga clic en **[!UICONTROL Seleccionar fecha]** y, a continuación, seleccione la fecha y la hora en que vence la tarea.
1. Haga clic en **[!UICONTROL Crear]** para guardar la tarea.
