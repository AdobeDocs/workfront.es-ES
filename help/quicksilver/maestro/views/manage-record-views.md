---
title: Administrar vistas de registros
description: Puede mostrar registros en una tabla o en una vista de escala de tiempo al utilizar Adobe Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 6d1d3d82e15f4232ff81294d9094c2683b01ca89
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 1%

---

# Administrar vistas de registros

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para utilizar las funciones de Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Después de seleccionar un tipo de registro en Adobe Maestro, puede mostrar todos los registros de ese tipo en las vistas siguientes:

* Tabla

  Para obtener más información, consulte [Administrar la vista de tabla](../views/manage-the-table-view.md).
* Cronología

  Para obtener más información, consulte [Administrar la vista de cronología](../views/manage-the-timeline-view.md).

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
   <p> producto de Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta cerrado de Adobe Maestro. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td role="rowheader">Nivel de acceso</td>
   <td> <p>Cualquiera</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Plantilla de diseño</td>
   <td> <p>El administrador del sistema debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/grant-access.md">Conceder acceso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Consideraciones al trabajar con las vistas de Maestro

* Las vistas de Maestro son específicas del tipo de registro. No se puede aplicar la misma vista a dos tipos de registro diferentes.
* Las vistas que cree serán visibles para todos los usuarios que tengan acceso al área de Maestro. <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* La creación de vistas para tipos de registro operativo es idéntica a la creación de vistas para tipos de registro de taxonomía.
* Al modificar o eliminar una vista, ésta se modifica y elimina para todos los usuarios que tengan acceso al área de Maestro.
* Los siguientes elementos son exclusivos de cada vista de Maestro:

   * Filtro
   * Agrupación
   * Ordenar

  <!-- some of these are not available in all of the views - edit above-->

  Por ejemplo, al crear un filtro en una vista de tabla, los resultados del filtro solo son visibles en la vista seleccionada y no en todas las vistas que aparecen en el menú desplegable Ver.

  >[!NOTE]
  >
  > Debido a que Maestro se encuentra actualmente en estado beta, es posible que algunos elementos de vista no estén disponibles para ambas vistas.


En este artículo se describe la siguiente información sobre las vistas de Maestro:

* [Creación y edición de una vista](#create-or-edit-record-views)
* [Eliminación de una vista](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
  <!--* [Share a view](#share-views) - not possible yet-->

## Similitudes y diferencias entre las vistas de tabla y de escala de tiempo

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
| Agrupar registros |           | ✓ |
| Ordenar registros | ✓ |              |
| Registros de código de color |           | ✓ |
| Agrupaciones de código de color |           | ✓ |

<!--| Sort groupings                                                        | ✓          | ✓             |-->
<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

## Creación o edición de vistas {#create-or-edit-views}

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha, o la **Menú principal** icono ![](assets/main-menu-shell.png) en la esquina superior izquierda, si está disponible, haga clic en **Maestro** ![](assets/maestro-icon.png).
El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada. Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).
1. Haga clic en una tarjeta de tipo de registro. Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Haga clic en **Ver** y seleccione una de las opciones existentes. **Vista de tabla** ![](assets/table-view-icon.png) o haga clic en **Crear vista > Tabla** para crear una vista de tabla

   O

   Seleccionar un existente **Vista Cronología** ![](assets/timeline-view-icon.png) ver o hacer clic **Crear vista > Cronología** para crear una vista de cronología.

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    Para crear una vista de escala de tiempo, el tipo de registro para el que genere la vista debe tener al menos dos campos de fecha. De lo contrario, la opción Cronología aparece atenuada.

1. (Opcional) Actualice el nombre de la vista y haga clic en **Crear** para guardarlo.

   De forma predeterminada, Maestro asigna a la vista el nombre &quot;Tabla &lt; número >&quot; o &quot;Línea de tiempo &lt; número >&quot;. El número es un incremento generado automáticamente.

1. (Opcional) Para cambiar el nombre de una vista una vez creada, haga clic en el menú desplegable de vista y, a continuación, haga clic en **Más** menú ![](assets/more-menu.png) > **Cambiar nombre** para actualizar el nombre de la vista. <!--ensure there is not another saving step here?!-->
1. (Opcional) Para administrar una vista, consulte los siguientes artículos para obtener más información:

   * [Administrar la vista de tabla](../views/manage-the-table-view.md)
   * [Administrar la vista de cronología](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## Eliminar vistas

1. Desde el **Menú principal** ![](assets/main-menu-workfront.png) en la esquina superior derecha de la pantalla, <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> click **Maestro** ![](assets/maestro-icon.png).

   El espacio de trabajo al que se accedió por última vez se abre de forma predeterminada. Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).
1. Haga clic en una tarjeta de tipo de registro.

   Para obtener información sobre cómo crear un tipo de registro, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Haga clic en el menú desplegable de vista, pase el cursor sobre una de las vistas de la lista y, a continuación, haga clic en **Más** menú ![](assets/more-menu.png) > **Eliminar**.
1. Clic **Eliminar** para confirmar. <!--ensure there is not another saving step here?!-->

   La vista se elimina para todos los usuarios que pueden tener acceso al área de Maestro y no se puede recuperar.

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
