---
title: Agregar una imagen de portada a un registro
description: Puede personalizar los registros agregando una imagen de portada a la página de registros en Adobe Workfront Planning, al editar un registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 1%

---


# Agregar una imagen de portada a un registro

{{planning-important-intro}}

Puede personalizar los registros agregando una imagen de portada a la página de registros en Adobe Workfront Planning, al editar un registro.

Para obtener información sobre cómo editar registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

Debe crear tipos de registros antes de empezar a crear y editar registros.

Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

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

## Consideraciones acerca de grabar imágenes de portada de página

Puede personalizar la página de un registro agregándole una imagen de portada.

Tenga en cuenta lo siguiente:

* Una imagen de portada es única para un registro y no se aplica a todos los registros del mismo tipo.
* Solo se pueden agregar archivos de imagen como imágenes de portada.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Puede agregar una imagen de portada a registros individuales desde la vista previa de los registros en cualquier vista o desde la página de registros.
* No se pueden agregar imágenes de portada desde una vista de registros.
* Workfront carga automáticamente una imagen de portada cada vez que crea un registro. Más adelante puede modificar esta imagen.

## Agregar una imagen de portada a un registro

Puede personalizar un registro agregando una imagen de portada en la parte superior de la vista previa del registro o de la página.

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos registros desee personalizar,

   O

   Desde un espacio de trabajo, expanda la flecha hacia abajo a la derecha del nombre de un espacio de trabajo existente, busque un espacio de trabajo y selecciónelo cuando se muestre en la lista.

   Se abre el espacio de trabajo y se muestran los tipos de registro.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en un registro

   O

   En la vista de tabla, haga clic en el icono **Abrir detalles** ![](assets/open-details-icon-in-table-name-field.png) de la primera columna.

   La vista previa del registro se abrirá en la vista.

   ![](assets/details-box.png)

1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una nueva pestaña.

   Se abre la página de registro.

   ![](assets/details-page.png)

1. En la página o vista previa del registro, haga clic en **Agregar portada**


   O

   Pase el ratón sobre una imagen de portada existente, haga clic en el menú **Más** ![](assets/more-menu.png) y luego haga clic en **Cargar**. <!--check the casing here; I logged a bug for this-->
El cuadro **Cubierta de registro** se abre en la ficha **Cargar**.

   ![](assets/record-cover-box-for-upload.png)

1. Haz clic en **Examinar imágenes** y busca una imagen en tu equipo para seleccionarla y agregarla.

1. (Opcional) Para quitar la imagen antes de guardarla, haga clic en el icono **Cargar nueva imagen** ![](assets/upload-new-image-icon.png) y cargue una nueva imagen.

1. (Opcional) Haga clic en la ficha **Galería** y luego haga clic en una imagen de la galería de imágenes. La galería de imágenes no se puede modificar.

   ![](assets/record-cover-box-for-gallery.png)

1. Haga clic en **Usar imagen**.

   La imagen se carga en la parte superior de la página o vista previa del registro y los cambios se guardan automáticamente.

   ![](assets/record-page-with-cover-image.png)

1. (Opcional) Pase el ratón sobre la imagen, luego haga clic en el menú **Más** ![](assets/more-menu.png) en la esquina inferior derecha de la imagen de la portada y siga uno de estos procedimientos:

   * Haz clic en **Cargar** si deseas reemplazar la imagen de portada y repite el paso 6 para cargar y guardar una nueva imagen.
   * Haga clic en **Cambiar posición**, use la herramienta **Cambiar posición** ![](assets/reposition-tool-icon.png) para centrar la imagen de portada y, después, haga clic en **Guardar** cuando haya terminado.
   * Haz clic en **Quitar** para quitar la imagen de la portada.

   Workfront guarda automáticamente los cambios.
