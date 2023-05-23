---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: editar de forma permanente la anchura de una columna"
description: Puede modificar temporalmente el ancho de las columnas arrastrando y soltando sus márgenes para que coincidan con el ancho deseado. Para obtener más información, consulte Modificación del ancho y el orden de las columnas.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Ver: editar de forma permanente la anchura de una columna

Puede modificar temporalmente el ancho de las columnas arrastrando y soltando sus márgenes para que coincidan con el ancho deseado. Para obtener más información, consulte [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Puede cambiar de forma permanente la anchura de cualquier columna de cualquier vista utilizando el modo de texto en la columna mientras edita la vista.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud para modificar una vista </p>
   <p>Plan para modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Editar de forma permanente la anchura de una columna

>[!IMPORTANT]
>
>Si modifica manualmente la anchura de una columna como se describe en la sección &quot;Modificación temporal de la anchura y el orden de las columnas&quot; del artículo [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) después de modificar permanentemente el ancho de la columna, el ancho de la columna se conserva según el cambio de tamaño manual y el ancho de la columna se actualiza según los pasos siguientes. Puede ver la columna según el ancho definido en los pasos siguientes después de borrar la caché o iniciar sesión desde otro explorador.

1. Ir a una lista de objetos.
1. Desde el **Ver** , haga clic en **Nueva vista**.

1. Clic **Agregar columna** para añadir una nueva columna.

   O

   Haga clic en el encabezado de cualquier columna existente.

1. Clic **Cambiar a modo de texto**.
1. Pase el ratón sobre el área de modo de texto y haga clic en **Haga clic para editar el texto**.
1. Agregue el siguiente código al modo de texto de la columna:

   ```
   width=200
   usewidths=true
   ```

   Para el **anchura** , especifique cualquier número (en píxeles) que represente el ancho que desea que muestre la columna en la vista.

1. Clic **Guardar**, entonces **Guardar vista**.
