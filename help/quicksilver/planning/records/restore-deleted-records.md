---
title: Restaurar registros eliminados
description: Puede recuperar los registros eliminados del área Eliminados recientemente en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 5%

---

# Restauración de registros eliminados

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->

{{planning-important-intro}}

Puede recuperar los registros eliminados del área Eliminados recientemente en Adobe Workfront Planning.

Para obtener información acerca de cómo eliminar registros, vea [Eliminar registros](/help/quicksilver/planning/records/delete-records.md).

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
<p>Cualquier Workfront y cualquier paquete de Planning</p> <p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de contribución o superiores para un espacio de trabajo y tipo de registro  </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
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
   <td><p> Standard</p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Consideraciones acerca de la recuperación de registros eliminados

* Puede restaurar los registros que usted u otros usuarios hayan eliminado.
* Los registros se almacenan en el grupo Eliminados recientemente durante 30 días. Después de 30 días, los registros se eliminan permanentemente de Workfront Planning.
* Si los registros eliminados están vinculados a otros registros, los registros vinculados no se eliminan, pero también se elimina la información del registro eliminado. La restauración de los registros eliminados restaurará la información de los registros conectados.
* Puede restaurar registros de forma masiva.
* Cuando se eliminan los registros, se almacena la siguiente información en el grupo Eliminados recientemente:
   * **Nombre**: Esta es la información del campo Principal del registro. Para obtener más información acerca de los campos primarios de registro, vea [Información general sobre el campo primario](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Fecha de eliminación**: La hora y la fecha en que se eliminó el registro.
   * **Tiempo en eliminaciones recientes**: El tiempo desde que se eliminó el registro. Los registros que se eliminaron más de 30 días antes de la fecha actual no se muestran en la bandeja Eliminados recientemente.
   * **Eliminado por**: Nombre del usuario que eliminó el registro.

## Restauración de registros eliminados

1. Vaya a la página de tipo de registro donde ha eliminado registros.
1. Haga clic en el icono **Deshacer** ![Deshacer icono](assets/undo-icon.png) en la esquina superior derecha de cualquier vista de página de tipo de registro y, a continuación, haga clic en **Eliminados recientemente**.

   Se muestra el cuadro **Eliminados recientemente**.

   ![Caja eliminada recientemente](assets/recently-deleted-box.png)

1. Seleccione los registros que desee eliminar y, a continuación, haga clic en **Restaurar** > **Restaurar**. Puede seleccionar más de un registro.

   Si la restauración se realizó correctamente, recibirá una notificación de éxito en la parte inferior de la pantalla.
1. Vaya a la vista de tabla y revise los registros restaurados.
