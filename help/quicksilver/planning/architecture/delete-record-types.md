---
title: Eliminar tipos de registro
description: Puede eliminar los tipos de registro cuando ya no sean relevantes. Al eliminar los tipos de registro también se elimina toda la información asociada a los tipos de registro, como sus registros, campos y vistas.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 75%

---


# Eliminar tipos de registro

{{planning-important-intro}}

Puede eliminar los tipos de registro cuando ya no sean relevantes.

Sin embargo, al eliminar los tipos de registro, también se elimina toda la información asociada a los tipos de registro. Para obtener más información, consulte la sección [Consideraciones al eliminar tipos de registros](#considerations-when-deleting-record-types) en este artículo.

Para obtener más información sobre los tipos de registros, consulte [Información general sobre los tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar</p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## Consideraciones al eliminar tipos de registros

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Únicamente se pueden eliminar los tipos de registro de espacios de trabajo para los que tenga permisos de administración.
* Al eliminar los tipos de registro, se elimina la información siguiente asociada a ellos:

   * Todos los registros de ese tipo.
   * Todos los campos asociados al tipo de registro.
   * Todas las vistas (incluidos filtros, agrupaciones y criterios de ordenación) del tipo de registro.
* El tipo de registro se elimina de todos los usuarios que acceden al espacio de trabajo.
* No se pueden recuperar los tipos de registros eliminados ni su información.
* Se recomienda volver a crear los campos y los registros asociados al tipo de registro que desea eliminar en otro tipo de registro antes de eliminarlos.

## Eliminar tipos de registro

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos tipos de registros desea eliminar,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo situada a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y, a continuación, selecciónelo cuando se muestre en la lista.

   Se abre el espacio de trabajo y se muestran los tipos de registro.
1. Realice una de las siguientes acciones:

   * Pase el puntero por encima de la tarjeta del tipo de registro, haga clic en el menú **Más** y luego en **Eliminar**.
   * Haga clic en la tarjeta del tipo de registro que desee eliminar y, en la página de tipo de registro, haga clic en el menú **Más** ![Más menú](assets/more-menu.png) a la derecha del nombre del tipo de registro y, a continuación, haga clic en **Eliminar**.

   ![Eliminar permanentemente la confirmación del tipo de registro](assets/permanently-delete-record-type-confirmation.png)

1. Escriba **Eliminar** en el cuadro de confirmación y haga clic en **Eliminar permanentemente**. Esto no distingue entre mayúsculas y minúsculas.

   El tipo de registro seleccionado, junto con sus campos, registros asociados y vistas, se eliminará y no se podrá recuperar.
