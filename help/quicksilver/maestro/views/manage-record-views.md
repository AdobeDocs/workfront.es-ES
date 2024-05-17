---
title: Administrar vistas de registros
description: Puede mostrar registros en una vista de tabla, escala de tiempo o calendario al utilizar Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 34b1bf4e776a1f5b4a413ab9f78bed63c4b64f45
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 1%

---

# Administrar vistas de registros

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede mostrar todos los registros de ese tipo en las siguientes vistas:

* Tabla

  Para obtener más información, consulte [Administrar la vista de tabla](../views/manage-the-table-view.md).

* Cronología

  Para obtener más información, consulte [Administrar la vista de cronología](../views/manage-the-timeline-view.md).

* Calendario

  Para obtener más información, consulte [Administrar la vista de calendario](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

Este artículo describe la siguiente información sobre las vistas de registros:

* [Creación y edición de una vista](#create-or-edit-record-views)
* [Eliminación de una vista](#delete-views)
* [Duplicación de una vista](#duplicate-views)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## Requisitos de acceso

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta cerrado de Adobe Workfront Planning. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <p>Cualquiera</p> 
   <p>Los administradores del sistema solo tienen acceso a las vistas que han creado o que se han compartido con ellos. </p>
  </td>
  </tr>

<tr>
   <td role="rowheader">Configuración del nivel de acceso</td>
   <td> <p>No hay controles de nivel de acceso para Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos de la vista</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Plantilla de diseño</td>
   <td> <p>El administrador del sistema debe añadir el área de planificación a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Consideraciones al trabajar con vistas de registros

* Las vistas de Workfront Planning son específicas del tipo de registro. No se puede aplicar la misma vista a dos tipos de registro diferentes.
* Las vistas que cree solo serán visibles para usted y para los usuarios con los que comparta las vistas.
* Al modificar o eliminar una vista, esta se modifica y elimina para todos los usuarios que tienen permisos de acceso a la vista.
* Cada usuario puede crear un máximo de 100 vistas. Puede mostrar más de 100 vistas para un tipo de registro, pero un usuario solo puede crear 100 vistas.
* Puede compartir vistas que cree con otros usuarios. Para obtener más información, consulte [Compartir vistas](/help/quicksilver/maestro/access/share-views.md).
* Los siguientes elementos son exclusivos de cada vista de registro:

   * Filtro
   * Agrupación
   * Ordenar
   * Apariencia de la barra (para la vista de la cronología)

  <!-- some of these are not available in all of the views - edit above-->

  Por ejemplo, al crear un filtro en una vista de tabla, los resultados del filtro solo son visibles en la vista seleccionada y no en todas las vistas asociadas al tipo de registro.

  >[!NOTE]
  >
  > Debido a que Adobe Workfront Planning se encuentra actualmente en estado beta, es posible que algunos elementos de vista no estén disponibles para todas las vistas.

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

{{step1-to-maestro}}


El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada. Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).

1. Haga clic en una tarjeta de tipo de registro. Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Clic **+ Ver** para añadir una nueva vista.
1. Seleccione entre los siguientes tipos de vistas:

   * Tabla
   * Cronología
   * Calendario

   Se crea una nueva pestaña con la vista seleccionada.

   Según el ancho de la pantalla, podrían mostrarse vistas adicionales en la **Más** menú ![](assets/more-menu.png).


>[!TIP]
>
>Al crear un tipo de registro, la vista de tabla también se crea de forma predeterminada.
>
>Para crear una escala de tiempo o una vista de calendario, el tipo de registro para el que genere la vista debe tener al menos dos campos de fecha. De lo contrario, las opciones Cronología y Calendario aparecen atenuadas.
>

![](assets/view-types-drop-down-from-record-type-list.png)

>[!NOTE]
>
>    Para crear una escala de tiempo o una vista de calendario, el tipo de registro para el que genere la vista debe tener al menos dos campos de fecha. De lo contrario, las opciones Cronología o Calendario aparecen atenuadas.

1. (Condicional) Haga clic en **Siguiente**, al crear una vista de calendario o de cronología.

   De forma predeterminada, Workfront asigna a la vista uno de los nombres siguientes:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   El número es un incremento generado automáticamente.

1. (Condicional) Seleccione la variable **Inicio** y **Fechas de finalización** para los registros que se mostrarán en la vista cronología o calendario.
1. Haga clic en **Crear**.

   La vista se muestra como una nueva pestaña. Las vistas se muestran en orden cronológico a partir del momento en que se crearon o compartieron con usted.
1. (Opcional) Haga clic en **Más** menú ![](assets/more-caret-down-icon-views.png) situado junto a la última vista para mostrar todas las vistas del tipo de registro seleccionado.

   Las vistas adicionales se muestran en **Más** después de la última pestaña de vista. El número situado junto al **Más** El menú muestra el número de vistas adicionales.
1. (Opcional) Para cambiar el nombre de una vista una vez creada, haga clic en el menú desplegable de vista y, a continuación, haga clic en **Más** menú ![](assets/more-menu.png) > **Cambiar nombre** para actualizar el nombre de la vista

   O

   Haga doble clic en el nombre de la vista y empiece a escribir el nuevo nombre.  <!--ensure there is not another saving step here?!-->

1. (Opcional) Para administrar un tipo de vista específico, consulte los siguientes artículos:

   * [Administrar la vista de tabla](../views/manage-the-table-view.md)
   * [Administrar la vista de cronología](../views/manage-the-timeline-view.md)
   * [Administrar la vista de calendario](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## Eliminar vistas

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada. Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).

1. Haga clic en una tarjeta de tipo de registro.

   Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Pase el ratón sobre uno de los nombres de la vista en la pestaña de vista y haga clic en **Más** ![](assets/more-menu.png) a la izquierda del nombre de la vista y haga clic en **Eliminar**.
Primero, es posible que tenga que hacer clic en **Más** a la izquierda de la última pestaña para buscar la vista que desea eliminar.

1. Clic **Eliminar** para confirmar. <!--ensure there is not another saving step here?!-->

   La vista se elimina para todos los usuarios que pueden acceder al área de registros y no se puede recuperar.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Duplicación de una vista

Si desea conservar varias versiones de una vista y realizar ligeros cambios entre ellas, puede duplicar una vista.

Al duplicar una vista, se crean copias idénticas de una vista existente.

Los permisos de uso compartido de la vista original no se transfieren a la vista duplicada.

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada.

Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).

1. Haga clic en una tarjeta de tipo de registro. Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Pase el ratón sobre la pestaña de la vista que quiera duplicar y haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre de la vista y haga clic en **Duplicar**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   La vista se duplica y el nombre de la nueva vista sigue el siguiente patrón: `Original view's name (Copy)`. La nueva pestaña de vista se muestra al final de todas las pestañas de vista.

