---
product-area: projects
navigation-topic: use-the-home-area
title: Uso del widget Mis solicitudes
description: Puede enviar solicitudes en el widget Mis solicitudes. También puede personalizar el widget con filtros y columnas.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
last-update: 2026-04-01T18:23:03.000Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
TQID: https://experienceleague.adobe.com/CmlT3NwdCWm-UiIiN5mxGgEVFVLjtqOY97ATuTgaN4g
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 674
ht-degree: 11%

---

# Uso del widget Mis solicitudes

<!--
remove Preview and Production references at Production release April 15, 2026

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>Este artículo describe el nuevo widget Mis solicitudes. Debe tener la nueva experiencia de solicitud habilitada para ver el nuevo widget.
>Puede habilitar la nueva experiencia de solicitud en el área de solicitudes.

El widget Mis solicitudes muestra las solicitudes que ha enviado. Puede filtrar las solicitudes, buscar solicitudes específicas o ajustar el orden y la visibilidad de las columnas. También puede crear una nueva solicitud desde el widget Mis solicitudes.

>[!NOTE]
>
>* Cuando se carga el widget Mis solicitudes, muestra hasta 50 solicitudes. Para mostrar más solicitudes, desplácese hacia abajo por la lista.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Cualquier paquete de flujo de trabajo o Workfront</p>
   <p>Cualquier paquete de Workfront Planning para acceder a las solicitudes de Workfront Planning y a sus objetos creados</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Configuración de nivel de acceso</strong></td> 
   <td> <p>Acceso superior o de visualización a cualquier objeto para el que esté etiquetado en una conversación o que necesite resolver una aprobación (proyectos, tareas, problemas, documentos)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de [!UICONTROL View] o superiores para proyectos, tareas, problemas o documentos en los que esté etiquetado en una conversación o necesite resolver una aprobación</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una solicitud

Puede crear una solicitud directamente desde el widget Mis solicitudes.

Para obtener instrucciones, vea la sección [Crear una solicitud](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) en el artículo [Crear elementos de trabajo y proyectos desde el área de inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Copiar una solicitud

Puede copiar una solicitud en el widget Mis solicitudes, editarla y enviarla como una solicitud nueva.

Para obtener instrucciones, consulte [Copiar y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Administrar información en la lista de solicitudes en el widget Mis solicitudes

<!--
This is similar to what we document in Enhanced lists, so we will link to that to avoid documentation duplication:
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haz clic en **Personalizar**, busca **Mis solicitudes** y luego haz clic en él para agregarlo a **Inicio**.
1. (Opcional) Para administrar la forma en que se muestra la información en la lista de solicitudes, cree o actualice los siguientes elementos de vista para la lista:

   * Ver
   * Filtro
   * Columnas
   * Agrupación
   * Formatear celdas
   * Altura de la fila

   Para obtener más información sobre cómo actualizar elementos de vista en la lista de solicitudes, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


<!--
 Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.
The filter is saved automatically.
-->

>[!TIP]
>
>Si su organización ha adquirido Workfront Planning además de Adobe Workfront, el widget Mis solicitudes incluirá tanto las solicitudes de Workfront como las de Workfront Planning.
> 
>* Para filtrar solo las solicitudes Workfront, establezca el filtro en **Tipo de objeto** > **Tiene cualquiera de** > **Problemas**.
>* Para filtrar solo las solicitudes de Workfront Planning, establezca el filtro en **Tipo de objeto** > **No tiene ninguno de** > **Problemas**.

<!--

Use enhanced lists and other requests articles describe all of these:

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## Solicitudes de búsqueda

Para buscar solicitudes específicas en el widget Mis solicitudes:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haz clic en **Personalizar**, busca **Mis solicitudes** y luego haz clic en él para agregarlo a **Inicio**.
1. En la barra de búsqueda cerca de la parte superior derecha del widget Mis solicitudes, introduzca el término que desea buscar.

   Las solicitudes que contienen el término se resaltan en naranja.

1. (Opcional) Para saltar a las solicitudes resaltadas, haga clic en las flechas arriba o abajo de la barra de búsqueda.

## Ir a un objeto creado por una solicitud

Puede encontrar objetos creados por una solicitud en el widget Mis solicitudes.

>[!NOTE]
>
>Los siguientes objetos tienen vínculos de la lista de solicitudes en el widget Mis solicitudes, cuando se habilita la nueva experiencia de solicitudes en el área Solicitudes:
>
>* Solicitudes de Planning y Workfront en el campo Asunto.
>* Registros de Planning creados a partir de solicitudes de Planning en el campo Objeto creado.
>* Las tareas y problemas de Workfront se convirtieron desde solicitudes de Workfront en el campo Objeto creado.

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/lines-main-menu.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haz clic en **Personalizar**, busca **Mis solicitudes** y luego haz clic en él para agregarlo a **Inicio**.
1. Busque la solicitud que creó el objeto.
1. Haga clic en el nombre de objeto en la columna **Objeto creado** para esa solicitud.

   Se abre la página del objeto.

   >[!TIP]
   >
   >Las tareas y proyectos de Workfront convertidos de problemas, así como los registros de Planning creados a partir de solicitudes de Planning, tienen un vínculo en el campo **Objeto creado**.



