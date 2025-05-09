---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creación y administración de perfiles de hojas de horas de un grupo
description: Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con los perfiles de plantillas de horas para los que los administradores del grupo o uno de sus subgrupos tienen acceso administrativo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 92%

---

# Crear y administrar los perfiles de plantillas de horas de un grupo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Cuando visualiza un grupo que administra en el área Grupos, puede ver y trabajar con los perfiles de plantillas de horas para los que los administradores del grupo o uno de sus subgrupos tienen acceso administrativo.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td>
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>Debe ser administrador de grupo del grupo o administrador del sistema.</p>
   <p>También debe tener acceso administrativo a las hojas de horas.</p></td>
  </tr>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear y editar perfiles de plantillas de horas de nivel de grupo

Puede crear y editar perfiles de hojas de horas para utilizarlos en un grupo que administre. Para obtener instrucciones, consulte [Crear, editar y asignar perfiles de plantillas de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Eliminar perfiles de plantillas de horas a nivel de grupo

Puede eliminar los perfiles de plantilla de horas que utilice un grupo que administre. Para obtener instrucciones, consulte [Eliminar perfiles de plantillas de horas](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Generar manualmente plantillas de horas de grupo

Para que los cambios realizados en los perfiles de plantillas de horas se puedan reflejar en las plantillas de horas agrupadas actuales, primero debe eliminar las plantillas de horas existentes y luego generar manualmente las nuevas. Para obtener instrucciones, consulte [Generar plantillas de horas manualmente a partir del área Plantillas de horas y horas](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) en [Generar plantillas de horas manualmente](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Para obtener información sobre la eliminación de plantillas de horas de grupo, consulte [Eliminar plantillas de horas en Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Exportar perfiles de plantillas de horas a nivel de grupo

{{step-1-to-setup}}

1. Haga clic en **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo con los perfiles de la plantilla de horas que desee exportar.
1. Haga clic en **Perfiles de plantilla de horas**.
1. Haga clic en **Exportar** para exportar la lista de perfiles de plantilla de horas del grupo.
