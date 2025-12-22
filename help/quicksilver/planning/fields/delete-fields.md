---
title: Eliminar campos
description: En Adobe Workfront Planning, puede eliminar campos personalizados que ya no sean relevantes.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 36%

---



# Eliminación de campos

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

En Adobe Workfront Planning, puede crear campos personalizados para almacenar información sobre registros.

Para obtener información acerca de cómo crear campos personalizados en Workfront Planning, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

Puede eliminar los campos de Workfront Planning que ya no sean relevantes.

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
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Cualquier Workfront y cualquier paquete de Planning</p></li>
O
<li><p>Cualquier flujo de trabajo y cualquier paquete de Planning</p></li></ul>

<p><span class="preview">Para eliminar campos de los tipos de registros globales:</span></p>
<ul><li><p><span class="preview">Cualquier paquete Workfront y un paquete Planning Plus</span></p></li>
O
<li><p><span class="preview">Cualquier paquete de flujo de trabajo y planificación de Prime y Ultimate</span></p></li></ul>

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

## Consideraciones sobre la eliminación de campos de Workfront Planning:

* Solo puede eliminar un campo en la vista de tabla de tipo de registro.
* No se puede eliminar el campo principal de un registro.
* La información almacenada en el campo se elimina y no se puede recuperar.
* Al eliminar un campo de registro conectado, todos los campos de búsqueda conectados también se eliminan del tipo de registro desde el que se conecta. Los campos de registro conectados de los tipos de registro a los que se conecta también se eliminan del registro al que se conecta.

  Por ejemplo, cuando conecta Campaigns a otro tipo de registro llamado Product y elimina el campo Product connected y el campo de búsqueda Product&#39;s Status de la campaña, se eliminan los siguientes elementos:

   * El campo Product connected de la campaña
   * El campo de búsqueda Estado del producto de la campaña
   * El campo conectado a Campaign desde el producto

  Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* <span class="preview">No se pueden eliminar campos de registros globales que se hayan agregado a espacios de trabajo secundarios desde los espacios de trabajo secundarios.</span>

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

   Los campos eliminados no se pueden recuperar.

   Dependiendo del tipo de campo que elimine, ocurre lo siguiente:

   * Si elimina un campo que pertenece al registro seleccionado, el campo se elimina y ya no se puede asociar con ningún registro. Si este campo se agrega como un campo de búsqueda en otros registros, esos campos también se eliminan.
   * Si elimina un campo de conexión, el campo se elimina del registro seleccionado. Además, también se elimina el campo de conexión correspondiente de su registro original.
   * Si elimina un campo de búsqueda que se agregó desde un registro conectado, el campo se eliminará del tipo de registro seleccionado, pero permanecerá en su tipo de registro original.
   * <span class="preview">Si elimina un campo de un tipo de registro global en su área de trabajo principal, se eliminará de todos los espacios de trabajo donde se haya agregado ese tipo de registro. No se pueden eliminar campos de los tipos de registros globales de sus espacios de trabajo secundarios.</span>
