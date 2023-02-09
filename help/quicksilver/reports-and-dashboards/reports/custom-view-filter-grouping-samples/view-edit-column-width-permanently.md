---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: editar permanentemente la anchura de una columna'
description: Puede modificar temporalmente el ancho de las columnas arrastrando y soltando sus márgenes para que coincidan con el ancho deseado. Para obtener más información, consulte Modificación del orden y el ancho de la columna.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: bb348deb9841320a367695845efe0ca36a9a9d8b
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Ver: editar permanentemente el ancho de una columna

Puede modificar temporalmente el ancho de las columnas arrastrando y soltando sus márgenes para que coincidan con el ancho deseado. Para obtener más información, consulte [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Puede cambiar de forma permanente el ancho de cualquier columna de cualquier vista mediante el modo de texto de la columna mientras edita la vista.

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

## Editar permanentemente el ancho de una columna

>[!IMPORTANT]
>
>Si modifica manualmente la anchura de una columna como se describe en la sección &quot;Modificación temporal del ancho y el orden de las columnas&quot; del artículo [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) después de modificar permanentemente el ancho de la columna, el ancho de la columna se conserva según el cambio de tamaño manual y se sobrescribe el ancho de la columna actualizado según los pasos siguientes. Puede ver la columna según el ancho definido en los pasos siguientes después de borrar la caché o iniciar sesión desde otro explorador.

1. Ir a una lista de objetos.
1. En el **Ver** menú desplegable, haga clic en **Nueva vista**.

1. Haga clic en **Agregar columna** para agregar una columna nueva.

   O

   Haga clic en el encabezado de columna de cualquier columna existente.

1. Haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área del modo de texto y haga clic en **Haga clic para editar texto**.
1. Agregue el siguiente código al modo de texto de la columna :

   ```
   width=200
   usewidths=true
   ```

   Para la variable **width** línea, especifique cualquier número (en píxeles) que represente la anchura con la que desea que se muestre la columna en la vista.

1. Haga clic en **Guardar**, luego **Guardar vista**.
