---
product-area: requests
navigation-topic: create-requests
title: Creación y administración de vistas en el área de solicitudes
description: Si utiliza la nueva experiencia de solicitud, puede crear y guardar vistas para el área de solicitudes.
author: Becky
feature: Work Management
source-git-commit: d8e5e6d313eb39c9ac26e7cb60113beac5637890
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 7%

---

# Creación y administración de vistas en el área de solicitudes

Si utiliza la nueva experiencia de solicitud, puede crear y guardar vistas para el área de solicitudes. Estas vistas incluyen filtros y disposiciones de columnas.

Las vistas se pueden crear y administrar en el área de solicitudes de Workfront.

>[!IMPORTANT]
>
>* Esta funcionalidad solo está disponible en la nueva experiencia de solicitud.
>* La configuración de vista no está disponible en el widget Mis solicitudes de Inicio.

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

## Creación de una vista en el área de Solicitudes

Puede crear una vista en el área de Solicitudes de Workfront,.

1. Para acceder a la lista de solicitudes:

   {{step1-to-requests}}

1. En la lista Solicitudes, haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y seleccione **Nueva vista**.

   ![Nueva vista](assets/create-new-view.png)

1. Escriba un nombre para la nueva vista y haga clic en **Crear**.
1. Continuar a [Editar una vista en el área de solicitudes](#edit-a-view-in-the-requests-area).

## Edición de una vista en el área de Solicitudes

Puede editar las vistas existentes, incluidas las que acaba de crear.

1. Para acceder a la lista de solicitudes:

   {{step1-to-requests}}
1. En la lista Solicitudes, busque la vista que desee editar.

1. (Opcional) Para cambiar el nombre de una vista, haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y haga clic en el menú de tres puntos situado junto a la vista, seleccione **Cambiar nombre** y, a continuación, escriba el nuevo nombre de la vista.
1. Haga clic en el menú desplegable **Vistas** ![Menú desplegable de vistas](assets/view-icon-requests.png) y seleccione la vista que desee editar.
1. Para agregar un campo personalizado como columna, haga clic en el icono **Agregar columna** ![Agregar columna](assets/add-column.png) cerca de la derecha de la pantalla y haga clic en el icono de signo más situado junto al campo de formulario personalizado que desea agregar como columna a la vista.

   >Los campos personalizados de los formularios adjuntos al objeto en la lista están disponibles para agregarlos como columnas.

   >[!TIP]
   >
   >Actualmente, no se pueden agregar columnas en el entorno de producción.
1. (Opcional) Haga clic en **Columnas** y oculte, muestre o reorganice las columnas en la lista de solicitudes.

   ![Cuadro de columnas](assets/columns-editing-box-in-requests-planning-tab.png)

   >[!TIP]
   >
   >Actualmente no se pueden agregar más columnas en el entorno de producción.

1. (Opcional) Haga clic en **Filtros** y empiece a agregar condiciones para las solicitudes que desee ver en la pestaña Planificación.

   ![Edición de filtros en la ficha de solicitudes de Planning](assets/filters-editing-box-in-requests-planning-tab.png)

   Puede filtrar por los siguientes campos:

   * **Workspace**: área de trabajo con la que está asociado el formulario de solicitud.
   * **Tipo de registro**: Tipo de registro al que está asociado el formulario de solicitud.
   * **Fecha de entrada**: La fecha en la que se envió la solicitud.
   * **Formulario de solicitud**: Nombre del formulario de solicitud utilizado para enviar la solicitud.
   * **Estado**: El estado de la solicitud.
   * **Ingresado por**: nombre del usuario que agregó la solicitud. Si alguien fuera de Workfront agregó la solicitud, el campo **Ingresado por** muestra `N/A`.

   También puede filtrar por cualquier campo personalizado que se haya agregado a la vista.

   Puede tener varios filtros unidos por **And** o **Or**.
La lista de solicitudes se filtra automáticamente a medida que se añaden las condiciones de filtro.



>[!IMPORTANT]
>
> * Los cambios en las vistas se guardan automáticamente.
> * Cualquier persona que utilice la vista podrá ver los cambios realizados en las vistas.
> * Para asegurarse de que la vista se aplique a la persona que está utilizando la vista, independientemente de quién la haya creado, puede utilizar el comodín de filtro &quot;Yo (usuario que ha iniciado sesión)&quot; en cualquier campo que tenga como valor usuarios.

## Añada la vista a una plantilla de diseño.

Un administrador de Workfront puede agregar la nueva vista a las plantillas de diseño.

Para obtener instrucciones, vea [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Compartir una vista

Puede compartir vistas que cree con otros usuarios, equipos o grupos.

1. Para acceder a la lista de solicitudes:

   {{step1-to-requests}}

1. En la lista Solicitudes, busque la vista que desee compartir.
1. Pase el ratón sobre la vista que quiera compartir y luego haga clic en el menú de tres puntos cuando aparezca.
1. Seleccione **Compartir**.
1. En el cuadro de diálogo que se abre, escriba los nombres de los usuarios, equipos o grupos con los que desea compartir la vista y, a continuación, selecciónelos en la lista cuando aparezcan.
1. Haga clic en **Guardar**.

