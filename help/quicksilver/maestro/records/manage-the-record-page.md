---
title: Administrar la página de registro
description: Puede editar y administrar el diseño del cuadro de registro y la página en Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Administrar la página de registro

{{maestro-important-intro}}

Puede editar y administrar el diseño del cuadro de registro y la página en Adobe Workfront Planning. Puede mostrar el cuadro de registro en una vista de registros.

El cuadro de registro es una vista más pequeña de la página de registro que se muestra en la vista de un tipo de registro.

Al cambiar el diseño de un cuadro de registro y de una página, el cuadro y la página cambian para todos los registros del mismo tipo.

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

* Al reorganizar los campos del cuadro de registro o de la página, se reorganizan los campos de todos los registros de ese tipo y de todos los usuarios que tienen acceso a esos registros.
* Agregar una imagen de portada a un registro no forma parte del diseño general del cuadro de registros o de la página. Puede agregar imágenes de portada únicas a cada registro. Para obtener más información, consulte [Agregar una imagen de portada a un registro](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

## Reorganizar campos en el cuadro de registro o en la página

{{step1-to-maestro}}

El espacio de trabajo al que se accede por última vez se abre.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.
1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

1. Desde cualquier vista, haga clic en el nombre de un registro

   O

   En la vista de tabla de tabla, haga clic en **Abrir detalles** icono ![](assets/open-details-icon-in-table-name-field.png) a la izquierda del nombre de un registro.

   El cuadro del registro se abre en la vista.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Puede ver el **Abrir detalles** a la izquierda del campo Nombre de un registro en una vista de tabla sólo cuando el campo Nombre es un campo principal.

1. (Opcional) Haga clic en **Abrir en ficha nueva** icono ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> en la esquina superior derecha del cuadro de registro para abrir la página del registro en una nueva ficha.

   Se abre la página de registro.

   ![](assets/details-page.png)

1. En el cuadro de registro o la página, haga clic en el icono de captura ![](assets/grab-icon.png) a la izquierda del nombre de un campo, arrástrelo y suéltelo en el lugar que desee.

   La nueva posición del campo se actualiza tanto en el cuadro como en la página de todos los registros del mismo tipo para todos los usuarios que ven los registros.

   Todos los cambios realizados en el diseño del cuadro de registro o de la página se guardan automáticamente.

