---
title: Administrar vistas de registros
description: Puede mostrar registros en una tabla, una escala de tiempo o una vista de calendario al utilizar las funciones de planificación de Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: b3a2f3ee4d89a6370c498457c1958cd7b9ea69b8
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 0%

---

# Administrar vistas de registros

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Después de seleccionar un tipo de registro en el área de funciones de planificación de Adobe Workfront, puede mostrar todos los registros de ese tipo en las siguientes vistas:

* Tabla

  Para obtener más información, consulte [Administrar la vista de tabla](../views/manage-the-table-view.md).

* Cronología

  Para obtener más información, consulte [Administrar la vista de cronología](../views/manage-the-timeline-view.md).

<!--* Calendar 

    For more information, see [Manage the calendar view](/help/quicksilver/maestro/views/manage-the-calendar-view.md). -->

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

En este artículo se describe la siguiente información sobre las vistas de Maestro:

* [Creación y edición de una vista](#create-or-edit-record-views)
* [Eliminación de una vista](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [Compartir una vista](#share-a-view)

## Similitudes y diferencias entre las vistas de tabla y de escala de tiempo

<!-- should we include Calendar here or remove this section???-->

En la tabla siguiente se muestran las similitudes y diferencias entre las vistas de tabla y de escala de tiempo de Maestro:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Función | Vista de tabla | Vista Cronología |
|-----------------------------------------------------------------------|------------|---------------|
| Mostrar registros en una lista o tabla | ✓ |              |
| Mostrar todos los campos como columnas en la tabla de forma predeterminada | ✓ |              |
| Ocultar o mostrar campos (o columnas) | ✓ |               |
| Editar valores de campo para cada registro | ✓ |               |
| Agregar registros como filas nuevas en la vista | ✓ |               |
| Agregar campos como nuevas columnas en la vista | ✓ |               |
| Copiar filas de una lista externa y pegarlas en una tabla | ✓ |               |
| Mostrar registros en una cronología |            | ✓ |
| Filtrar registros | ✓ | ✓ |
| Agrupar registros | ✓ | ✓ |
| Ordenar registros | ✓ |              |
| Registros de código de color |           | ✓ |
| Agrupaciones de código de color |           | ✓ |
| Buscar registros específicos | ✓ | ✓ |
| Compartir vista | ✓ | ✓ |
| Abra la página Detalles del registro desde la vista | ✓ | ✓ |

## Creación o edición de vistas {#create-or-edit-views}

{{step1-to-maestro}}


El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada. Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).

1. Haga clic en una tarjeta de tipo de registro. Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

<!--
    1. Click **+ View** to add a new view. 

    1. Select from the following types of views: 

        * Table
        * Timeline
        * Calendar

        >[!TIP]
        >
        >When you create a record type, the table view is also created by default. 
        >
        >To create a timeline or a calendar view, the record type you build the view for must have at least two date fields. Otherwise, the Timeline and the Calendar options are dimmed.
        >
        >(*********remove all of the below steps and replace the screen shot when calendar view releases*********)
    -->

1. Haga clic en **Ver** y seleccione una de las opciones existentes. **Vista de tabla** ![](assets/table-view-icon.png) o haga clic en **Crear vista > Tabla** para crear una vista de tabla

   O

   Seleccionar un existente **Vista Cronología** ![](assets/timeline-view-icon.png) ver o hacer clic **Crear vista > Cronología** para crear una vista de cronología.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Para crear una vista de escala de tiempo, el tipo de registro para el que genere la vista debe tener al menos dos campos de fecha. De lo contrario, la opción Cronología aparece atenuada.

1. (Opcional) Actualice el nombre de la vista y haga clic en **Crear** para guardar una vista de tabla

   O haga clic en **Siguiente**, al crear una cronología <!--or calendar--> vista.

   De forma predeterminada, Workfront asigna a la vista el nombre &quot;Tabla &lt; número >&quot; o &quot;Línea de tiempo &lt; número >&quot;, <!--or "Calendar < number >"-->. El número es un incremento generado automáticamente.

1. (Condicional) Seleccione las fechas de inicio y finalización de los registros que se mostrarán en la cronología <!--or calendar--> y, a continuación, haga clic en **Crear**.
1. (Opcional) Para cambiar el nombre de una vista una vez creada, haga clic en el menú desplegable de vista y, a continuación, haga clic en **Más** menú ![](assets/more-menu.png) > **Cambiar nombre** para actualizar el nombre de la vista. <!--ensure there is not another saving step here?!-->
   <!--1. (Optional) To rename a view after it is created, double-click the view name and start typing the new name, or click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Rename**.-->
1. (Opcional) Para administrar un tipo de vista específico, consulte los siguientes artículos:

   * [Administrar la vista de tabla](../views/manage-the-table-view.md)
   * [Administrar la vista de cronología](../views/manage-the-timeline-view.md)
     <!--* [Manage the calendar view](/help/quicksilver/maestro/views/manage-the-calendar-view.md)-->


## Eliminar vistas

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada. Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).

1. Haga clic en una tarjeta de tipo de registro.

   Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

<!--1. Hover over on the of the view's names in the view tab, then click **More** ![](assets/more-menu.png) > **Delete**. (********delete the instructions below but keep the last step***********)-->
1. Haga clic en el menú desplegable de vista, pase el cursor sobre una de las vistas de la lista y, a continuación, haga clic en **Más** menú ![](assets/more-menu.png) > **Eliminar**.
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
