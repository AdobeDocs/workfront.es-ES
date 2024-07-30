---
title: Administrar el diseño de página de registro
description: Puede editar el diseño de la vista previa y la página del registro en Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Administrar el diseño de página de registro

{{planning-important-intro}}

Puede editar el diseño de la vista previa y la página del registro en Adobe Workfront Planning.

La vista previa de registros es una vista más pequeña de la página de registros que se muestra en la vista de un tipo de registro.

Al cambiar el diseño de una vista previa y una página de registro, los cambios afectan a los cuadros de vista previa y a las páginas de detalles de todos los registros del mismo tipo.

Este artículo describe cómo puede cambiar el diseño y el aspecto de un cuadro de vista previa de registro o de una página de registro. Para obtener información sobre cómo editar registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

Debe crear tipos de registros y registros antes de poder empezar a editar páginas de registros.

Para obtener más información, consulte los siguientes artículos:

* [Creación de tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md)

* [Creación de registros](/help/quicksilver/planning/records/create-records.md)

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

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
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p>
   O
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administrar permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones sobre la edición de páginas de registro

* De forma predeterminada, las páginas de detalles y de vista previa de un registro muestran todos los campos asociados con el registro.

* No se pueden agregar nuevos campos para un registro en la página de vista previa o de detalles. Debe agregar nuevos campos en la vista de tabla para mostrarlos en las páginas de vista previa y detalles.

* Puede agregar secciones a una vista previa de registro o a una página de detalles para organizar la información según criterios comunes y facilitar su búsqueda.

* Los siguientes cambios afectan a todos los registros del mismo tipo y son visibles para todos los usuarios que acceden a esos registros:

   * Reorganización de campos
   * Agregar o quitar secciones

* Los cambios de visualización que realice en la vista previa del registro se pueden ver inmediatamente en la página de detalles del registro. Los cambios realizados en la página de registro también se pueden ver en el cuadro de vista previa del registro.

* La adición de una imagen de portada o una miniatura a un registro no forma parte del diseño general de la vista previa o la página del registro. Puede agregar imágenes de portada o miniaturas únicas a cada registro. Para obtener más información, vea [Agregar una imagen de portada a un registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) y [Agregar una miniatura a un registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Agregar secciones a una vista previa de registro o página

Tenga en cuenta lo siguiente al agregar secciones a una página de registro:

* No hay límite en cuanto a la cantidad de secciones que se pueden tener en una página.
* No puede tener una sección vacía. Debe haber al menos un campo en una sección.
* Puede arrastrar y soltar campos de una sección a otra. Para obtener más información, vea la sección [Reorganizar campos en la vista previa de registro o en la página de detalles](#rearrange-fields-in-the-record-preview-or-details-page) de este artículo.
* Al eliminar todos los campos de una sección, esta se elimina automáticamente y no se puede recuperar.

Para agregar una sección a una vista previa de registro o a una página:

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el nombre de un registro

   O

   En la vista de tabla, haga clic en el icono **Abrir detalles** ![](assets/open-details-icon-in-table-name-field.png) de la primera columna.

   La vista previa del registro se abrirá en la vista.

   ![](assets/details-box.png)

1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una ficha nueva.

   Se abre la página de registro.

   ![](assets/details-page.png)

1. En la página o vista previa del registro, pase el ratón sobre el espacio en blanco que hay a la izquierda de los campos y, a continuación, haga clic en el icono **Agregar sección** ![](assets/add-section-icon.png) para agregar una sección.
1. Haga clic dentro del nombre de la sección y reemplace **Sección sin título** por un nombre; a continuación, haga clic en Entrar. Los campos que se muestran en la sección forman parte automáticamente de la nueva sección.
1. Empiece a arrastrar y soltar campos en la nueva sección, tal como se describe en la sección [Reorganizar campos en la vista previa del registro o en la página de detalles](#rearrange-fields-in-the-record-preview-or-details-page) de este artículo.

1. (Opcional) Pase el ratón sobre el nombre de una sección y haga clic en el menú **Más** ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Opcional) Realice una de las siguientes acciones para editar la sección:

   * Haga clic en **Cambiar nombre** para cambiar el nombre de la sección

     >[!TIP]
     >
     > Puede cambiar el nombre de una sección en línea haciendo clic en el nombre.

   * Haga clic en **Subir** para subir la sección una posición

     O

     Haga clic en **Bajar** para bajar la sección una posición.
Todos los campos de la sección se mueven con la sección.

   * Haga clic en **Eliminar** para eliminar la sección. La sección se elimina y no se puede recuperar. Todos los usuarios que accedan a los registros de este tipo ya no verán la sección eliminada.

1. Haga clic en la flecha hacia abajo situada a la izquierda del nombre de la sección para contraerla o en la flecha hacia la derecha para expandirla.
Todas las secciones se expanden de forma predeterminada.

1. (Opcional) Haga clic en el icono **asidero** ![](assets/grab-icon.png) a la izquierda del nombre de una sección y, a continuación, arrástrela y suéltela en el lugar que desee.

   La nueva posición de la sección se actualiza tanto en la vista previa como en la página de todos los registros del mismo tipo para todos los usuarios que ven los registros.

   Todos los cambios realizados en las secciones y el orden de los campos se guardan automáticamente.

## Reorganizar campos en la página de vista previa o detalles del registro

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el nombre de un registro

   O

   En la vista de tabla, haga clic en el icono **Abrir detalles** ![](assets/open-details-icon-in-table-name-field.png) de la primera columna.

   La vista previa del registro se abrirá en la vista.

   ![](assets/details-box.png)

1. (Opcional) Haga clic en el icono **Abrir en ficha nueva** ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una nueva pestaña.

   Se abre la página de registro.

   ![](assets/details-page.png)

1. En la página o vista previa del registro, haga clic en el icono **asir** ![](assets/grab-icon.png) que hay a la izquierda del nombre de campo y, a continuación, arrástrelo y suéltelo en el lugar que desee. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   La nueva posición del campo se actualiza tanto en la vista previa como en la página de todos los registros del mismo tipo para todos los usuarios que ven los registros.

   Todos los cambios en el diseño de la vista previa del registro o de la página se guardan automáticamente.

