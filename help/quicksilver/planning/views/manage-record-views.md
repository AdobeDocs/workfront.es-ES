---
title: Administrar vistas de registros
description: Puede mostrar registros en una vista de tabla, escala de tiempo o calendario al utilizar Adobe Workfront Planning. Este artículo describe cómo crear una vista y editar o eliminar una existente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '1425'
ht-degree: 77%

---


# Administrar vistas de registros

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->


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
* [Eliminar una vista](#delete-views)
* [Duplicar una vista](#duplicate-views)
* [Habilitar los indicadores de presencia en tiempo real en una vista](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->


## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

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
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
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
   <p>Permisos de visualización de una vista para cambiar temporalmente su configuración</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--old: 

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
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->


## Consideraciones al trabajar con vistas de registros

* Las vistas de Workfront Planning son específicas del tipo de registro. No puede aplicar la misma vista a dos tipos de registro diferentes.
* Las vistas que cree solo serán visibles para usted y para los usuarios con los que comparta las vistas.
* Al modificar o eliminar una vista, esta se modifica y elimina para todos los usuarios que tengan permisos de acceso sobre ella.
* Cada usuario puede crear un máximo de 100 vistas. Puede mostrar más de 100 vistas para un tipo de registro, pero un usuario solo puede crear 100 vistas.
* Puede compartir vistas que cree con otros usuarios. Para obtener más información, consulte [Compartir vistas](/help/quicksilver/planning/access/share-views.md).
* Los siguientes elementos son exclusivos de cada vista de registro:

   * Filtro
   * Agrupación
   * Ordenar
   * Aspecto de la barra (para la vista de la línea de tiempo)

  <!-- some of these are not available in all of the views - edit above-->

  Por ejemplo, al crear un filtro en una vista de tabla, los resultados del filtro solo son visibles en la vista seleccionada y no en todas las vistas asociadas al tipo de registro.

  >[!NOTE]
  >
  > Es posible que algunos elementos de vista no estén disponibles para todas las vistas.


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
| Registros con código de color |           | ✓ | ✓ |
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

   Según el ancho de la pantalla, es posible que se muestren vistas adicionales en el menú **Más** ![](assets/more-menu.png).


>[!TIP]
>
>Al crear un tipo de registro, la vista de tabla también se crea de forma predeterminada.
>
>Para crear una vista de línea de tiempo o de calendario, el tipo de registro para el que genere la vista debe tener al menos dos campos de fecha.
>
>De lo contrario, las opciones Línea de tiempo y Calendario aparecen atenuadas.
>

![](assets/view-types-drop-down-from-record-type-list.png)

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
1. (Opcional) Haga clic en el menú **Más** ![](assets/more-caret-down-icon-views.png) que está junto a la última vista para mostrar todas las vistas del tipo de registro seleccionado.

   Se muestran vistas adicionales en el menú **Más** después de la última pestaña de vista. El número al lado del menú **Más** muestra el número de vistas adicionales.
1. (Opcional) Para cambiar el nombre de una vista una vez creada, haga clic en el menú desplegable de vista y, a continuación, haga clic en el menú **Más** ![](assets/more-menu.png) > **Cambiar nombre** para actualizar el nombre de la vista

   O

   Haga doble clic en el nombre de la vista y empiece a escribir el nuevo nombre. <!--ensure there is not another saving step here?!-->

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

1. Pase el puntero por encima de uno de los nombres de la vista en la ficha de la vista, luego haga clic en **Más** ![](assets/more-menu.png) a la izquierda del nombre de la vista y luego haga clic en **Eliminar**.
En primer lugar, es posible que deba hacer clic en **Más** a la izquierda de la última ficha para encontrar la vista que desee eliminar.

1. Haga clic en **Eliminar** para confirmar. <!--ensure there is not another saving step here?!-->

   La vista se elimina para todos los usuarios que pueden acceder al área de registros y no se puede recuperar.

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## Duplicar una vista

Si desea conservar varias versiones de una vista y realizar ligeros cambios entre ellas, puede duplicar una vista.

Al duplicar una vista, se crean copias idénticas de una vista existente.

Los permisos de uso compartido de la vista original no se transfieren a la vista duplicada.

{{step1-to-planning}}

1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Pase el puntero por encima de la ficha de la vista que desee duplicar, haga clic en el menú **Más** ![](assets/more-menu.png) a la derecha del nombre de la vista y luego haga clic en **Duplicar**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   La vista está duplicada y el nombre de la nueva vista sigue el siguiente patrón: `Original view's name (Copy)`. La nueva ficha de vista se muestra al final de todas las fichas de vista.

## Habilitar el indicador de presencia en tiempo real en una vista

De forma predeterminada, los avatares de otros usuarios que están editando información de registro al mismo tiempo que se muestran en la esquina superior derecha de todas las vistas de registros.

Al mostrar la vista de tabla, también puede ver qué campo está editando otro usuario en el momento en que está viendo el registro.

1. Vaya a una página de tipo de registro y abra cualquier vista.
1. (Condicional) Si hay otros usuarios editando al mismo tiempo los registros del tipo seleccionado, sus avatares se mostrarán en la esquina superior derecha de la vista.
1. Haga clic en el menú desplegable situado junto a los avatares y seleccione la opción **Mostrar colaboradores**. La opción está seleccionada de forma predeterminada.

   ![](assets/show-collaborators-toggle-selected.png)

1. (Condicional) Abra una vista de tabla y el campo que otra persona está editando activamente se resaltará en el color correspondiente al contorno de su avatar en la vista de tabla.

   Si el color de resaltado del avatar es gris, el usuario dejó de editar activamente el registro hace más de 30 segundos.

   ![](assets/real-time-indicator-table-field-and-avatar-connection.png)

   >[!TIP]
   >
   >Puede seleccionar la opción **Mostrar colaboradores** de cualquier vista. El campo editado actualmente por otros usuarios sólo se describe en la vista de tabla.
