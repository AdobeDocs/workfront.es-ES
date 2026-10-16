---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Editar información de la plantilla de horas
description: Como usuario con acceso administrativo a las plantillas de horas, puede editar información sobre las existentes en Adobe Workfront. Por ejemplo, puede editar el Propietario, los Aprobadores o el lapso de tiempo de la plantilla de horas.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
TQID: https://experienceleague.adobe.com/--QshuygnTfcEJtt6-Tx-2QtNT-5p9TrTWaQTMBZNAg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 69%
---
# Editar información de la plantilla de horas

Como usuario con acceso administrativo a las plantillas de horas, puede editar información sobre las existentes en Adobe Workfront. Por ejemplo, puede editar el Propietario, los Aprobadores o el lapso de tiempo de la plantilla de horas.

Puede editar la información en una sola plantilla de horas o puede editar varias plantillas de horas de forma masiva.

>[!IMPORTANT]
>
>Si los usuarios están asociados con perfiles de plantillas de horas y estas se generan automáticamente, los cambios que realice en las plantillas de horas existentes no se reflejarán en las plantillas de horas que se generarán en fechas futuras. Todas las plantillas de horas generadas automáticamente tienen la configuración establecida en Perfiles de plantillas de horas. Para obtener más información, consulte [Crear perfiles de plantillas de horas](../create-and-manage-timesheets/create-timesheet-profiles.md)

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
   <td><p>Acceso administrativo a hojas de horas</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar plantillas de horas

{{step1-to-timesheets}}

De forma predeterminada, se muestran todas las hojas de horas a las que tiene acceso para ver.

![Lista de hojas de horas](assets/list-of-all-timesheets.png)

1. (Opcional) Haga clic en el icono **buscar** ![Icono de búsqueda](assets/search-icon.png) y escriba una palabra clave para buscar una hoja de horas específica. Por ejemplo, puede buscar un lapso de tiempo o un nombre de propietario para una plantilla de horas.

1. (Opcional) Realice una de las siguientes acciones para actualizar el filtro en la lista de plantillas de horas:

   * Seleccione **Mis aprobaciones de hojas de horas** en la esquina superior derecha de la página para ver solamente las hojas de horas que usted apruebe,

     O

     Seleccione **Mis plantillas de horas** para ver solamente sus plantillas de horas.

     Esto aplica los filtros **Mis aprobaciones de hojas de horas** o **Mi hoja de horas** a la lista de hojas de horas.

   * Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-nwepng.png) para aplicar un filtro o crear uno nuevo. Para obtener información sobre cómo crear o actualizar filtros, consulte [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Las opciones Mis aprobaciones de hojas de horas y Mis hojas de horas no se muestran en la parte superior de la lista de hojas de horas ni en la lista de filtros si el administrador de Workfront o de un grupo ha eliminado esos filtros de los controles de lista en el área de Configuración o de la plantilla de diseño. Para obtener más información, consulte [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Opcional) Haga clic en los iconos **Ver** ![Ver icono](assets/view-icon.png) o **Agrupar** ![Icono de agrupación](assets/grouping.png) para aplicar una vista o agrupación o para crear una nueva.

   Para obtener información sobre la creación de filtros, vistas o agrupaciones, consulte los siguientes artículos:

   * [Crear o editar filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Crear o editar vistas en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Creación de agrupaciones en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Seleccione una o varias hojas de horas y luego haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) en la parte superior de la lista de hojas de horas.
1. Consulte o introduzca la siguiente información:

   | Nombre de campo | Descripción |
   | --------- | ---------- |
   | Propietario | <p>Nombre del usuario para el que se creó la plantilla de horas. No puede editar este campo.</p><p>Este campo no se muestra al seleccionar varias plantillas de horas.</p> |
   | Fecha de inicio | Esta la fecha de inicio de la plantilla de horas. |
   | Fecha de finalización | Esta es la fecha de finalización de la plantilla de horas. |
   | Estado | <p>Este es el estado de la plantilla de horas. Las siguientes son posibles opciones de estado de la plantilla de horas:</p><ul><li>**Abrir**: la plantilla de horas está abierta y las entradas de horas se pueden editar.</li><li>**Enviada**: la plantilla de horas se envía para su aprobación a los aprobadores designados.</li><li>**Rechazada**: la plantilla de horas no fue aprobada por los aprobadores y ahora está disponible nuevamente para que el usuario edite las entradas de tiempo.</li><li>**Cerrada**: la plantilla de horas está cerrada por el usuario o aprobada por el aprobador y, como resultado, ahora está cerrada. No se puede añadir tiempo a una plantilla de horas cerrada.</li></ul> |
   | Aprobadores | <p>Los aprobadores aprueban la plantilla de horas de los usuarios asociados con ella. Solo los usuarios con derechos administrativos de plantilla de horas pueden establecerse como aprobadores. Para obtener más información sobre los derechos administrativos sobre las plantillas de horas, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Comience a introducir los nombres de los aprobadores de plantillas de horas y selecciónelos cuando aparezcan en la lista.</p> <p>Puede tener varios aprobadores en una plantilla de horas. En este caso, una vez que uno de los aprobadores apruebe la plantilla de horas, esta se marcará como **Cerrada** y desaparecerá de la lista de aprobaciones de plantillas de horas de todos los aprobadores restantes.</p> |
   | Puede editar el tiempo | <p>Seleccione esta opción si desea permitir que los aprobadores editen las horas en la plantilla de horas.</p><p>Esta opción no está disponible si selecciona varias plantillas de horas.</p> |
   | Horas extra | <p>Puede elegir ocultar el cuadro Horas extra en la plantilla de horas.</p><p>Esta opción está desactivada de forma predeterminada.</p> |

1. Haga clic en **Guardar**.
