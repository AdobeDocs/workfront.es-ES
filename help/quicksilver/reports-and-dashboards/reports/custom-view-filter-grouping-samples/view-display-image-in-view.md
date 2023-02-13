---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: mostrar una imagen en lugar de una cadena en una columna'
description: Puede reemplazar el nombre de un objeto de una vista con una imagen mediante el modo de texto. También puede agregar un vínculo a la imagen que pueda abrir el objeto al que reemplaza.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Ver: mostrar una imagen en lugar de una cadena en una columna

Puede reemplazar el nombre de un objeto de una vista con una imagen mediante el modo de texto. También puede agregar un vínculo a la imagen que pueda abrir el objeto al que reemplaza.

>[!NOTE]
>
>Las imágenes aparecen en su resolución real, por lo que intente utilizar imágenes pequeñas.

![](assets/replace-project-name-with-image-and-link-350x125.png)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Ejemplo: Sustituya el nombre de un proyecto en una vista de proyecto por una imagen:

1. Cargue una imagen en un sitio web o servidor externo a Adobe Workfront. Debe poder acceder a la imagen mediante el explorador web.

   >[!TIP]
   >
   >* Cada tipo de explorador es diferente, pero todos pueden mostrar direcciones URL.
   >* Evite utilizar imágenes cargadas en Workfront. Como las imágenes almacenadas en Workfront no están disponibles para el público y tienen una clave de acceso que caduca después de un período de tiempo, estas imágenes dejan de mostrarse en la vista a lo largo del tiempo.
   >* Una imagen guardada en el equipo no tiene una dirección URL inherente. Encuentre un sitio que proporcione alojamiento de imágenes y aloje su imagen allí. Es posible que su organización ya tenga un sitio de este tipo.


1. Con el explorador web, vaya a la imagen que guardó.
1. Obtenga la URL de la imagen haciendo lo siguiente:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Haga clic con el botón derecho y seleccione **Copiar ubicación de imagen** o **Obtener vínculo**, según el explorador. Ahora tiene la dirección URL de esa imagen específica y puede pegarla desde el portapapeles.
   1. Asegúrese de que todas las personas con ese vínculo tengan permisos para ver la imagen solo yendo al vínculo y que no necesiten un inicio de sesión para acceder a él.

1. Vaya a un proyecto y haga clic en el **Más** menú ![](assets/more-icon-45x33.png) junto al nombre del proyecto y, a continuación, haga clic en **Editar**.

1. En el **URL** , añada el vínculo a la imagen.
1. Vaya a la vista de un proyecto de una lista o informe y personalice la vista.
1. Haga clic en el encabezado de la columna de la **Nombre del proyecto** y haga clic en **Cambiar al modo de texto**.

1. Agregue el siguiente código a la columna del código existente:

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   La imagen seleccionada sustituye al nombre del proyecto en la vista del proyecto y la imagen es un vínculo al proyecto.

1. Haga clic en **Guardar vista**.
