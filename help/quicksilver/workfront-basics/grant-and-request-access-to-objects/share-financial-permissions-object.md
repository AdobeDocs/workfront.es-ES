---
title: Compartir permisos financieros en un objeto
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: El administrador de Adobe Workfront puede otorgarle acceso para ver o editar datos financieros al asignar su nivel de acceso. Para obtener más información, consulte Concesión de acceso a datos financieros.
author: Alina
feature: Get Started with Workfront
exl-id: 0d0e13d9-b234-48d3-a818-5b6fb36a4688
source-git-commit: b4e90918c5f499638d0cf5355dc75c3ceca48293
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 24%

---

# Compartir permisos financieros en un objeto

{{highlighted-preview}}

El administrador de Adobe Workfront puede otorgarle acceso para ver o editar datos financieros al asignar su nivel de acceso. Para obtener más información, consulte [Concesión de acceso a los datos financieros](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede concederles permisos para Ver o Administrar finanzas para proyectos, tareas o problemas específicos que tenga acceso para compartir.

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los datos financieros, vea la sección [Datos financieros](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Requisitos de acceso

<!--drafted for P&P:

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
   <td> <p>View or higher access to Projects, Tasks, Issues, and Financial&nbsp;Data</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to projects, tasks, and issues that include at least View Finance permissions</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Debe tener lo siguiente para compartir información de datos financieros sobre objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Consulta o acceso superior a Proyectos, Tareas, Problemas y Datos financieros</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos o superiores de proyectos, tareas y problemas que incluyen al menos Ver permisos de finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Compartir un objeto y conceder permisos financieros

Tenga en cuenta lo siguiente al conceder permisos financieros a objetos:

* Puede conceder permisos financieros a proyectos, tareas, problemas, <span class="preview">y tarjetas de tarifas</span>.
* Los permisos se pueden heredar: si tiene permisos de Ver finanzas en un proyecto, hereda automáticamente los permisos de Ver finanzas en las tareas y problemas del proyecto.

Para conceder permisos financieros a un objeto:

1. Vaya a una tarea, proyecto o problema que desee compartir con otros.
1. Cerca del nombre del objeto, haga clic en el menú Más ![](assets/more-icon.png) y, a continuación, haga clic en **Compartir**.

1. En el campo **Dar acceso a `<Object name>` a** comience a escribir el nombre de un usuario, equipo, rol, grupo o compañía con el que desee compartir el objeto.

   >[!TIP]
   >
   >Únicamente puede compartir un objeto con usuarios, equipos, funciones o compañías activas.

1. Si aparece un menú desplegable a la derecha del nombre seleccionado, haga clic en una de las siguientes opciones disponibles:

   * **Ver**
   * **Contribute a la misma**
   * **Administrar**

     ![](assets/12.png)      ![](assets/13.png) ![](assets/14.png)

   <span class="preview"> en vista previa:
   ![](assets/project-permissions.png)
   </span>

1. En el mismo menú desplegable, haga clic en **Configuración avanzada** y, a continuación, siga uno de estos procedimientos:

   * Si seleccionó una de las tres opciones en el paso anterior, asegúrese de que **Ver finanzas** está seleccionada.
   * Si seleccionaste **Administrar finanzas** en el paso anterior, asegúrate de que **Administrar finanzas** esté seleccionado.

1. Haga clic en **Guardar**.

## Permiso financiero para todos los niveles de uso compartido

En la tabla siguiente se muestran los permisos financieros que obtienen los usuarios al concederles permisos de Vista, Contribute o Administrar en objetos: 

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
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Administrar/ Ver tarifas de facturación y de costo de rol</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Administrar/ Ver tarifas de facturación y de costo de usuario</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ver finanzas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> ✓</td> 
  </tr> 
  <tr> 
   <td><span class="preview">Administrar tarjetas de tarifas</span></td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span class="preview">Ver tarjetas de tarifa</span></td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> ✓</td> 
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
   <td> </td> 
   <td> </td> 
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
