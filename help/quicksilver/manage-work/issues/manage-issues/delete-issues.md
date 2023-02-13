---
product-area: projects
navigation-topic: manage-issues
title: Eliminar problemas
description: Puede eliminar problemas o solicitudes en Adobe Workfront si tiene el acceso y los permisos correctos para hacerlo.
author: Alina
feature: Work Management
exl-id: 31cc802f-7fa6-420c-8494-a45313df1f10
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# Eliminar problemas

Puede eliminar problemas o solicitudes en Adobe Workfront si tiene el acceso y los permisos correctos para hacerlo.

>[!TIP]
>
>Los &quot;problemas&quot; y las &quot;solicitudes&quot; se utilizan de forma intercambiable en Workfront. Puede registrar problemas tanto en proyectos como en tareas para indicar el trabajo imprevisto que debe solucionarse. También puede enviar solicitudes que se registren como problemas en un proyecto designado como cola de solicitud.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> <p>Revise o otorgue una licencia superior para eliminar problemas en la sección Problemas de un proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuración del nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Ver o acceder más a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas en el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concesión de acceso a problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos sobre el problema</p> <p>Contribute o permisos superiores en el proyecto o la tarea</p> <p> Para obtener información sobre la concesión de permisos a problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre la solicitud de permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones para eliminar problemas

* El administrador de Workfront o un administrador de grupo deben habilitar la eliminación de problemas en un proyecto que tenga el estado Completado en el área Preferencias del proyecto. Para obtener información sobre la configuración de las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Si el problema ha registrado horas, el administrador de Workfront o un administrador de grupo debe permitir la eliminación de estos problemas configurando las Preferencias de tarea y problema en la instancia de Workfront. Esto también se aplica cuando intenta eliminar proyectos que tienen problemas con las horas registradas en ellos.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   Para obtener más información sobre cómo habilitar la eliminación de problemas en los que se registran horas, consulte la sección &quot;Eliminación&quot; en [Configurar las preferencias de problemas y tareas de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## El impacto de la eliminación de problemas

Al eliminar un problema, se ven afectados otros objetos vinculados a él.

Los siguientes objetos adjuntos a un problema también se eliminan al eliminar un problema:

* Documentos

   No puede eliminar un problema que tenga un documento que se haya extraído adjunto. Para obtener más información sobre la comprobación de documentos, consulte [Ver documentos](../../../documents/managing-documents/check-out-documents.md).

* Notas
* Rutas de aprobación

Dependiendo de cómo configure el administrador de Workfront o de grupo las preferencias de eliminación de proyectos, tareas o problemas en la sección **Preferencias de horario y hora** de su instancia de Workfront, las horas registradas para los problemas se gestionan de una de las siguientes maneras al eliminar un problema:

* Mover al proyecto y no se restaurará en el problema si el problema se restaura más tarde.
* Se eliminará y se restaurará en el problema si el problema se restaura más tarde.

   Esto también se aplica cuando intenta eliminar proyectos que tienen tareas con horas registradas.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">(this is not possible in classic)</span>
  </MadCap:conditionalText>
  -->

   Para obtener más información sobre la configuración de las preferencias de eliminación para las horas registradas en los problemas, consulte [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Los usuarios asignados al problema o a la aprobación del problema permanecen en el equipo del proyecto.\
   Para obtener más información sobre los equipos de proyecto, consulte [Información general del equipo del proyecto](../../../manage-work/projects/planning-a-project/project-team-overview.md).

## Eliminar problemas

* [Eliminar varios problemas en un proyecto simultáneamente](#delete-multiple-issues-in-a-project-simultaneously)
* [Eliminar un solo problema](#delete-a-single-issue)

### Eliminar varios problemas en un proyecto simultáneamente  {#delete-multiple-issues-in-a-project-simultaneously}

1. Vaya a la **Menú principal**.
1. Haga clic en **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene los problemas que desea eliminar.
1. Haga clic en **Problemas** en el panel izquierdo.
1. Seleccione un problema y haga clic en el botón **Eliminar** icono ![](assets/delete.png) en la parte superior de la lista.

1. Si la eliminación está permitida, haga clic en **Sí, elimínelo**.\
   Es posible que el administrador de Workfront no permita la eliminación de problemas en los que se registran horas.\
   Para obtener más información sobre el acceso y los permisos necesarios para eliminar un problema, consulte [Eliminar problemas](#access-and-permissions-needed).

### Eliminar un solo problema {#delete-a-single-issue}

1. Haga clic en el **Principal** para abrir el Navegador.
1. Haga clic en **Proyectos**.
1. Haga clic en el nombre del proyecto que contiene el problema que desea eliminar.
1. Haga clic en **Problemas** en el panel izquierdo.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. Haga clic en el nombre del problema que desee eliminar.
1. Haga clic en el **Más** para abrir el Navegador.

   ![](assets/qs-issue-more-menu-highlighted-350x469.png)

1. Haga clic en **Eliminar**.
1. Si la eliminación está permitida, haga clic en **Sí, elimínelo**.

   Es posible que el administrador de Workfront no permita la eliminación de problemas en los que se registran horas.\
   Para obtener más información sobre el acceso y los permisos necesarios para eliminar un problema, consulte [Eliminar problemas](#access-and-permissions-needed).

## Restaurar problemas eliminados

Un administrador de Workfront o de grupo puede restaurar los problemas en un plazo de 30 días después de eliminarlos. Para obtener más información sobre la restauración de elementos en Workfront, consulte [Restaurar elementos eliminados](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
