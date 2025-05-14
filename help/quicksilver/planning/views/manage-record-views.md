---
title: Administrar vistas de registros
description: Puede mostrar registros en una vista de tabla, escala de tiempo o calendario al utilizar Adobe Workfront Planning. Este artículo describe cómo crear una vista y editar una existente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: a215cf721cc4d517ee39cfa864e29dbbbfeb0a31
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 57%

---


# Administrar vistas de registros

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede mostrar todos los registros de ese tipo en las siguientes vistas:

* Tabla

  Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

* Cronología

  Para obtener más información, consulte [Administrar la vista de línea de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Calendario

  Para obtener más información, consulte [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

En este artículo se describe la siguiente información sobre las vistas de registros:

* [Crear y editar una vista](#create-or-edit-record-views)
* [Habilitar los indicadores de presencia en tiempo real en una vista](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Para obtener más información sobre la administración de vistas de registros de Workfront Planning, consulte también los siguientes artículos:

* [Eliminar vistas de registros](/help/quicksilver/planning/views/delete-record-views.md)
* [Duplicar vistas de registros](/help/quicksilver/planning/views/duplicate-record-views.md)
* [Compartir vistas](/help/quicksilver/planning/access/share-views.md)


## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar </p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración de una vista</p>  
   <p>Ver permisos en una vista para cambiar temporalmente la configuración de la vista o para duplicarla</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>En el entorno de producción, todos los usuarios, incluidos los administradores del sistema, deben estar asignados a una plantilla de diseño que incluya Planning.</p>
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen Planning habilitado de forma predeterminada.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al trabajar con vistas de registros

* Las vistas de Workfront Planning son específicas del tipo de registro. No puede aplicar la misma vista a dos tipos de registro diferentes.
* Las vistas que cree solo serán visibles para usted y para los usuarios con los que comparta las vistas.
* Al modificar o eliminar una vista, esta se modifica y elimina para todos los usuarios que tengan permisos de acceso sobre ella.
* Cada usuario puede crear un máximo de 100 vistas. Puede mostrar más de 100 vistas para un tipo de registro, pero un usuario solo puede crear 100 vistas.
* Aunque algunos elementos de vista se pueden aplicar a varias vistas del mismo registro, son únicos en cada vista de registro:

   * Filtro
   * Agrupación (para las vistas Tabla y Cronología)
   * Apariencia de la barra (para las vistas de calendario y cronología)

  Por ejemplo, al crear un filtro en una vista de tabla, los resultados del filtro sólo son visibles en la vista seleccionada (la vista de tabla) y no en todas las vistas asociadas al tipo de registro.

  >[!TIP]
  >
  >Algunos elementos de vista no estarán disponibles para todas las vistas.


## Similitudes y diferencias entre vistas de registros

En la tabla siguiente se muestran las similitudes y diferencias entre las vistas de tabla, línea de tiempo y calendario:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Función | Vista de tabla | Vista de línea de tiempo | Vista de calendario |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Mostrar registros en una lista o tabla | ✓ |              | |
| Mostrar todos los campos como columnas en la tabla de forma predeterminada | ✓ |              |    |
| Ocultar o mostrar campos (o columnas) | ✓ |               |    |
| Editar valores de campo para cada registro | ✓ |               |             |
| Añadir registros como filas nuevas en la vista | ✓ |               |        |
| Añadir campos como nuevas columnas en la vista | ✓ |               |         |
| Copiar filas de una lista externa y pegarlas en una tabla | ✓ |               |          |
| Mostrar registros en una línea de tiempo |            | ✓ |             |
| Filtrar registros | ✓ | ✓ | ✓ |
| Mostrar registros en un calendario |           |              | ✓ |
| Registros de grupo | ✓ | ✓ |
| Ordenar registros | ✓ |              |
| <span class="preview">Registros de código de color</span> | <span class="preview">✓</span> | ✓ | ✓ |
| Agrupaciones de código de color |           | ✓ |
| Buscar registros específicos | ✓ | ✓ |
| Compartir la vista con otros usuarios | ✓ | ✓ | ✓ |
| Abra la página del registro desde la vista | ✓ | ✓ |    |
| Mostrar registros por año y trimestre |           | ✓ |    |
| Mostrar registros por mes |           | ✓ | ✓ |
| Mostrar registros por semana |           |               | ✓ |


## Crear o editar vistas {#create-or-edit-views}

{{step1-to-planning}}


1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Haga clic en **+ Vista** para añadir una vista nueva.
1. Seleccione entre los siguientes tipos de vistas:

   * Tabla
   * Cronología
   * Calendario

   Se crea una nueva ficha con la vista seleccionada.

   Según la anchura de la pantalla, es posible que se muestren vistas adicionales en el menú **Más** ![Menú más](assets/more-menu.png).


>[!TIP]
>
>Al crear un tipo de registro, la vista de tabla también se crea de forma predeterminada.
>
>Para crear una vista de línea de tiempo o de calendario, el tipo de registro para el que genere la vista debe tener al menos dos campos de fecha.
>
>De lo contrario, las opciones Línea de tiempo y Calendario aparecen atenuadas.
>

![Lista desplegable de tipos de vista de la lista de tipos de registro](assets/view-types-drop-down-from-record-type-list.png)

1. (Condicional) Haga clic en **Siguiente** al crear una vista de línea de tiempo o de calendario.

   De forma predeterminada, Workfront asigna a la vista uno de los nombres siguientes:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   El número es un incremento generado automáticamente.

1. (Condicional) Seleccione las **fechas de inicio** y **de finalización** para los registros que se mostrarán en la vista de línea de tiempo o de calendario.

   >[!TIP]
   >
   >    Puede seleccionar entre los campos de fecha de registro o los campos de fecha de búsqueda de los tipos de objeto o registro conectados. Debe utilizar agregadores para los campos de fecha (MAX o MIN) cuando seleccione los campos de búsqueda como las fechas de inicio y de finalización para las vistas de línea de tiempo y calendario. Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Haga clic en **Crear**.

   La vista se muestra como una nueva pestaña. Las vistas se muestran en orden cronológico a partir del momento en que se crearon o compartieron con el usuario.
1. (Opcional) Haga clic en el menú **Más** ![Más vistas del icono de acento circunflejo invertido](assets/more-caret-down-icon-views.png) junto a la última vista para mostrar todas las vistas del tipo de registro seleccionado.

   Se muestran vistas adicionales en el menú **Más** después de la última pestaña de vista. El número al lado del menú **Más** muestra el número de vistas adicionales.
1. (Opcional) Para cambiar el nombre de una vista una vez creada, haga clic en el menú desplegable de vista y, a continuación, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) > **Cambiar nombre** para actualizar el nombre de la vista

   O

   Haga doble clic en el nombre de la vista y empiece a escribir el nuevo nombre. <!--ensure there is not another saving step here?!-->

1. (Opcional) Para administrar un tipo de vista específico, consulte los siguientes artículos:

   * [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Administrar la vista de cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## Habilitar el indicador de presencia en tiempo real en una vista

Puede ver si otros usuarios están editando registros al mismo tiempo que usted siguiendo los indicadores de presencia en tiempo real de la vista.

De forma predeterminada, los avatares de otros usuarios que están editando información de registro al mismo tiempo que se muestran en la esquina superior derecha de todas las vistas de registros.

Al mostrar la vista de tabla, también puede ver qué campo está editando otro usuario en el momento en que está viendo el registro.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).



<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->
