---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: editar de forma permanente la anchura de una columna"
description: Puede modificar temporalmente el ancho de las columnas arrastrando y soltando sus márgenes para que coincidan con el ancho deseado. Para obtener más información, consulte Modificación del ancho y el orden de las columnas.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 261c1b73d785094de4ee8549c856a091920ba04a
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Ver: editar de forma permanente la anchura de una columna

<!-- Audited: 1/2024 -->

Puede modificar temporalmente el ancho de las columnas arrastrando y soltando sus márgenes para que coincidan con el ancho deseado. Para obtener más información, consulte [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Para cambiar de forma permanente la anchura de cualquier columna de cualquier vista, debe utilizar el modo de texto en la columna mientras edita la vista.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo:<ul><li>Colaborador para modificar una vista</li><li>Estándar para modificar un informe</li></ul></p><p>O</p>Actual:<ul><li>Solicitud para modificar una vista</li><li>Plan para modificar un informe</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Editar de forma permanente la anchura de una columna

>[!IMPORTANT]
>
>Si modifica manualmente el ancho de una columna como se describe en la sección [Modificar temporalmente el ancho y el orden de las columnas](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) en el artículo [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) después de modificar permanentemente el ancho de la columna, el ancho de la columna se conserva según el cambio de tamaño manual. En este caso, se sobrescribe la anchura de la columna actualizada según los pasos siguientes. Puede ver la columna según el ancho definido en los pasos siguientes después de borrar la caché o iniciar sesión desde otro explorador.
>
>Para obtener información adicional sobre cómo personalizar el ancho de las columnas al utilizar la interfaz del Modo de texto, consulte las definiciones de &quot;ancho&quot; y &quot;ampliación&quot; en la [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

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


