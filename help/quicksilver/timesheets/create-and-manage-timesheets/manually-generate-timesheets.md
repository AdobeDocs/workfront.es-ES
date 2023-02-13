---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Generar hojas de hora manualmente
description: Para habilitar los cambios realizados en los perfiles de hojas de horas para que se reflejen en las hojas de horas actuales, primero debe eliminar las hojas de horas existentes y luego generar manualmente las nuevas. Puede generar hojas de horas manualmente desde el área Hojas de horas o el área Diagnóstico de Configuración, tal como se explica en este artículo.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 0%

---

# Generar hojas de hora manualmente

Para habilitar los cambios realizados en los perfiles de hojas de horas para que se reflejen en las hojas de horas actuales, primero debe eliminar las hojas de horas existentes y luego generar manualmente las nuevas. Puede generar hojas de horas manualmente desde el área Hojas de horas o el área Diagnóstico de Configuración, tal como se explica en este artículo.

Para obtener instrucciones sobre la eliminación de partes de horas, consulte [Eliminar partes de horas en Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront o, si está trabajando en perfiles de parte de horas para un grupo, debe ser administrador de grupo (o administrador de Workfront). Para obtener más información, consulte <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupo</a>.</p> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre las hojas de horas generadas manualmente

Cuando genera hojas de horas manualmente:

* Se generan según los perfiles de hojas de horas asociados a los usuarios. Los usuarios que no tienen perfiles de parte de horas asociados a ellos no reciben partes de horas. 
* Solo se generan el parte de horas actual y el que se va a seguir. Workfront no genera dos partes de horas para el mismo período. Si ya tiene un parte de horas para un lapso de tiempo específico, otro no se generará cuando esté utilizando el proceso manual para generar partes de horas.

## Generar hojas de horas manualmente desde el área Hojas de horas y horas

Puede generar manualmente hojas de hora a nivel de sistema o de grupo desde el área Hojas de hora y horas de Configuración.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Si está generando partes de horas en uso en todo el sistema, haga clic en **Hojas de hora y horas.**

   O

   Si está generando partes de horas utilizadas por un grupo específico, haga clic en **Grupos** y, a continuación, haga clic en el nombre del grupo.

1. Haga clic en **Perfiles de parte de horas**.
1. Haga clic en **Más**, luego **Generar hojas de hora**.

   Se crean nuevas hojas de horas para un máximo de dos períodos de tiempo para los usuarios asociados con perfiles de hojas de horas.

## Generar manualmente hojas de horas a nivel de sistema desde el área Diagnóstico

Puede generar manualmente hojas de horas a nivel de sistema desde el área Diagnóstico de Configuración.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema** y haga clic en **Diagnóstico**.

1. Haga clic en **Diagnóstico de conducta**. 
1. Haga clic en **Generar hojas de hora**.
