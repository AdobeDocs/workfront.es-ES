---
product-area: requests
navigation-topic: create-requests
title: Creación y administración de vistas en el área de solicitudes
description: Si utiliza la nueva experiencia de solicitud, puede crear y guardar vistas para el área de solicitudes.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 31aff197d6af521df2258f3f99fea6fb5785b9e3
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 10%

---


# Creación y administración de vistas en el área de solicitudes

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

Si utiliza la nueva experiencia de solicitud en Adobe Workfront, puede crear y guardar vistas para el área de solicitudes. Estas vistas incluyen filtros, disposiciones de columna y agrupaciones.

>[!IMPORTANT]
>
>* Esta funcionalidad solo está disponible en la nueva experiencia de solicitud del área de solicitudes.
>* La configuración de vista también está disponible en el widget Mis solicitudes de Inicio. Sin embargo, las vistas del área de Solicitudes son independientes de las del widget Mis solicitudes.
>* La lista de solicitudes del área de solicitudes y el widget Mi trabajo utilizan la lista mejorada de Workfront. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de flujo de trabajo o Workfront</p>
   <p>Cualquier licencia de Workfront Planning para ver solicitudes de Workfront Planning en listas de solicitudes</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p>  <p>Debe ser administrador de Workfront para agregar vistas a las plantillas de diseño</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vistas del sistema para solicitudes

>[!WARNING]
>
>Las vistas del sistema documentadas en esta sección aún no están disponibles. Estarán disponibles en una fecha posterior al 16 de abril de 2026.

Además de las vistas que puede crear usted mismo, Workfront ofrece las siguientes vistas del sistema para el área Solicitudes y el widget Mis solicitudes en Inicio:

* **Todas las solicitudes**: todas las solicitudes que usted u otra persona hayan enviado en colas o espacios de trabajo para las que tiene permisos de visualización. Esto no está disponible para el widget Mis solicitudes.
* **Mis solicitudes**: Solicitudes que ha enviado, independientemente de su estado.
* **Mis solicitudes abiertas**: Solicitudes que ha enviado y que siguen abiertas.
* **Mis borradores**: Borradores de tus misiones que aún no se han enviado.
* **Solicitudes abiertas**: Solicitudes que usted o cualquier otra persona ha enviado en colas o para espacios de trabajo para los que tiene permisos de visualización que aún están abiertos. Esto no está disponible para el widget Mis solicitudes.

No puede editar las vistas del sistema. Puede modificar sus elementos y, a continuación, copiar la vista y editar o compartir la copia.

## Creación de una vista para solicitudes

Puede crear una vista en el área de Solicitudes de Workfront al utilizar la nueva experiencia de solicitudes. Después de habilitar y crear una experiencia de solicitudes nueva, también puede crear vistas para el widget Mis solicitudes en Inicio.

1. Para acceder a la lista **Solicitudes**:

   {{step1-to-requests}}

   1. Asegúrese de que la opción **Usar nueva experiencia** esté activada.

1. Para acceder al widget **Mis solicitudes** de inicio:

   {{step1-to-home}}

   1. Agregar o ir al widget **Mis solicitudes**.

1. En la lista de solicitudes, haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y luego haga clic en **Nueva vista**.

   <!-- 
   
   replace the screen shot with release
   ![New view](assets/create-new-view.png)

   -->

1. Escriba un nombre para la nueva vista y haga clic en **Crear**.
1. Continuar a [Editar una vista para solicitudes](#edit-a-view-for-requests).

## Edición de una vista para solicitudes

Puede editar las vistas existentes, incluidas las que acaba de crear en el área de Solicitudes o el widget Mis solicitudes en Inicio.

Al editar una vista, puede cambiar los siguientes elementos de la vista:

* Nombre
* Filtros
* Columnas
* Agrupación
* Formatear celdas
* Altura de la fila

Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Los cambios en las vistas se guardan automáticamente.
> * Cualquier persona que utilice la vista sólo podrá ver los cambios realizados en las vistas cuando comparta una copia nueva de la vista después de realizar cambios en ella.
> * Use el comodín de filtro **Me (usuario conectado)** en cualquier campo que tenga como valor usuarios.

## Añadir la vista de solicitudes a una plantilla de diseño

Un administrador de Workfront puede agregar una nueva vista a las plantillas de diseño para el área de Solicitudes.

Para obtener instrucciones, vea [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Compartir una vista

Puede compartir vistas que cree con otros usuarios, equipos, grupos o empresas.

Después de compartir una vista, otros usuarios pueden ver los elementos de vista actualizados que editó para la vista antes de compartirla.

Si actualizan la vista, sus cambios no serán visibles para otros, a menos que realicen una copia de la misma vista y conserven sus cambios antes de compartir la copia.

Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->