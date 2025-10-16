---
title: Eliminar campos
description: En Adobe Workfront Planning, puede eliminar campos personalizados que ya no sean relevantes.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 57%

---



# Eliminación de campos

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

En Adobe Workfront Planning, puede crear campos personalizados para almacenar información sobre registros.

Para obtener información acerca de cómo crear campos personalizados en Workfront Planning, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

Puede eliminar los campos de Workfront Planning que ya no sean relevantes.

## Consideraciones sobre la eliminación de campos de Workfront Planning:

* Solo puede eliminar un campo en la vista de tabla de tipo de registro.
* No se puede eliminar el campo principal de un registro.
* La información almacenada en el campo se elimina y no se puede recuperar.
* Al eliminar un campo de registro conectado, todos los campos de búsqueda conectados también se eliminan del tipo de registro desde el que se conecta. Los campos de registro conectados de los tipos de registro a los que se conecta también se eliminan del registro al que se conecta.

  Por ejemplo, cuando conecta campañas a otro tipo de registro llamado producto y elimina el campo Producto conectado y el campo de búsqueda Estado del producto de la campaña, se eliminan los siguientes elementos:

   * El campo Product connected de la campaña
   * El campo de búsqueda Estado del producto de la campaña
   * El campo conectado a Campaign desde el producto.

  Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Cualquier Workfront y cualquier paquete de Planning</p></li>
<p>O</p>
<li><p>Cualquier flujo de trabajo y cualquier paquete de Planning</p></li></ul>

<!--
<p><span class="preview">To delete global record types:</span</p>
<ul><li><p><span class="preview">Any Workfront package and a Planning Plus package</span></p></li>
<p>Or</p>
<li><p><span class="preview">Workflow and Planning Prime and Ultimate packages</span></p></li></ul>
-->

<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Eliminación de campos

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos campos de registro desee eliminar.

   Se abre el espacio de trabajo y se muestran los tipos de registro.

1. Haga clic en la tarjeta de un tipo de registro.

1. (Condicional) Si aún no está seleccionado, haga clic en la pestaña de una **Vista de tabla** en la página de tipo de registro.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.

1. Busque el campo que desea eliminar en los encabezados de columna, pase el puntero por encima del encabezado de columna y, a continuación, haga clic en la flecha hacia abajo situada después del nombre del campo.

   ![Menú de flecha después del nombre del campo en el encabezado de tabla resaltado](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Haga clic en **Eliminar**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. Haga clic en **Eliminar** para confirmar.

   El campo se elimina, no se puede recuperar y ya no se puede asociar a ningún registro.
