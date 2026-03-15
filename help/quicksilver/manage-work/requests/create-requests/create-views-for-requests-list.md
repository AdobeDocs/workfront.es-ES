---
product-area: requests
navigation-topic: create-requests
title: Creación y administración de vistas en el área de solicitudes
description: Si utiliza la nueva experiencia de solicitud, puede crear y guardar vistas para el área de solicitudes.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: 78ad910e8d121dda38c9a7da27b0b338e0e1dcda
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 7%

---


# Creación y administración de vistas en el área de solicitudes

<span class="preview">La información de esta página se refiere a una funcionalidad que no está disponible de forma general. Solo está disponible en el entorno de previsualización para todos los clientes. Después de los lanzamientos mensuales a Production, las mismas funciones también están disponibles en el entorno de Production para los clientes que habilitaron los lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Si utiliza la nueva experiencia de solicitud en Adobe Workfront, puede crear y guardar vistas para el área de solicitudes. Estas vistas incluyen filtros y disposiciones de columnas.

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* Esta funcionalidad solo está disponible en la nueva experiencia de solicitud del área de solicitudes.
>* La configuración de vista también está disponible en el widget Mis solicitudes de Inicio. Sin embargo, las vistas del área de Solicitudes son independientes de las del widget Mis solicitudes.
>* La lista de solicitudes del área Solicitudes utiliza la lista mejorada en Workfront. Para obtener más información, vea [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete Workfront o Workflow</p>

<p>Cualquier licencia de Workfront Planning, para ver las solicitudes de Workfront Planning en listas de solicitudes</p>
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

## Creación de una vista para solicitudes

Puede crear una vista en el área Solicitudes de Workfront al utilizar la nueva experiencia de solicitudes.

1. Para acceder a la lista de solicitudes:

   {{step1-to-requests}}

1. Asegúrese de que la opción **Usar nueva experiencia** esté activada.

1. En la lista **Solicitudes**, haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y luego haga clic en **Nueva vista**.

   ![Nueva vista](assets/create-new-view.png)

1. Escriba un nombre para la nueva vista y haga clic en **Crear**.
1. Continuar a [Editar una vista en el área de solicitudes](#edit-a-view-in-the-requests-area).

## Edición de una vista para solicitudes

Puede editar las vistas existentes, incluidas las que acaba de crear en el área Solicitudes de Workfront.

Al editar una vista en el área Solicitudes, puede cambiar los siguientes elementos de la vista:

* Nombre
* Filtros
* Columnas

Los cambios que realice en una vista serán visibles para todos los usuarios con los que comparta la vista.

1. Para acceder a una lista de solicitudes en el apartado Solicitudes:

   {{step1-to-requests}}

1. Asegúrese de que la opción **Usar nueva experiencia** esté activada.
1. En la lista **Solicitudes**, busque la vista que desea editar en el menú desplegable **Vistas** ![Lista desplegable Vistas](assets/view-icon-requests.png).

1. Haga clic en la lista desplegable **Views** ![Views](assets/view-icon-requests.png) y haga clic en el menú de tres puntos situado junto a la vista, seleccione **Renombrar** y, a continuación, escriba el nuevo nombre de la vista.
1. Presione Intro para guardar el nuevo nombre.
1. Haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y seleccione la vista que desee editar.
1. Para agregar un campo como columna, haga clic en el icono **Agregar columna** ![Agregar columna](assets/add-column.png) situado en la esquina superior derecha de la lista.

   Se abre el **Administrador de columnas**.
1. Haga clic en el icono más situado junto al campo que desee agregar como columna a la vista y, a continuación, haga clic en **Guardar**.

   Los campos asociados a los objetos de la lista están disponibles para agregarlos como columnas. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >Los campos que agregue a las columnas deben existir antes de que estén disponibles en el **Administrador de columnas**.


1. (Opcional) Haga clic en **Columnas** para abrir el cuadro F **Proporciona visibilidad y orden**.
1. Active la configuración de cada campo que desee mostrar en la lista, apáguelo para ocultarlo o arrastre y suelte los campos en un orden diferente.

1. (Opcional) Haga clic en **Filtros** y comience a agregar condiciones para las solicitudes que desee ver.

   Puede filtrar por los siguientes campos de solicitud:

   * **Workspace**: espacio de trabajo con el que está asociado el formulario de solicitud.
   * **Tipo de objeto**: tipo de registro al que está asociado el formulario de solicitud.
   * **Fecha de entrada**: La fecha en que se envió la solicitud.
   * **Formulario de solicitud**: nombre del formulario de solicitud utilizado para enviar la solicitud.
   * **Estado**: el estado de la solicitud.
   * **Escrito por**: el nombre del usuario que agregó la solicitud. Si alguien fuera de Workfront agregó la solicitud, el campo **Entered by** muestra `N/A`.

   También puede filtrar por cualquier campo que se haya añadido a la vista para cualquier objeto visible en la vista.

   Puede tener varios filtros unidos por **And** o **Or**.
La lista de solicitudes se filtra automáticamente a medida que se añaden las condiciones de filtro.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Los cambios en las vistas se guardan automáticamente.
> * Los cambios realizados en las vistas los podrá ver cualquier usuario que utilice la vista.
> * Use el comodín de filtro **Yo (usuario que inició sesión)** en cualquier campo que tenga como valor usuarios.

## Agregue la vista Solicitudes a una plantilla de diseño.

Un administrador de Workfront puede agregar la nueva vista a las plantillas de diseño.

Para obtener instrucciones, vea [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Compartir una vista

Puede compartir vistas que cree con otros usuarios, equipos o grupos.

1. Para tener acceso a una lista de solicitudes en las siguientes:

   {{step1-to-requests}}

1. Asegúrese de que está activada la opción **Usar nueva experiencia**.
1. En la lista **Solicitudes**, busque la vista que desea compartir.
1. Pase por encima de la vista que desee compartir y, a continuación, haga clic en el menú de tres puntos situado a la derecha del nombre de vista y, a continuación, haga clic en **Compartir**.
1. En el cuadro **Compartir**, escriba las personas, equipos, roles, grupos o empresas con las que desee compartir la vista y, a continuación, selecciónelas de la lista cuando aparezcan.
1. Haga clic en **Guardar**.

   La vista se comparte con las entidades que indique. Pueden ver los elementos de vista actualizados que editó para la vista antes de compartirla. <span class="preview">Si actualizan la vista, sus cambios no serán visibles para los demás, a menos que realicen una copia de la misma vista y conserven sus cambios antes de compartir la copia. Para obtener más información, vea [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
