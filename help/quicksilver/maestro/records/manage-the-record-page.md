---
title: Administrar la página de registro
description: Puede editar el diseño de la vista previa y la página del registro en Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Administrar la página de registro

{{planning-important-intro}}

Puede editar el diseño de la vista previa y la página del registro en Adobe Workfront Planning.

La vista previa de registros es una vista más pequeña de la página de registros que se muestra en la vista de un tipo de registro.

Al cambiar el diseño de una vista previa y una página de registro, los cambios afectan a los cuadros de vista previa y a las páginas de detalles de todos los registros del mismo tipo.

Este artículo describe cómo puede cambiar el diseño y el aspecto de un cuadro de vista previa de registro o de una página de registro. Para obtener información sobre cómo editar registros, consulte [Edición de registros](/help/quicksilver/maestro/records/edit-records.md).

Debe crear tipos de registros y registros antes de poder empezar a editar páginas de registros.

Para obtener más información, consulte los siguientes artículos:

* [Creación de tipos de registros](../architecture/create-record-types.md)

* [Creación de registros](/help/quicksilver/maestro/records/create-records.md)

## Requisitos de acceso

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta de Adobe Workfront Planning. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <p>Nuevo: claro o superior</p>
   O
   <p>Actual: Trabajo o superior</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administrar permisos superiores a un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Consideraciones sobre la edición de páginas de registro

* De forma predeterminada, las páginas de detalles y de vista previa de un registro muestran todos los campos asociados con el registro.

* No se pueden agregar nuevos campos para un registro en la página de vista previa o de detalles. Debe agregar nuevos campos en la vista de tabla para mostrarlos en las páginas de vista previa y detalles.

* Puede agregar secciones a una vista previa de registro o a una página de detalles para organizar la información según criterios comunes y facilitar su búsqueda.

* Los siguientes cambios afectan a todos los registros del mismo tipo y son visibles para todos los usuarios que acceden a esos registros:

   * Reorganización de campos
   * Agregar o quitar secciones

* Los cambios de visualización que realice en la vista previa del registro se pueden ver inmediatamente en la página de detalles del registro. Los cambios realizados en la página de registro también se pueden ver en el cuadro de vista previa del registro.

* Agregar una imagen de portada a un registro no forma parte del diseño general de la vista previa del registro o de la página. Puede agregar imágenes de portada únicas a cada registro. Para obtener más información, consulte [Agregar una imagen de portada a un registro](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

## Agregar secciones a una vista previa de registro o página

Tenga en cuenta lo siguiente al agregar secciones a una página de registro:

* No hay límite en cuanto a la cantidad de secciones que se pueden tener en una página.
* No puede tener una sección vacía. Debe haber al menos un campo en una sección.
* Puede arrastrar y soltar campos de una sección a otra. Para obtener más información, consulte la sección [Reorganizar campos en la página de vista previa o detalles del registro](#rearrange-fields-in-the-record-preview-or-details-page) en este artículo.
* Al eliminar todos los campos de una sección, esta se elimina automáticamente y no se puede recuperar.

Para agregar una sección a una vista previa de registro o a una página:

{{step1-to-maestro}}

El espacio de trabajo al que se accede por última vez se abre.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.
1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el nombre de un registro

   O

   En la vista de tabla de tabla, haga clic en **Abrir detalles** icono ![](assets/open-details-icon-in-table-name-field.png) a la izquierda del nombre de un registro.

   La vista previa del registro se abrirá en la vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Puede ver el **Abrir detalles** a la izquierda del campo Nombre de un registro en una vista de tabla sólo cuando el campo Nombre es un campo principal.

1. (Opcional) Haga clic en **Abrir en ficha nueva** icono ![](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una nueva pestaña.

   Se abre la página de registro.

   ![](assets/details-page.png)

1. En la página o vista previa del registro, pase el ratón sobre el espacio en blanco a la izquierda de los campos y, a continuación, haga clic en **Agregar sección** icono ![](assets/add-section-icon.png) para añadir una sección.
1. Haga clic dentro del nombre de la sección y reemplace **Sección sin título** con un nombre y, a continuación, haga clic en Entrar. Los campos que se muestran en la sección forman parte automáticamente de la nueva sección.
1. Arrastre y suelte los campos en la nueva sección, tal como se describe en la sección [Reorganizar campos en la página de vista previa o detalles del registro](#rearrange-fields-in-the-record-preview-or-details-page) en este artículo.

1. (Opcional) Pase el ratón sobre el nombre de una sección y haga clic en el botón **Más** menú ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Opcional) Realice una de las siguientes acciones para editar la sección:

   * Clic **Cambiar nombre** para cambiar el nombre de la sección

     >[!TIP]
     >
     > Puede cambiar el nombre de una sección en línea haciendo clic en el nombre.

   * Clic **Mover hacia arriba** para subir la sección una posición

     O

     Clic **Mover hacia abajo** para bajar la sección una posición.
Todos los campos de la sección se mueven con la sección.

   * Clic **Eliminar** para eliminar la sección. La sección se elimina y no se puede recuperar. Todos los usuarios que accedan a los registros de este tipo ya no verán la sección eliminada.

1. Haga clic en la flecha hacia abajo situada a la izquierda del nombre de la sección para contraerla o en la flecha hacia la derecha para expandirla.
Todas las secciones se expanden de forma predeterminada.

1. (Opcional) Haga clic en **agarrar** icono ![](assets/grab-icon.png) a la izquierda del nombre de una sección y, a continuación, arrástrela y suéltela en el lugar que desee.

   La nueva posición de la sección se actualiza tanto en la vista previa como en la página de todos los registros del mismo tipo para todos los usuarios que ven los registros.

   Todos los cambios realizados en las secciones y el orden de los campos se guardan automáticamente.

## Reorganizar campos en la página de vista previa o detalles del registro

{{step1-to-maestro}}

El espacio de trabajo al que se accede por última vez se abre.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.
1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el nombre de un registro

   O

   En la vista de tabla de tabla, haga clic en **Abrir detalles** icono ![](assets/open-details-icon-in-table-name-field.png) a la izquierda del nombre de un registro.

   La vista previa del registro se abrirá en la vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Puede ver el **Abrir detalles** a la izquierda del campo Nombre de un registro en una vista de tabla sólo cuando el campo Nombre es un campo principal.

1. (Opcional) Haga clic en **Abrir en ficha nueva** icono ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha de la vista previa del registro para abrir la página del registro en una nueva pestaña.

   Se abre la página de registro.

   ![](assets/details-page.png)

1. En la página de vista previa o de registro, haga clic en **agarrar** icono ![](assets/grab-icon.png) a la izquierda del nombre de un campo, arrástrelo y suéltelo en el lugar que desee. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   La nueva posición del campo se actualiza tanto en la vista previa como en la página de todos los registros del mismo tipo para todos los usuarios que ven los registros.

   Todos los cambios en el diseño de la vista previa del registro o de la página se guardan automáticamente.

