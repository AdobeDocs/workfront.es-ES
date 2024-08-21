---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creación y administración de perfiles de hojas de horas de un grupo
description: Cuando visualiza un grupo que administra en el área de Grupos, puede ver y trabajar con los perfiles de plantilla de horas para los que los administradores del grupo o uno de sus subgrupos tienen acceso administrativo.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Crear y administrar perfiles de hojas de horas de un grupo

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

Cuando visualiza un grupo que administra en el área de Grupos, puede ver y trabajar con los perfiles de plantilla de horas para los que los administradores del grupo o uno de sus subgrupos tienen acceso administrativo.

Si hay grupos por encima del grupo que administra, sus administradores también pueden hacerlo en su grupo. Lo mismo ocurre con los administradores de Workfront (para cualquier grupo).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de grupo del grupo.</p>  <p>También debe tener acceso administrativo a las hojas de horas. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder a los usuarios acceso administrativo a ciertas áreas</a>.</p>  <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Crear y editar perfiles de hojas de horas de nivel de grupo

Puede crear y editar perfiles de hojas de horas para utilizarlos en un grupo que administre. Para obtener instrucciones, consulte [Crear, editar y asignar perfiles de hojas de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Eliminar perfiles de hojas de horas de nivel de grupo

Puede eliminar los perfiles de hoja de horas que utilice un grupo que administre. Para obtener instrucciones, consulte [Eliminar perfiles de hojas de horas](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Generar manualmente hojas de horas de grupo

Para permitir que los cambios realizados en los perfiles de plantillas de horas se reflejen en las plantillas de horas agrupadas actuales, primero debe eliminar las plantillas de horas existentes y luego generar manualmente las nuevas. Para obtener instrucciones, consulte [Generar hojas de horas manualmente a partir del área Hojas de horas y horas](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) en [Generar hojas de horas manualmente](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Para obtener información sobre cómo eliminar hojas de horas de grupo, consulte [Eliminar hojas de horas en Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Exportar perfiles de hojas de horas de nivel de grupo

{{step-1-to-setup}}

1. Haga clic en **Grupos**.

   En la lista que se muestra, puede ver los grupos que administra, junto con los subgrupos que tengan. Los administradores de Adobe Workfront pueden ver todos los grupos.

1. Haga clic en el nombre del grupo con los perfiles de plantilla de horas que desee exportar.
1. Haga clic en **Perfiles de hojas de horas**.
1. Haga clic en **Exportar** para exportar la lista de perfiles de hojas de horas del grupo.
