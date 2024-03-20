---
title: Administrar vistas de registros
description: Puede mostrar registros en una tabla, una escala de tiempo o una vista de calendario al utilizar las funciones de planificación de Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 1%

---

# Administrar vistas de registros

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Después de seleccionar un tipo de registro en el área de funciones de planificación de Adobe Workfront, puede mostrar todos los registros de ese tipo en las siguientes vistas:

* Tabla

  Para obtener más información, consulte [Administrar la vista de tabla](../views/manage-the-table-view.md).

* Cronología

  Para obtener más información, consulte [Administrar la vista de cronología](../views/manage-the-timeline-view.md).

* Calendario

  Para obtener más información, consulte [Administrar la vista de calendario](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

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
<p>Su organización debe estar inscrita en el programa beta cerrado de capacidades de planificación de Adobe Workfront. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
  </td>
  </tr>

<tr>
   <td role="rowheader">Configuración del nivel de acceso</td>
   <td> <p>No hay controles de nivel de acceso para las funciones de planificación de Workfront</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos de la vista</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Plantilla de diseño</td>
   <td> <p>El administrador del sistema debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Consideraciones al trabajar con vistas de registros

* Las vistas del área de funciones de planificación de Workfront son específicas del tipo de registro. No se puede aplicar la misma vista a dos tipos de registro diferentes.
* Las vistas que cree solo serán visibles para usted y para los usuarios con los que comparta las vistas.
* La creación de vistas para tipos de registro operativo es idéntica a la creación de vistas para tipos de registro de taxonomía.
* Al modificar o eliminar una vista, esta se modifica y elimina para todos los usuarios que tienen permisos de acceso a la vista.
* Los siguientes elementos son exclusivos de cada vista de registro:

   * Filtro
   * Agrupación
   * Ordenar

  <!-- some of these are not available in all of the views - edit above-->

  Por ejemplo, al crear un filtro en una vista de tabla, los resultados del filtro solo son visibles en la vista seleccionada y no en todas las vistas que aparecen en el menú desplegable Ver.

  >[!NOTE]
  >
  > Debido a que las funcionalidades de planificación de Adobe Workfront se encuentran actualmente en estado beta, es posible que algunos elementos de vista no estén disponibles para todas las vistas.

Este artículo describe la siguiente información sobre las vistas de registros:

* [Creación y edición de una vista](#create-or-edit-record-views)
* [Eliminación de una vista](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Compartir una vista](#share-a-view)

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
| Abra la página Detalles del registro desde la vista | ✓ | ✓ |    |


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

## Compartir una vista

Para obtener información sobre cómo compartir vistas, consulte [Compartir vistas](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
