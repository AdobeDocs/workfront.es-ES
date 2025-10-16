---
title: Exportar registros desde la vista de tabla
description: Puede exportar registros y su información desde la vista de tabla a un archivo CSV o de Excel.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 3%

---

# Exportar registros desde la vista de tabla

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede exportar registros y su información desde la vista de tabla a un archivo de Excel o CSV en Adobe Workfront Planning.

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
   <td><p>Ligero o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Ver permisos superiores a un espacio de trabajo y un tipo de registro</p>   
   <p>Ver o permisos superiores a una vista</p>

</td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>
</td>
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
   <td><p> Light or higher </p>
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
   <td>   <p>View or higher permissions to a view</p>  
   </td> 
  </tr> 
</tbody> 
</table> -->


## Exportar registros desde la vista de tabla

Tenga en cuenta lo siguiente al exportar la vista de tabla:

* La información exportada a un archivo de Excel conserva los filtros, agrupaciones y ordenaciones aplicados a la vista de tabla en Workfront Planning. Las agrupaciones no son visibles en el archivo CSV.

* Los archivos exportados no admiten miniaturas ni colores de fila personalizados.

* Solo se exportan los campos que se hacen visibles en la interfaz de Workfront. Los campos ocultos no se exportan.

Para exportar información desde la vista de tabla o un tipo de registro:

1. Vaya a una página de tipo de registro y haga clic en una ficha de vista de tabla.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre el nombre de la pestaña de la vista de tabla, luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png) a la derecha del nombre de la vista y luego haga clic en **Exportar**.

   ![Menú Más en una vista](assets/view-more-menu-with-duplicate-option.png)

   * Haga clic en **Compartir** > **Exportar la vista actual**. Esta opción sólo está disponible cuando se muestra la vista de tabla.

   ![Botón Compartir con tipo de registro y ver opciones de uso compartido](assets/share-button-with-record-type-and-view-sharing-options.png)

1. Seleccione uno de los siguientes formatos:

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >No se puede exportar información desde la vista de tabla cuando se muestra una vista diferente en la pantalla. Debe mostrar la vista de tabla que desea exportar para acceder a la opción Exportar en el menú Más.

   El archivo se descargará en el equipo.

1. (Opcional) Vaya a la carpeta de descargas del equipo y busque el archivo descargado.

   El nombre del archivo exportado sigue el siguiente formato:

   `Name of the view - name of the record type`

   Por ejemplo, una vista de tabla para el tipo de registro Campañas genera un archivo denominado `Table view - Campaigns`.

   El archivo muestra la siguiente información:

   * Los encabezados de columna se resaltan en negro en el archivo de Excel
   * Todos los campos visibles en la interfaz de Workfront, ordenados y filtrados según los mismos criterios
   * Las agrupaciones se conservan en el archivo de Excel

   Ahora puede compartir los archivos exportados con otros usuarios o adjuntarlos a cualquier comunicación.

</div>
