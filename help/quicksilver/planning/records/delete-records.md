---
title: Eliminar registros
description: Puede eliminar los registros que usted u otro usuario hayan creado.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 42%

---


# Eliminar registros

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Puede eliminar los registros que ya no sean relevantes en Adobe Workfront Planning. Puede recuperar los registros eliminados durante 30 días después de haberlos eliminado. Para obtener información acerca de cómo recuperar los registros eliminados, vea [Recuperar registros eliminados](/help/quicksilver/planning/records/restore-deleted-records.md).

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
   <td>   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Consideraciones sobre la eliminación de registros

* Puede eliminar los registros que usted u otro usuario hayan creado.
* Puede recuperar los registros eliminados que usted u otros usuarios hayan eliminado.
* Si los registros eliminados están vinculados a otros registros, los registros vinculados no se eliminan, pero también se elimina la información del registro eliminado.
* No se pueden eliminar registros de la escala de tiempo o de las vistas de calendario.

## Eliminar registros

Puede eliminar un registro de las siguientes áreas:

* [Desde la página del registro](#delete-a-record-from-the-records-page)
* [Desde la vista de tabla de un tipo de registro](#delete-a-record-from-the-record-type-table-view)

### Eliminar un registro de la página del registro

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos registros desee eliminar.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. Realice una de las siguientes acciones:

   * En la vista Tabla, haga clic en el nombre de un registro.
   * En la vista Tabla, pase el ratón sobre el nombre de un registro, haga clic en el menú **Más** ![Menú Más](assets/more-menu.png) y, a continuación, haga clic en **Ver**

     ![Menú contextual para la fila de registros](assets/contextual-menu-for-record-row.png)
   * En una vista Línea de tiempo, haga clic en una barra de registro.

   Se abre la página de registro.

1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del registro, luego haga clic en **Eliminar** y después en **Eliminar** de nuevo para confirmar.

   ![Más opciones de menú de la página de detalles del registro](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Se elimina el registro.
1. (Opcional) Vaya a la vista de tabla de la página del registro y haga clic en el icono **Deshacer** ![Deshacer icono](assets/undo-icon.png) en la esquina superior derecha de la vista; a continuación, haga clic en **Eliminados recientemente** para recuperar los registros eliminados.

Para obtener información acerca de cómo recuperar los registros eliminados, vea [Recuperar registros eliminados](/help/quicksilver/planning/records/restore-deleted-records.md).

### Eliminar un registro de la vista de tabla de tipo de registro

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos registros desee eliminar.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) En el menú desplegable **Vista** de la esquina superior izquierda de la tabla, seleccione una Vista de tabla. Esta debe ser la vista predeterminada, a menos que haya visto el tipo de registro en la vista de cronología cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Realice una de las siguientes acciones:

   * Haga clic con el botón derecho en una fila de registro y, a continuación, haga clic en **Eliminar**.
   * Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del registro y, a continuación, haga clic en **Eliminar**.

     ![Menú contextual para la fila de registros](assets/contextual-menu-for-record-row.png)

   * Haga clic en el icono **Abrir detalles** ![Abrir detalles en el campo de nombre de tabla](assets/open-details-icon-in-table-name-field.png) para abrir el cuadro con la información detallada del registro, haga clic en **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre del registro y, a continuación, en **Eliminar**.

   Se elimina el registro.

1. (Opcional) Realice una de las siguientes acciones para deshacer o rehacer la eliminación de un registro:

   * Haga clic en el icono **Deshacer** ![Deshacer icono](assets/undo-icon.png) y, a continuación, **Eliminado(a) recientemente** para recuperar los registros eliminados. Para obtener información acerca de cómo recuperar los registros eliminados, vea [Recuperar registros eliminados](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Utilice los siguientes métodos abreviados del teclado para deshacer o rehacer la eliminación de un registro:

      * CTRL + Z (⌘ + Z para Mac) para deshacer la eliminación de un registro
      * CTRL + Mayús + Z (⌘ + Mayús + Z para Mac) para rehacer la eliminación del registro




