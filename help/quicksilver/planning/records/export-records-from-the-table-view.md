---
title: Exportar registros desde la vista de tabla
description: Puede exportar registros y su información desde la vista de tabla a un archivo CSV o de Excel.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d8ac4d94-28b5-41d6-acb8-259696897c8a
source-git-commit: 10fec10e1bb885ac20e1ef9526cfa8a59086d874
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 11%

---

# Exportar registros desde la vista de tabla

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Puede exportar registros y su información desde la vista de tabla a un archivo de Excel o CSV en Adobe Workfront Planning.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Ligero o superior </p>
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
   <td>   <p>Ver o permisos superiores a una vista</p>  
   </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
