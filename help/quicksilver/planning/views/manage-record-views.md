---
title: Administrar vistas de registros
description: Puede mostrar registros en una vista de tabla, escala de tiempo o calendario al utilizar Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '1113'
ht-degree: 1%

---

# Administrar vistas de registros

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede mostrar todos los registros de ese tipo en las siguientes vistas:

* Tabla

  Para obtener más información, vea [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

* Cronología

  Para obtener más información, vea [Administrar la vista de escala de tiempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Calendario

  Para obtener más información, consulte [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md).

Este artículo describe la siguiente información sobre las vistas de registros:

* [Crear y editar una vista](#create-or-edit-record-views)
* [Eliminación de una vista](#delete-views)
* [Duplicar una vista](#duplicate-views)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<!--at GA the plan below will change to Prime, Select and Ultimate only-->

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p>
   O
   <p>Actual: plan </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> No hay controles de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en una vista</p>  
   <p>Ver permisos de una vista para cambiar temporalmente su configuración</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> <p>Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Consideraciones al trabajar con vistas de registros

* Las vistas de Workfront Planning son específicas del tipo de registro. No se puede aplicar la misma vista a dos tipos de registro diferentes.
* Las vistas que cree solo serán visibles para usted y para los usuarios con los que comparta las vistas.
* Al modificar o eliminar una vista, esta se modifica y elimina para todos los usuarios que tienen permisos de acceso a la vista.
* Cada usuario puede crear un máximo de 100 vistas. Puede mostrar más de 100 vistas para un tipo de registro, pero un usuario solo puede crear 100 vistas.
* Puede compartir vistas que cree con otros usuarios. Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).
* Los siguientes elementos son exclusivos de cada vista de registro:

   * Filtro
   * Agrupación
   * Ordenar
   * Apariencia de la barra (para la vista de la cronología)

  <!-- some of these are not available in all of the views - edit above-->

  Por ejemplo, al crear un filtro en una vista de tabla, los resultados del filtro solo son visibles en la vista seleccionada y no en todas las vistas asociadas al tipo de registro.

  >[!NOTE]
  >
  > Es posible que algunos elementos de vista no estén disponibles para todas las vistas.


## Similitudes y diferencias entre vistas de registros

En la tabla siguiente se muestran las similitudes y diferencias entre las vistas de tabla, escala de tiempo y calendario:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Función | Vista de tabla | Vista Cronología | Vista de calendario |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Mostrar registros en una lista o tabla | ✓ |              | |
| Mostrar todos los campos como columnas en la tabla de forma predeterminada | ✓ |              |    |
| Ocultar o mostrar campos (o columnas) | ✓ |               |    |
| Editar valores de campo para cada registro | ✓ |               |             |
| Agregar registros como filas nuevas en la vista | ✓ |               |        |
| Agregar campos como nuevas columnas en la vista | ✓ |               |         |
| Copiar filas de una lista externa y pegarlas en una tabla | ✓ |               |          |
| Mostrar registros en una cronología |            | ✓ |             |
| Filtrar registros | ✓ | ✓ | ✓ |
| Mostrar registros en un calendario |           |              | ✓ |
| Agrupar registros | ✓ | ✓ |
| Ordenar registros | ✓ |              |
| Registros de código de color |           | ✓ | ✓ |
| Agrupaciones de código de color |           | ✓ |
| Buscar registros específicos | ✓ | ✓ |
| Compartir vista | ✓ | ✓ | ✓ |
| Abra la página del registro desde la vista | ✓ | ✓ |    |


## Creación o edición de vistas {#create-or-edit-views}

{{step1-to-planning}}


1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Haga clic en **+ Vista** para agregar una vista nueva.
1. Seleccione entre los siguientes tipos de vistas:

   * Tabla
   * Cronología
   * Calendario

   Se crea una nueva pestaña con la vista seleccionada.

   Según el ancho de la pantalla, es posible que se muestren vistas adicionales en el menú **Más** ![](assets/more-menu.png).


>[!TIP]
>
>Al crear un tipo de registro, la vista de tabla también se crea de forma predeterminada.
>
>Para crear una escala de tiempo o una vista de calendario, el tipo de registro para el que genere la vista debe tener al menos dos campos de fecha.
>
>De lo contrario, las opciones Cronología y Calendario aparecen atenuadas.
>

![](assets/view-types-drop-down-from-record-type-list.png)

1. (Condicional) Haga clic en **Siguiente** al crear una vista de calendario o de cronología.

   De forma predeterminada, Workfront asigna a la vista uno de los nombres siguientes:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   El número es un incremento generado automáticamente.

1. (Condicional) Seleccione las **fechas de inicio** y de finalización **3} para los registros que se mostrarán en la vista de calendario o de cronología.**

   >[!TIP]
   >
   >    Puede seleccionar entre los campos de fecha de registro o los campos de fecha de búsqueda de los tipos de objeto o registro conectado. Debe utilizar acumuladores para los campos de fecha (MAX o MIN) cuando seleccione los campos de búsqueda como fechas de inicio y finalización para las vistas de calendario y de escala de tiempo. Para obtener más información, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Haga clic en **Crear**.

   La vista se muestra como una nueva pestaña. Las vistas se muestran en orden cronológico a partir del momento en que se crearon o compartieron con usted.
1. (Opcional) Haga clic en el menú **Más** ![](assets/more-caret-down-icon-views.png) que está junto a la última vista para mostrar todas las vistas del tipo de registro seleccionado.

   Se muestran vistas adicionales en el menú **Más** después de la última ficha de vista. El número al lado del menú **Más** muestra el número de vistas adicionales.
1. (Opcional) Para cambiar el nombre de una vista una vez creada, haga clic en el menú desplegable de vista y, a continuación, haga clic en el menú **Más** ![](assets/more-menu.png) > **Cambiar nombre** para actualizar el nombre de la vista

   O

   Haga doble clic en el nombre de la vista y empiece a escribir el nuevo nombre.  <!--ensure there is not another saving step here?!-->

1. (Opcional) Para administrar un tipo de vista específico, consulte los siguientes artículos:

   * [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Administrar la vista de cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Administrar la vista de calendario](/help/quicksilver/planning/views/manage-the-calendar-view.md)


## Eliminar vistas

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Pase el ratón sobre uno de los nombres de la vista en la pestaña de la vista, luego haga clic en **Más** ![](assets/more-menu.png) a la izquierda del nombre de la vista y luego haga clic en **Eliminar**.
En primer lugar, es posible que deba hacer clic en **Más** a la izquierda de la última pestaña para encontrar la vista que desee eliminar.

1. Haga clic en **Eliminar** para confirmar. <!--ensure there is not another saving step here?!-->

   La vista se elimina para todos los usuarios que pueden acceder al área de registros y no se puede recuperar.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Duplicación de una vista

Si desea conservar varias versiones de una vista y realizar ligeros cambios entre ellas, puede duplicar una vista.

Al duplicar una vista, se crean copias idénticas de una vista existente.

Los permisos de uso compartido de la vista original no se transfieren a la vista duplicada.

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Pase el ratón sobre la pestaña de la vista que quiera duplicar, haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre de la vista y luego haga clic en **Duplicar**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   La vista está duplicada y el nombre de la nueva vista sigue el siguiente patrón: `Original view's name (Copy)`. La nueva pestaña de vista se muestra al final de todas las pestañas de vista.

