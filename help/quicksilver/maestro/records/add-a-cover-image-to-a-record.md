---
title: Agregar una imagen de portada a un registro
description: Puede personalizar los registros agregando una imagen de portada a la página de registros en Adobe Workfront Planning, al editar un registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---


<!--update the metadata with real information-->

# Agregar una imagen de portada a un registro

{{maestro-important-intro}}

Puede personalizar los registros agregando una imagen de portada a la página de registros en Adobe Workfront Planning, al editar un registro.

Para obtener información sobre cómo editar registros, consulte [Edición de registros](/help/quicksilver/maestro/records/edit-records.md).

Debe crear tipos de registros antes de empezar a crear y editar registros.

Para obtener más información, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

## Requisitos de acceso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <p>Cualquiera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de acceso para Workfront Planning </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Permisos de contribución o superiores en un espacio de trabajo </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td>  <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> <p>Para obtener más información, consulte <a href="/help/quicksilver/maestro/access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Consideraciones acerca de grabar imágenes de portada de página

Puede personalizar la página de un registro agregándole una imagen de portada.

Tenga en cuenta lo siguiente:

* Una imagen de portada es única para un registro y no se aplica a todos los registros del mismo tipo.
* Solo se pueden agregar archivos de imagen como imágenes de portada.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Puede agregar una imagen de portada a registros individuales desde la vista previa de los registros en cualquier vista o desde la página de registros.
* No puede agregar imágenes de portada en línea desde ninguna vista de registros.

## Agregar una imagen de portada a un registro

Puede personalizar un registro agregando una imagen de portada en la parte superior de la vista previa del registro o de la página.

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

1. En la página de vista previa o de registro, haga clic en **Añadir portada**. <!--check the casing here; I logged a bug for this-->
El **Cubierta de registro** se abre el cuadro.

1. Clic **Seleccionar para cargar** y busque una imagen en el equipo para seleccionarla, agréguela y haga clic en **Usar imagen**.

   La imagen se carga en la parte superior de la página o vista previa del registro y los cambios se guardan automáticamente.

   ![](assets/record-page-with-cover-image.png)

1. (Opcional) Pase el ratón sobre la imagen y haga clic en **Más** menú ![](assets/more-menu.png) en la esquina inferior derecha de la imagen de la portada, siga uno de estos procedimientos:

   * Clic **Cargar** Si desea reemplazar la imagen de portada, repita el Paso 6 para cargar y guardar una nueva imagen.
   * Clic **Cambiar posición** y utilice el **Cambiar posición** herramienta ![](assets/reposition-tool-icon.png) para centrar la imagen de la portada, haga clic en **Guardar** cuando termine.
   * Clic **Eliminar** para quitar la imagen de portada.

   Workfront guarda automáticamente los cambios.
