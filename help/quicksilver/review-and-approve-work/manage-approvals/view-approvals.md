---
product-area: projects
navigation-topic: approvals
title: Ver aprobaciones
description: Los procesos de aprobación proporcionan la flexibilidad para crear aprobaciones de varios pasos para proyectos, tareas y problemas. Los administradores de Adobe Workfront definen los procesos de aprobación para proporcionar coherencia en todo el sistema.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: b0b83e8a8a2a076ec20691183605e3d25d10129d
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Ver aprobaciones

Los procesos de aprobación proporcionan la flexibilidad para crear aprobaciones de varios pasos para proyectos, tareas y problemas. Los administradores de Adobe Workfront definen los procesos de aprobación para proporcionar coherencia en todo el sistema.

Para obtener información acerca de cómo crear procesos de aprobación, vea [Crear un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Para obtener información acerca de cómo asociar aprobaciones con trabajo en Workfront, vea [Asociar un proceso de aprobación nuevo o existente con trabajo](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a los objetos asociados con las aprobaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores a los objetos asociados con las aprobaciones o</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

+++

## Localización de aprobaciones en Adobe Workfront

Puede ver o administrar las aprobaciones de varias áreas de Workfront. Para obtener información sobre cómo administrar aprobaciones en diversas áreas, consulte [Aprobación de trabajo](../../review-and-approve-work/manage-approvals/approving-work.md).

Puede ver o administrar aprobaciones desde las siguientes áreas:

* En el área de Inicio

   * Todos los proyectos, tareas, problemas, plantillas de horas, documentos y accesos pendientes de su aprobación se muestran en el widget Mis aprobaciones en el área de Inicio.
   * Las aprobaciones que usted mismo ha enviado también se muestran en el widget Mis aprobaciones del área de Inicio al elegir la opción de filtro Aprobaciones que he enviado. Para obtener más información, consulte la sección [Revisar el trabajo que envía para su aprobación en el área de inicio](#review-work-you-submit-for-approval-in-the-home-area) de este artículo.
   * Las aprobaciones se eliminan del widget Mis aprobaciones en el área de Inicio cuando el proyecto, tarea o problema asociado está marcado como Resuelto, En espera, Cerrado o Cancelado.

  Para obtener información sobre cómo usar Inicio, consulte [Introducción a Inicio](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* En el encabezado de un proyecto, tarea, problema, documento o prueba
* En la sección Aprobaciones de un proyecto, tarea o problema
* En un informe

  >[!NOTE]
  >
  >No se puede tomar una decisión sobre una aprobación de un informe.

  Puede crear un informe de aprobación de proyecto, tarea, problema o documento que contenga información de aprobación.

  Para obtener información sobre cómo crear informes, consulte [Crear un informe personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Revise el trabajo que envía para su aprobación en el área de Inicio {#review-work-you-submit-for-approval-in-the-home-area}

1. Haga clic en **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Haga clic en **Personalizar** para agregar el widget **Mis aprobaciones**.
1. (Condicional) Haga clic en el menú desplegable **Filtro** y, a continuación, seleccione **Aprobaciones que he enviado** para ver las aprobaciones que ha enviado.


## Ver el estado de aprobación de un objeto

Puede ver el estado de aprobación de un objeto en las siguientes secciones del objeto:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Actualizaciones </td> 
   <td> <p>Muestra todos los estados de aprobación cuando se producen. Los estados de aprobación se muestran en línea con otros estados mostrados en la sección <strong>Actualizaciones</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rutas de aprobación</td> 
   <td> <p>Muestra información más detallada sobre el proceso de aprobación, como cada fase del proceso de aprobación y si los aprobadores han concedido la aprobación.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Utilice el área de Actualizaciones para ver un estado de aprobación {#use-the-updates-area-to-view-an-approval-status}

Cuando se inicia una aprobación en un proyecto, tarea o problema, se muestra un estado en la pestaña **Actualizaciones** del objeto, que indica el estado de aprobación. Aparece un nuevo estado cada vez que el objeto pasa por el proceso de aprobación. Esto incluye los siguientes eventos:

* Se inicia un proceso de aprobación en un objeto. El proceso de aprobación se inicia cuando se cambia el estado.
* El objeto se rechaza
* Se aprueba el objeto

>[!TIP]
>
>Si se aplica una aprobación a una tarea, las actualizaciones de aprobación se muestran en la pestaña Actualizaciones de la tarea, no en la pestaña Actualizaciones del proyecto donde reside la tarea.

### Utilice el área de Aprobaciones para ver un estado de aprobación {#use-the-approvals-area-to-view-an-approval-status}

Puede obtener visibilidad sobre dónde se encuentra actualmente una tarea o un problema en el que está trabajando en el proceso de aprobación. Puede ver la siguiente información:

* La fase del proceso de aprobación
* Qué aprobadores ya lo han aprobado
* Qué aprobadores aún no lo han aprobado

Para ver el estado actual de dónde se encuentra una tarea o un problema en el proceso de aprobación:

1. Vaya al proyecto, tarea o problema con el que está asociada la aprobación.
1. En el panel izquierdo, haga clic en **Aprobaciones**. Es posible que primero tengas que hacer clic en **Mostrar más**.

   La pestaña Approvals muestra la información completa sobre todas las rutas y etapas de aprobación anteriores. Puede ver exactamente quién tomó una decisión sobre la aprobación o si la aprobación está establecida para un equipo, rol de trabajo o usuario.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Para obtener información acerca de cómo crear un proceso de aprobación, vea [Crear un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
