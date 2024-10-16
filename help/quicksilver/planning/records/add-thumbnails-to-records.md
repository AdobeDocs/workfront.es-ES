---
title: Agregar una miniatura a un registro
description: Puede editar la información del registro en Adobe Workfront Planning y asociar cada registro con miniaturas individuales para que sean fácilmente reconocibles.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---


# Añadir una miniatura en un registro

{{planning-important-intro}}

Puede asociar registros con miniaturas únicas en Adobe Workfront Planning para que sean fácilmente reconocibles.

Debe crear tipos de registros antes de empezar a crear y editar registros.
Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisitos de acceso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td> 
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
   <td><p> Estándar </p>
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
   <td>   <p>Administración de permisos en un espacio de trabajo </p>  
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

<!--OLD:


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
   <td> <p>There are no access controls for Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td>  <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfornt documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Consideraciones sobre las miniaturas de registros

Para distinguir visualmente entre registros en una vista de tabla, puede asociar una imagen en miniatura única a cada registro.

Tenga en cuenta lo siguiente:

* Una miniatura es única para un registro y no se aplica a todos los registros del mismo tipo.
* Solo puede agregar archivos de imagen como miniaturas.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Puede agregar una imagen en miniatura a registros individuales en la vista de tabla o desde la página o el cuadro de vista previa del registro.
* Workfront carga automáticamente una imagen en miniatura cada vez que crea un registro. Más adelante puede modificar esta imagen.
* Las miniaturas pertenecen a la información del registro y se muestran en las áreas en las que se muestran los registros. Por ejemplo, las miniaturas se muestran junto a la información de registro en las áreas siguientes:

   * Campo principal de un registro en la vista de tabla
   * Barra de registro en la vista de escala de tiempo.
   * Vista previa y página de detalles del registro.

## Añadir una miniatura en un registro

Puede añadir una miniatura de las siguientes maneras:

* [Agregar una miniatura a un registro desde la vista de tabla](#add-a-thumbnail-to-a-record-from-the-table-view)
* [Añadir una miniatura a un registro desde la página de detalles](#add-a-thumbnail-to-a-record-from-the-details-page)

### Agregar una miniatura a un registro desde la vista de tabla

{{step1-to-planning}}

1. Haga clic en el área de trabajo para cuyos registros desea agregar miniaturas y, a continuación, haga clic en la tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. Seleccione una vista de tabla del menú desplegable **Ver**. Todos los registros del tipo seleccionado se muestran en una tabla.
1. Pase el ratón sobre la información del campo principal, haga clic en el menú **Más** ![](assets/more-menu.png) y luego haga clic en **Miniatura**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   El campo principal es el campo que se muestra en la primera columna de una vista de tabla. El campo principal siempre está inmovilizado y no se puede ocultar ni reubicar. La opción Miniatura no está disponible en el menú Más cuando el campo principal es un campo de fórmula.

   La ficha **Cargar** se abre de forma predeterminada en el cuadro **Grabar miniatura**.

   Para obtener más información acerca de cómo cargar la miniatura, vea la sección [Agregar una miniatura a un registro desde la página de detalles](#add-a-thumbnail-to-a-record-from-the-details-page) en este artículo, a partir del paso 6. <!--see if this is accurate-->

<!--
   ![](assets/record-thumbnail-box-for-upload.png) 

  *****update screen shot with correct casing****

1. Drag and drop a file to add as a thumbnail
   
   Or
   
   Click **Browse images**, then browse for an image file to add. The file must be saved on your computer. 
1. (Optional) After the image uploads in the **Record thumbnail** box, use the sizing tool to crop and resize the image.
1. (Optional) Click the **Upload new image** icon ![](assets/upload-new-image-icon.png) to upload another image. 
1. (Optional) To remove a thumbnail before it is saved, click  **Remove uploaded image** icon ![](assets/remove-image-icon.png) to the right of the image. 
1. (Optional) Click the **Gallery** tab, then click an image. The gallery of images cannot be modified.

   ![](assets/record-thumbnail-box-for-gallery.png)
1. Click **Use image** to add the image as a thumbnail. 
   This closes the **Record thumbnail** box.
   The thumbnail displays in areas of Workfront Planning where the record displays. 

   >[!TIP]
   >
   >   You must enable the Thumbnail field in the table view to display thumbnails in this view. It is disabled by default.

1. (Optional) To remove the thumbnail after it is saved, hover over the primary field and click the **More** menu ![](assets/more-menu.png)> **Thumbnail** > the **Remove** icon ![](assets/remove-image-icon.png), then click **Save changes**. -->

### Añadir una miniatura a un registro desde la página de detalles

{{step1-to-planning}}

1. Haga clic en el área de trabajo para cuyos registros desea agregar miniaturas y, a continuación, haga clic en la tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. Desde cualquier vista, haga clic en un registro para abrirlo.

   Se muestra el cuadro de vista previa de detalles.
1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha.

   Se abre la página de detalles del registro.
1. Pase el ratón sobre la imagen en miniatura o el icono ![](assets/record-thumbnail-icon-on-details-page.png) y luego haga clic en el menú **Más** ![](assets/more-menu.png) > **Editar miniatura**.

   La ficha **Cargar** se abre de forma predeterminada en el cuadro **Grabar miniatura**.

   ![](assets/record-thumbnail-box-for-upload.png)

1. Arrastre y suelte un archivo para añadirlo como miniatura

   O

   Haz clic en **Examinar imágenes** y busca un archivo de imagen para agregar. El archivo debe guardarse en el equipo.

1. (Opcional) Una vez que la imagen se haya cargado en el cuadro **Grabar miniatura**, use la herramienta de ajuste de tamaño para recortar y cambiar el tamaño de la imagen.
1. (Opcional) Haga clic en el icono **Cargar nueva imagen** ![](assets/upload-new-image-icon.png) para cargar otra imagen.
1. (Opcional) Haga clic en la ficha **Galería** y, a continuación, haga clic en una imagen. La galería de imágenes no se puede modificar.

   ![](assets/record-thumbnail-box-for-gallery.png)

1. (Opcional) Para quitar la miniatura antes de guardarla, haga clic en el icono **Quitar** ![](assets/remove-image-icon.png) a la derecha de la imagen.

1. Haga clic en **Usar imagen** para agregar la imagen como miniatura.
Se cerrará el cuadro **Grabar miniatura**.
La miniatura aparece en áreas de Workfront Planning donde se muestra el registro.

   >[!TIP]
   >
   >   Debe habilitar el campo Miniatura en la vista de tabla para que se muestren miniaturas en esta vista. Está desactivada de forma predeterminada.

1. (Opcional) Para quitar la miniatura después de guardarla, haga clic en un registro de cualquier vista para abrir la página de detalles, pase el ratón sobre la imagen en miniatura y haga clic en el icono **Más** del menú ![](assets/more-menu.png)> **Quitar** ![](assets/remove-image-icon.png). Se elimina la imagen en miniatura.




<!--
### Generate a thumbnail for a record

{{step1-to-planning}}

1. Click the workspace for whose records you want to add thumbnails, then click the record type card. 

   This opens the record type page. 
1. Select a table view from the **View** drop-down menu. All records of the type you selected display in a table. 
1. Hover over the primary field information, click the **More** menu ![](assets/more-menu.png), then click **Thumbnail**. 

   ![](assets/record-more-menu-expanded.png)

      >[!TIP]
      >
      >   The primary field is the field that displays in the first column of a table view. The primary field is always frozen and cannot be hidden or relocated. 

   The **Record thumbnail** box opens.

(*************** update the screenshot below*************)
   ![](assets/record-thumbnail-box-for-upload.png) 

1. Click the **Generate** tab, and type a prompt describing the type of image you want to add in the space provided. 
1. Click **Generate**. 

   A set of four suggested images displays. 

1. Click an image to select it, then click **Use image**. 

   The Record thumbnail box closes and the thumbnail is attached to the record. All users who can view the records can now see the selected thumbnail. 
1. (Optional) Click the **More** menu ![](assets/more-menu.png) to the right of the record name in the table view, then click **Thumbnail**. 

   The generated image opens in the **Upload** tab where you can modify or remove it, as described in the section [Upload a thumbnail to a record](#upload-a-thumbnail-to-a-record) in this article. 
-->