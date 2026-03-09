---
product-area: requests
navigation-topic: create-requests
title: Creación y administración de vistas en el área de solicitudes
description: Si utiliza la nueva experiencia de solicitud, puede crear y guardar vistas para el área de solicitudes.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
source-git-commit: e4d57d0b5042dc4889d5b676396b56c05ab1515d
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 7%

---


# Creación y administración de vistas en el área de solicitudes

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>





Si utiliza la nueva experiencia de solicitud en Adobe Workfront, puede crear y guardar vistas para el área de solicitudes. Estas vistas incluyen filtros y disposiciones de columnas.

<!--<span class="preview"> and groupings.</span>-->


>[!IMPORTANT]
>
>* Esta funcionalidad solo está disponible en la nueva experiencia de solicitud del área de solicitudes.
>* La configuración de vista también está disponible en el widget Mis solicitudes de Inicio. Sin embargo, las vistas del área de Solicitudes son independientes de las del widget Mis solicitudes.
>* La lista de solicitudes del área de Solicitudes utiliza la lista mejorada de Workfront. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
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
  <tr> 
   <td role="rowheader"> Producto</td> 
   <td> <ul><li>Adobe Workfront</li><li>Debe tener Adobe Workfront Planning para ver solicitudes de Planning o formularios de solicitud</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una vista para solicitudes

Puede crear una vista en el área de Solicitudes de Workfront al utilizar la nueva experiencia de solicitudes.

1. Para acceder a la lista de solicitudes:

   {{step1-to-requests}}

1. Asegúrese de que la opción **Usar nueva experiencia** esté activada.

1. En la lista **Solicitudes**, haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y luego haga clic en **Nueva vista**.

   ![Nueva vista](assets/create-new-view.png)

1. Escriba un nombre para la nueva vista y haga clic en **Crear**.
1. Continuar a [Editar una vista en el área de solicitudes](#edit-a-view-in-the-requests-area).

## Edición de una vista para solicitudes

Puede editar las vistas existentes, incluidas las que acaba de crear en el área de Solicitudes de Workfront.

Al editar una vista en el área de Solicitudes, puede cambiar los siguientes elementos de la vista:

* Nombre
* Filtros
* Columnas

Los cambios realizados en una vista son visibles para todos los usuarios con los que comparte la vista.

1. Para acceder a una lista de solicitudes en las solicitudes, haga lo siguiente:

   {{step1-to-requests}}

1. Asegúrese de que la opción **Usar nueva experiencia** esté activada.
1. En la lista **Solicitudes**, busque la vista que desee editar en el menú desplegable **Vistas** ![Menú desplegable Vistas](assets/view-icon-requests.png).

1. Haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y haga clic en el menú de tres puntos situado junto a la vista, seleccione **Cambiar nombre** y, a continuación, escriba el nuevo nombre de la vista.
1. Pulse Intro para guardar el nuevo nombre.
1. Haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y seleccione la vista que desee editar.
1. Para agregar un campo como columna, haga clic en el icono **Agregar columna** ![Agregar columna](assets/add-column.png) en la esquina superior derecha de la lista.

   Se abre **Administrador de columnas**.
1. Haga clic en el icono de signo más situado junto al campo que desee agregar como columna a la vista y, a continuación, haga clic en **Guardar**.

   Los campos asociados con los objetos de la lista están disponibles para agregarlos como columnas. <!--keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future-->

   >[!TIP]
   >
   >Los campos que agregue a las columnas deben existir antes de que estén disponibles en el **Administrador de columnas**.


1. (Opcional) Haga clic en **Columnas** para abrir el cuadro F **Campos de visibilidad y orden**.
1. Active la configuración para cada campo que desee mostrar en la lista, desactívela para ocultarla o arrastre y suelte los campos en un orden diferente.

1. (Opcional) Haga clic en **Filtros** y empiece a agregar condiciones para las solicitudes que desee ver.

   Puede filtrar por los siguientes campos de solicitud:

   * **Workspace**: área de trabajo con la que está asociado el formulario de solicitud.
   * **Tipo de objeto**: Tipo de registro al que está asociado el formulario de solicitud.
   * **Fecha de entrada**: La fecha en la que se envió la solicitud.
   * **Formulario de solicitud**: Nombre del formulario de solicitud utilizado para enviar la solicitud.
   * **Estado**: El estado de la solicitud.
   * **Ingresado por**: nombre del usuario que agregó la solicitud. Si alguien fuera de Workfront agregó la solicitud, el campo **Ingresado por** muestra `N/A`.

   También puede filtrar por cualquier campo que se haya añadido a la vista para cualquier objeto visible en la vista.

   Puede tener varios filtros unidos por **And** o **Or**.
La lista de solicitudes se filtra automáticamente a medida que se añaden las condiciones de filtro.


<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Los cambios en las vistas se guardan automáticamente.
> * Cualquier persona que utilice la vista podrá ver los cambios realizados en las vistas.
> * Use el comodín de filtro **Me (usuario conectado)** en cualquier campo que tenga como valor usuarios.

## Agregue la vista Solicitudes a una plantilla de diseño.

Un administrador de Workfront puede agregar la nueva vista a las plantillas de diseño.

Para obtener instrucciones, vea [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Compartir una vista

Puede compartir vistas que cree con otros usuarios, equipos o grupos.

1. Para acceder a una lista de solicitudes en las solicitudes, haga lo siguiente:

   {{step1-to-requests}}

1. Asegúrese de que la opción **Usar nueva experiencia** esté activada.
1. En la lista **Solicitudes**, busque la vista que desee compartir.
1. Pase el ratón sobre la vista que quiera compartir, luego haga clic en el menú de tres puntos a la derecha del nombre de la vista y luego haga clic en **Compartir**.
1. En el cuadro **Compartir**, escriba las personas, los equipos, las funciones, los grupos o las empresas con los que desea compartir la vista y, a continuación, selecciónelos en la lista cuando aparezcan.
1. Haga clic en **Guardar**.

   La vista se comparte con las entidades que indique. Pueden ver los elementos de vista actualizados que editó para la vista antes de compartirla. <span class="preview">Si actualizan la vista, sus cambios no serán visibles para otros, a menos que realicen una copia de la misma vista y conserven sus cambios antes de compartir la copia. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
