---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: Editar permanentemente el ancho de una columna'
description: Puede modificar temporalmente el ancho de las columnas arrastrando y soltando sus márgenes para que coincidan con el ancho deseado. Para obtener más información, consulte Modificación del ancho y el orden de las columnas.
author: Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 90%

---

# Ver: editar de forma permanente la anchura de una columna

<!-- Audited: 11/2024 -->

Puede modificar temporalmente el ancho de las columnas arrastrando y soltando sus márgenes para que coincidan con el ancho deseado. Para obtener más información, consulte [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Para cambiar de forma permanente la anchura de cualquier columna de cualquier vista, debe utilizar el modo de texto en la columna mientras edita la vista.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o solicitud para modificar una vista </p>
   <p>Estándar o Plan para modificar un informe</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Informes, Paneles de control y Calendarios para modificar un informe</p> <p>Edición del acceso a Filtros, Vistas y Agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar de forma permanente la anchura de una columna

>[!IMPORTANT]
>
>Si modifica manualmente el ancho de una columna como se describe en la sección [Modificar el ancho y el orden de las columnas temporalmente](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) en el artículo [Modificar el ancho y el orden de las columnas](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) después de haber modificado permanentemente el ancho de la columna, el ancho de la columna se conservará según el cambio de tamaño manual. En este caso, se sobrescribe la anchura de la columna actualizada según los pasos siguientes. Puede ver la columna según el ancho definido en los pasos siguientes después de borrar la caché o iniciar sesión desde otro explorador.
>
>Para obtener información adicional acerca de cómo personalizar el ancho de las columnas al usar la interfaz de modo de texto, consulte las definiciones de &quot;ancho&quot; y &quot;estirado&quot; en el [Glosario de terminología de Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Ir a una lista de objetos.
1. En el menú desplegable **Vista**, haga clic en **Nueva vista**.

1. Haga clic en **Añadir columna** para añadir una columna nueva.

   O

   Haga clic en el encabezado de cualquier columna existente.

1. Haga glic en **Cambiar a modo texto**.
1. Haga Clic En **Editar Modo De Texto**.T
1. Agregue el siguiente código al modo de texto de la columna:

   ```
   width=200
   usewidths=true
   ```

   En la línea **width**, especifique cualquier número (en píxeles) que represente el ancho que desea que muestre la columna en la vista.

1. Haga clic en **Listo** y luego en **Guardar vista**.


