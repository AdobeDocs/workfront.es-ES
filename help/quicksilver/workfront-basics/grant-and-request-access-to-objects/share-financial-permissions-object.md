---
title: Compartir permisos financieros en un objeto
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: El administrador de Adobe Workfront puede otorgarle acceso para ver o editar datos financieros al asignar su nivel de acceso. Para obtener más información, consulte Concesión de acceso a datos financieros.
author: Courtney
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/IVsfFJKauKvgOzXMP8rxHos8LDhqWYnThoyZeaiMCv0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 542
ht-degree: 20%

---

# Compartir permisos financieros en un objeto

El administrador de Adobe Workfront puede otorgarle acceso para ver o editar datos financieros al asignar su nivel de acceso. Para obtener más información, consulte [Concesión de acceso a los datos financieros](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para Ver o Administrar finanzas para proyectos, tareas o problemas específicos que tenga acceso para compartir.

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los datos financieros, vea la sección [Datos financieros](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Requisitos de acceso

<!--
drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial  Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> 
   <p>Plan</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Consulta o acceso superior a Proyectos, Tareas, Problemas y Datos financieros</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> Ver permisos o superiores en proyectos, tareas y problemas que incluyen al menos Ver tarifas de facturación, Ver tarifas de costo y Ver permisos financieros generales</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartir un objeto y conceder permisos financieros

Tenga en cuenta lo siguiente al conceder permisos financieros a objetos:

* Puede conceder permisos financieros a proyectos, tareas y problemas.
* Los permisos se pueden heredar: si tiene permisos de Ver finanzas generales en un proyecto, hereda automáticamente los permisos de Ver finanzas generales en las tareas y problemas del proyecto.
* La concesión de permisos para las tarifas de facturación y de costo permite al usuario ver o editar las tarifas de ese objeto. Los permisos para finanzas generales permiten al usuario ver o editar campos financieros generales (no relacionados con la facturación o las tasas de coste) en el objeto.

Para conceder permisos financieros a un objeto:

1. Vaya a una tarea, proyecto o problema que desee compartir con otros.
1. Cerca del nombre del objeto, haga clic en **Compartir**.

1. En el campo **Dar acceso a `<Object name>` a** comience a escribir el nombre de un usuario, equipo, rol, grupo o compañía con el que desee compartir el objeto.

   >[!TIP]
   >
   >Únicamente puede compartir un objeto con usuarios, equipos, funciones o compañías activas.

1. Haga clic en la lista desplegable a la derecha del nombre del usuario y seleccione una de las siguientes opciones:

   * **Vista**
   * **Aportar**
   * **Administrar**

1. En el mismo menú desplegable, haga clic en el icono de opciones avanzadas situado junto al nivel de permisos y, a continuación, realice una de las siguientes acciones:

   * Para cualquier nivel de permiso, seleccione **Ver tarifas de facturación**, **Ver tarifas de costo** y **Ver finanzas generales** según sea necesario.
   * Solo para **administrar** permisos, seleccione **Editar tarifas de facturación**, **Editar tarifas de costo** y **Editar finanzas generales** según sea necesario.

1. Haga clic en **Guardar**.

## Permiso financiero para todos los niveles de uso compartido

En la tabla siguiente se muestran los permisos financieros que obtienen los usuarios cuando se les conceden los permisos de Ver, Contribuir o Administrar en objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Acciones</strong> </th> 
   <th><strong>Administrar</strong> </th> 
   <th><strong>Aportar</strong> </th> 
   <th><strong>Vista</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Administrar registros de facturación</td> 
   <td>✓</td> 
   <td> <p>  </p> </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Editar tarifas de facturación</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Editar tarifas de coste</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>  
  <tr> 
   <td>Editar finanzas generales</td> 
   <td>✓</td> 
   <td></td> 
   <td>  </td> 
  </tr>
  <tr> 
   <td>Ver tarifas de facturación</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Ver tarifas de coste</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr>  
  <tr> 
   <td>Ver finanzas generales</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>  ✓</td> 
  </tr> 
  <tr> 
   <td>Ver información por coste en las herramientas de planificación de recursos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Recursos presupuestarios en las herramientas de planificación de recursos*</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Ver recursos en las herramientas de planificación de recursos*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Requiere acceso adicional a Administración de recursos.

Para obtener información acerca del acceso a Administración de recursos, vea [Conceder acceso a Administración de recursos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

<!--
These rows removed from last table.

  <tr> 
   <td>Manage/ View Role Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 
  <tr> 
   <td>Manage/ View User Billing and Cost Rates</td> 
   <td>✓</td> 
   <td>  </td> 
   <td>  </td> 
  </tr> 

-->
