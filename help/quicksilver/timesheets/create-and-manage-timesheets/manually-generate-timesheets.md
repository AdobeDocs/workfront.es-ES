---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Generar manualmente hojas de horas
description: Para permitir que los cambios realizados en los perfiles de plantilla de horas se reflejen en las plantillas de horas actuales, primero debe eliminar las plantillas de horas existentes y luego generar manualmente las nuevas. Puede generar manualmente plantillas de horas desde el área Plantillas de horas o el área Diagnóstico en Configuración, tal como se explica en este artículo.
author: Alina
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
source-git-commit: a4bb3582eb476acbefa5d11db1f2c06eafc13cdd
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 27%

---

# Generar manualmente hojas de horas

Para permitir que los cambios realizados en los perfiles de plantilla de horas se reflejen en las plantillas de horas actuales, primero debe eliminar las plantillas de horas existentes y luego generar manualmente las nuevas. Puede generar manualmente plantillas de horas desde el área Plantillas de horas o el área Diagnóstico en Configuración, tal como se explica en este artículo.

Para obtener instrucciones sobre cómo eliminar hojas de horas, consulte [Eliminar hojas de horas en Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Requisitos de acceso

Para realizar los pasos de este artículo, debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront o, si está trabajando en perfiles de plantilla de horas para un grupo, debe ser administrador de grupo (o administrador de Workfront). Para obtener más información, consulte <a href="../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores de grupos</a>.</p> <p>Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Creación o modificación de niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Consideraciones sobre las plantillas de horas generadas manualmente

Cuando se generan manualmente hojas de horas:

* Se generan según los perfiles de hoja de horas asociados a los usuarios. Los usuarios que no tengan perfiles de hojas de horas asociados a ellos no reciben hojas de horas. 
* Solo se genera la plantilla de horas actual y la que se va a seguir. Workfront no genera dos plantillas de horas para el mismo período. Si ya tiene una plantilla de horas para el periodo de tiempo actual, otra no se generará cuando utilice el proceso manual para generar plantillas de horas.

## Generar manualmente hojas de horas desde el área Hojas de horas y horas

Puede generar manualmente plantillas de horas a nivel del sistema o de grupo desde el área Plantillas de horas y Horas en Configuración.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Si está generando hojas de horas en uso en todo el sistema, haga clic en **Hojas de horas y horas.**

   O

   Si está generando hojas de horas usadas por un grupo específico, haga clic en **Grupos** y luego haga clic en el nombre del grupo.

1. Haga clic en **Perfiles de plantilla de horas**.
1. Haga clic en el icono **Más** ![Icono de más](assets/more-icon.png) y luego en **Generar hojas de horas**.

   Las nuevas hojas de horas se crean para un máximo de dos períodos de tiempo para los usuarios asociados con perfiles de hojas de horas.

## Genere manualmente hojas de horas de nivel de sistema desde el área de Diagnóstico

Puede generar manualmente plantillas de horas de nivel de sistema desde el área Diagnóstico en Configuración.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Expanda **Sistema** y, a continuación, haga clic en **Diagnósticos**.

1. Haga clic en **Diagnóstico de conducta**. 
1. Haga clic en **Generar hojas de horas**.
