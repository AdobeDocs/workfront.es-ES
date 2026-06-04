---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Generar plantillas de horas manualmente
description: Para permitir que los cambios realizados en los perfiles de plantilla de horas se reflejen en las plantillas de horas actuales, primero debe eliminar las plantillas de horas existentes y luego generar manualmente las nuevas. Puede generar manualmente plantillas de horas desde el área Plantillas de horas o el área Diagnóstico en Configuración, tal como se explica en este artículo.
author: Lisa
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
TQID: https://experienceleague.adobe.com/0hU3VlHM8l5TXee6K3lJaV9-W3ZKujDYf9-f1NXH-Nc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 18%

---

# Generar plantillas de horas manualmente

Para permitir que los cambios realizados en los perfiles de plantilla de horas se reflejen en las plantillas de horas actuales, primero debe eliminar las plantillas de horas existentes y luego generar manualmente las nuevas. Puede generar manualmente plantillas de horas desde el área Plantillas de horas o el área Diagnóstico en Configuración, tal como se explica en este artículo.

Para obtener instrucciones sobre cómo eliminar hojas de horas, consulte [Eliminar hojas de horas en Adobe Workfront](../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td><p>Debe ser administrador de Workfront o, si está trabajando en perfiles de plantilla de horas para un grupo, debe ser administrador de grupo (o administrador de Workfront).</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
1. Haga clic en el icono de más ![icono de más](assets/more-icon.png) y luego en **Generar hojas de horas**.

1. En la parte superior de la lista de perfiles de hojas de horas, haga clic en el icono **Más** ![Icono de más](assets/more-icon.png) para perfiles de hojas de horas de nivel de sistema o en **Más** para perfiles de hojas de horas de grupo y, a continuación, haga clic en **Generar hojas de horas**.

   Las nuevas hojas de horas se crean para un máximo de dos períodos de tiempo para los usuarios asociados con perfiles de hojas de horas.

## Genere manualmente hojas de horas de nivel de sistema desde el área de Diagnóstico

Puede generar manualmente plantillas de horas de nivel de sistema desde el área Diagnóstico en Configuración.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Expanda **Sistema** y, a continuación, haga clic en **Diagnósticos**.

1. Haga clic en **Diagnóstico de conducta**.
1. Haga clic en **Generar hojas de horas**.
