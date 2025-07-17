---
title: Conceder acceso a filtros, vistas y agrupaciones
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los controles de filtro, vista y agrupación para listas e informes.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 100%

---

# Conceder acceso a filtros, vistas y agrupaciones

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los controles de filtro, vista y agrupación para listas e informes, como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Para obtener información sobre los controles de filtro, vista y agrupación, consulte [Elementos de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurar el acceso de los usuarios a filtros, vistas y agrupaciones mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) del botón **Ver** o **Editar** situado a la derecha de los filtros y, a continuación, seleccione las capacidades que desea conceder en **Ajuste la configuración**.

   ![](assets/gear-icon-filters-dashboards-groupings.png)

   De forma predeterminada, los usuarios con una licencia de planificación, trabajo, revisor o solicitud tienen capacidades plenas de visualización y edición. Los usuarios con una licencia de usuario externo no tienen acceso a filtros, vistas y agrupaciones.

   <!--If this changes, undraft section with table below
   -->

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

<!--## Access to filters, views, and groupings by license type

Drafting out this section for now because the table is redundant since all four license types can do everything.</span>-->

En esta tabla se enumera lo que un administrador de Workfront puede permitir que hagan los usuarios según cada tipo de licencia con los filtros, las vistas y las agrupaciones. Para obtener información sobre los tipos de licencia de Workfront, consulte [Información general sobre licencias de Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> Acción </th>
<th> Planificador </th>
<th> Trabajador </th>
<th> Revisor </th>
<th> Solicitante </th>
</tr>
</thead>
<tbody>
<tr>
<td>Edición de filtros, vistas y agrupaciones</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Creación de filtros, vistas y agrupaciones</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Visualización de filtros, vistas y agrupaciones</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Eliminación de filtros, vistas y agrupaciones</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Compartir filtros, vistas y agrupaciones</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Compartir filtros, vistas y agrupaciones en todo el sistema</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>
