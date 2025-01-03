---
title: Eliminar registros
description: Puede eliminar los registros que usted u otro usuario hayan creado.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 9b528e751d23b04ae1e495f00e06ffef8aa60156
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 2%

---


# Eliminación de registros

<!--take Preview and Production references out at release-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede eliminar los registros que ya no sean relevantes en Adobe Workfront Planning. <span class="preview">Puede recuperar los registros eliminados durante 30 días después de su eliminación. Para obtener información acerca de cómo recuperar los registros eliminados, vea [Recuperar registros eliminados](/help/quicksilver/planning/records/restore-deleted-records.md). </span>

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

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
   <td role="rowheader"><p>plan Adobe Workfront*</p></td> 
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
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p> 
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
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de Contribute o superiores para un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> </td> 
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

OLD

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
   <td role="rowheader"><p>Adobe Workfront license*</p>
   </td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning </p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
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

## Consideraciones acerca de la eliminación de registros

* Puede eliminar los registros que usted u otro usuario hayan creado.
* No se pueden recuperar los registros eliminados en el entorno de producción. <span class="preview">Puede recuperar los registros eliminados en el entorno de vista previa.</span>
* Si los registros eliminados están vinculados a otros registros, los registros vinculados no se eliminan, pero también se elimina la información del registro eliminado.
* No se pueden eliminar registros de la escala de tiempo o de las vistas de calendario.

## Eliminación de registros

Puede eliminar un registro de las siguientes áreas:

* [Desde la página del registro](#delete-a-record-from-the-records-page)
* [Desde la vista de tabla de un tipo de registro](#delete-a-record-from-the-record-type-table-view)

### Eliminar un registro de la página del registro

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee eliminar.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. Realice una de las siguientes acciones:

   * En la vista Tabla, haga clic en el nombre de un registro.
   * En la vista Tabla, pase el ratón sobre el nombre de un registro, haga clic en el menú **Más** ![](assets/more-menu.png) y, a continuación, haga clic en **Ver**

     ![](assets/contextual-menu-for-record-row.png)
   * En una vista Línea de tiempo, haga clic en una barra de registros.

   Se abre la página de registro.

1. Haga clic en el menú **Más** ![](assets/more-menu.png) que se encuentra a la derecha del nombre del registro, luego haga clic en **Eliminar** y después en **Eliminar** de nuevo para confirmar.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Se elimina el registro.
1. (Opcional y condicional) Si elimina el registro en el entorno de vista previa, vaya a la vista de tabla de la página del registro, haga clic en el icono **Deshacer** ![](assets/undo-icon.png) en la esquina superior derecha de la vista y, a continuación, haga clic en **Eliminados recientemente** para recuperar los registros eliminados.

Para obtener información acerca de cómo recuperar los registros eliminados, vea [Recuperar registros eliminados](/help/quicksilver/planning/records/restore-deleted-records.md).

### Eliminar un registro de la vista de tabla de tipo de registro

{{step1-to-planning}}

1. Haga clic en el área de trabajo cuyos registros desee eliminar.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) En el menú desplegable **Vista** de la esquina superior izquierda de la tabla, seleccione una Vista de tabla. Esta debe ser la vista predeterminada, a menos que haya visto el tipo de registro en la vista de escala de tiempo cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Realice una de las siguientes acciones:

   * Haga clic con el botón secundario en una fila de registro y luego haga clic en **Eliminar**.
   * Haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre del registro y, a continuación, haga clic en **Eliminar**.

     ![](assets/contextual-menu-for-record-row.png)

   * Haga clic en el icono **Abrir detalles** ![](assets/open-details-icon-in-table-name-field.png) para abrir el cuadro con la información detallada del registro, y haga clic en **Más** ![](assets/more-menu.png) a la derecha del nombre del registro y, a continuación, en **Eliminar**.

   Se elimina el registro.

1. (Opcional) Realice una de las siguientes acciones para deshacer o rehacer la eliminación de un registro:

   * <span class="preview">Haga clic en el icono **Deshacer** ![](assets/undo-icon.png) y después en **Eliminados recientemente** para recuperar los registros eliminados. Para obtener información acerca de cómo recuperar los registros eliminados, vea [Recuperar registros eliminados](/help/quicksilver/planning/records/restore-deleted-records.md). </span>
   * Utilice los siguientes métodos abreviados del teclado para deshacer o rehacer la eliminación de un registro:

      * CTRL + Z (⌘ + Z para Mac) para deshacer la eliminación de un registro
      * CTRL + Mayús + Z (⌘ + Mayús + Z para Mac) para rehacer la eliminación del registro




