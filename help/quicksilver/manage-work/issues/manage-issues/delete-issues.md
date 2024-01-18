---
product-area: projects
navigation-topic: manage-issues
title: Eliminar problemas
description: Puede eliminar problemas o solicitudes en Adobe Workfront si tiene el acceso y los permisos correctos para hacerlo.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 1%

---

# Eliminar problemas

<!--Audited: 01/2024-->

Puede eliminar problemas o solicitudes en Adobe Workfront si tiene el acceso y los permisos correctos para hacerlo.

>[!TIP]
>
>&quot;Problemas&quot; y &quot;solicitudes&quot; se usan indistintamente en Workfront. Puede registrar los problemas tanto de los proyectos como de las tareas para indicar el trabajo imprevisto que debe solucionarse. También puede enviar solicitudes que se registren como problemas en un proyecto designado como Cola de solicitudes.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: Colaborador o superior</p>
   <p>Actual: Solicitud o superior</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuración del nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Acceso de visualización o superior a Proyectos y tareas</p>  <p>Para obtener información sobre el acceso a los problemas del nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acceso a los problemas</a>.  </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos sobre el problema</p> <p>Aportar o permisos superiores en el proyecto o tarea</p> <p> Para obtener información sobre la concesión de permisos a los problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront. Para obtener más información sobre los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Consideraciones para eliminar problemas

* El administrador de Workfront o de un grupo debe habilitar la eliminación de problemas en un proyecto que tenga el estado Completo en el área de Preferencias del proyecto. Para obtener información sobre la configuración de preferencias de proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si el problema ha registrado horas, el administrador de Workfront o de un grupo debe permitir la eliminación de estos problemas configurando las Preferencias de tarea y problema en la instancia de Workfront. Esto también se aplica cuando intenta eliminar proyectos que tienen problemas con horas registradas en ellos.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Para obtener más información sobre cómo habilitar la eliminación de problemas en los que se registran horas, consulte la sección &quot;Eliminación&quot; en [Configurar las preferencias de tareas y problemas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Impacto de la eliminación de problemas

Cuando se elimina un problema, se afectan otros objetos vinculados al problema.

Los siguientes objetos adjuntos a un problema también se eliminan al eliminar un problema:

* Documentos

  No se puede eliminar un problema que tenga adjunto un documento desprotegido. Para obtener más información sobre la retirada de documentos, consulte [Desproteger documentos](../../../documents/managing-documents/check-out-documents.md).

* Notas
* Rutas de aprobación

Según la configuración de Workfront o del administrador del grupo en las Preferencias de eliminación de proyectos, tareas o problemas en **Hoja de horas y preferencias de horas** En la instancia de Workfront, las horas registradas para los problemas se gestionan de una de las siguientes maneras al eliminar un problema:

* Mover al proyecto y no se restaurará en el problema, si el problema se restaura más adelante.
* Se eliminarán y se restaurarán en función del problema si este se restaura más adelante.

  Esto también se aplica cuando intenta eliminar proyectos que tienen tareas con horas registradas en ellos.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

  Para obtener más información sobre la configuración de las preferencias de eliminación para los problemas de horas de sesión, consulte [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Los usuarios asignados al problema o a la aprobación del problema permanecen en el equipo del proyecto.\
  Para obtener más información sobre los equipos de proyecto, consulte [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Eliminar problemas

* [Eliminar varios problemas en un proyecto simultáneamente](#delete-multiple-issues-in-a-project-simultaneously)
* [Eliminar un solo problema](#delete-a-single-issue)

### Eliminar varios problemas en un proyecto simultáneamente  {#delete-multiple-issues-in-a-project-simultaneously}

1. Vaya a la **Menú principal**.
1. Clic **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene los problemas que desea eliminar.
1. Clic **Problemas** en el panel izquierdo.
1. Seleccione un problema y haga clic en **Eliminar** icono ![](assets/delete.png) al principio de la lista.

1. Si la eliminación está permitida, haga clic en **Sí, eliminarla**.\
   Es posible que el administrador de Workfront no permita la eliminación de problemas en los que se registran horas.\
   Para obtener más información sobre el acceso y los permisos necesarios para eliminar un problema, consulte [Eliminar problemas](#access-and-permissions-needed).

### Eliminar un solo problema {#delete-a-single-issue}

{{step1-to-projects}}

1. Haga clic en el nombre del proyecto que contiene el problema que desea eliminar.
1. Clic **Problemas** en el panel izquierdo.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Haga clic en el nombre del problema que desee eliminar.
1. Haga clic en **Más** a la derecha del nombre del problema.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Clic **Eliminar problema**.
1. Si la eliminación está permitida, haga clic en **Sí, eliminarla**.

   Es posible que el administrador de Workfront no permita la eliminación de problemas en los que se registran horas.\
   Para obtener más información sobre el acceso y los permisos necesarios para eliminar un problema, consulte [Eliminar problemas](#access-and-permissions-needed).

## Restaurar problemas eliminados

Un administrador de Workfront o de grupo puede restaurar los problemas en un plazo de 30 días después de eliminarlos. Para obtener más información sobre la restauración de elementos en Workfront, consulte [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
