---
title: Añadir miniaturas a los registros
description: Puede editar la información del registro en Adobe Workfront Planning y asociar cada registro con miniaturas individuales para que sean fácilmente reconocibles.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b22c4955-c3f2-4841-a278-bb40e8890ed9
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Añadir miniaturas a los registros

{{maestro-important-intro}}

Puede asociar registros con miniaturas únicas en la planificación de Adobe Workfront para que sean fácilmente reconocibles.

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
<p>Su organización debe estar inscrita en el programa beta de planificación de Adobe Workfront. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td> <p>No hay controles de acceso para la planificación de Workfront </p>  
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

## Consideraciones sobre las miniaturas de registros

Para distinguir visualmente entre registros en una vista de tabla, puede asociar una imagen en miniatura única a cada registro.

Tenga en cuenta lo siguiente:

* Solo puede agregar archivos de imagen como miniaturas.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Puede agregar una imagen en miniatura a registros individuales en la vista de tabla.
* Las miniaturas pertenecen a la información del registro y se muestran en las vistas en las que se muestran los registros. Por ejemplo, las miniaturas se muestran junto a la información de registro en las áreas siguientes:

   * Campo principal de un registro en la vista de tabla
   * Barra de registro en la vista de escala de tiempo.
* No se pueden agregar miniaturas de registros desde la página Detalles del registro o en la vista de escala de tiempo.
* Las miniaturas no se muestran en la página Detalles del registro.

## Añadir una miniatura en un registro

{{step1-to-maestro}}

1. Seleccione el espacio de trabajo para cuyos registros desea agregar miniaturas y, a continuación, haga clic en la tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. Seleccione una vista de tabla de la **Ver** menú desplegable. Todos los registros del tipo seleccionado se muestran en una tabla.
1. Pase el ratón sobre la información del campo principal y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Miniatura**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   El campo principal es el campo que se muestra en la primera columna de una vista de tabla. El campo principal siempre está inmovilizado y no se puede ocultar ni reubicar.

   El **Grabar miniatura** se abre el cuadro.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. En el **Cargar** , arrastre y suelte un archivo para añadirlo como miniatura O haga clic en **Seleccionar para cargar**, a continuación busque un archivo de imagen para añadir. El archivo debe guardarse en el equipo.
1. (Opcional) Utilice la herramienta de ajuste de tamaño para recortar y cambiar el tamaño de la imagen.
1. Clic **Usar imagen** para añadir la imagen como miniatura.
Esto cierra el **Grabar miniatura** cuadro.
1. (Condicional) Si tiene al menos permisos de contribución en la vista de tabla, haga clic en **Campos** en la esquina superior derecha de la vista de tabla.
1. Seleccione el **Miniatura** alternar para mostrar la miniatura. De forma predeterminada, esta opción no está seleccionada.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   La miniatura se muestra a la izquierda del valor del campo principal.
1. (Opcional y condicional) Si no dispone de permisos de contribución o superiores para la vista, seleccione una nueva vista de la **Ver** menú desplegable o cree una vista.
1. (Opcional) Para quitar la miniatura, pase el ratón sobre el campo principal y haga clic en el botón **Más** menú ![](assets/more-menu.png)> **Miniatura** > el **Eliminar** icono ![](assets/remove-image-icon.png), luego haga clic en **Guardar cambios**.
