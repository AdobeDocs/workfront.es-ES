---
title: Administrar vistas de registros
description: Puede mostrar registros en una vista de tabla, escala de tiempo o calendario al utilizar Adobe Workfront Planning. Este artículo describe cómo crear una vista y editar una existente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1181'
ht-degree: 46%

---


# Administrar vistas de registros

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Después de seleccionar un tipo de registro en el área de Adobe Workfront Planning, puede mostrar todos los registros de ese tipo en las siguientes vistas:

* Tabla

  Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

* Cronología

  Para obtener más información, consulte [Administrar la vista de cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md).

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

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier Workfront y cualquier paquete de Planning</p>
<p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p> Estándar para crear y eliminar vistas</p>
   <p>Colaborador o superior para actualizar los elementos de vista</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración de una vista</p>  
   <p>Ver permisos en una vista para cambiar temporalmente la configuración de la vista o para duplicarla</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya Planning.
   <p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>-->

## Consideraciones al trabajar con vistas de registros

* Las vistas de Workfront Planning son específicas del tipo de registro. No puede aplicar la misma vista a dos tipos de registro diferentes.
* Las vistas que cree solo serán visibles para usted y para los usuarios con los que comparta las vistas.
* Al modificar o eliminar una vista, esta se modifica y elimina para todos los usuarios que tengan permisos de acceso sobre ella.
* Cada usuario puede crear un máximo de 100 vistas. Puede mostrar más de 100 vistas para un tipo de registro, pero un usuario solo puede crear 100 vistas.
* Aunque algunos elementos de vista se pueden aplicar a varias vistas del mismo registro, son únicos en cada vista de registro:

   * Filtro
   * Ordenar (para la vista de tabla)
   * Colores de fila (para la vista de tabla)
   * Campos (para la vista de tabla)
   * Desglose (para la vista de cronología)
   * Agrupación (para las vistas Tabla y Cronología)
   * Apariencia de la barra (para las vistas de calendario y cronología)
   * Altura de fila (para la tabla y la vista de calendario mensual)

  Por ejemplo, al crear un filtro en una vista de tabla, los resultados del filtro sólo son visibles en la vista seleccionada (la vista de tabla) y no en todas las vistas asociadas al tipo de registro.

  >[!TIP]
  >
  >Algunos elementos de vista no estarán disponibles para todas las vistas.


## Similitudes y diferencias entre vistas de registros

En la tabla siguiente se muestran las similitudes y diferencias entre las vistas de tabla, cronología y calendario:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Función | Vista de tabla | Vista de cronología | Vista de calendario |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Mostrar registros en una lista o tabla | ✓ |              | |
| Mostrar todos los campos como columnas en la tabla de forma predeterminada | ✓ |              |    |
| Ocultar o mostrar campos (o columnas) | ✓ |               |    |
| Editar valores de campo para cada registro | ✓ |               |             |
| Añadir registros como filas nuevas en la vista | ✓ |               |        |
| Añadir campos como nuevas columnas en la vista | ✓ |               |         |
| Copiar filas de una lista externa y pegarlas en una tabla | ✓ |               |          |
| Mostrar registros en una cronología |            | ✓ |             |
| Filtrar registros | ✓ | ✓ | ✓ |
| Mostrar registros en un calendario |           |              | ✓ |
| Registros de grupo | ✓ | ✓ |  |
| Ordenar registros | ✓ |              |  |
| Registros con código de color | ✓ | ✓ | ✓ |
| Agrupaciones de código de color |           | ✓ |  |
| Buscar registros específicos | ✓ | ✓ |  |
| Compartir la vista con otros usuarios | ✓ | ✓ | ✓ |
| Abra la página del registro desde la vista | ✓ | ✓ |    |
| Mostrar registros por año y trimestre |           | ✓ |    |
| Mostrar registros por mes |           | ✓ | ✓ |
| Mostrar registros por semana |           |               | ✓ |
| Exportación de información desde una vista | ✓ |               |    |
| Mostrar en pantalla completa | ✓ | ✓ | ✓ |
| Creación de registros en la vista | ✓ | ✓ | ✓ |
| Desglose de registros por sus conexiones |          | ✓ |    |

## Crear o editar vistas {#create-or-edit-views}

{{step1-to-planning}}


1. Haga clic en la tarjeta de un espacio de trabajo.

   El espacio de trabajo se abre y los tipos de registro se muestran como tarjetas.

1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.

   De forma predeterminada, todos los registros del tipo seleccionado se muestran en la vista de tabla.

1. Haga clic en el icono desplegable ![Icono desplegable](assets/drop-down-icon.png) junto al nombre de la vista actual y, a continuación, haga clic en **+Nueva vista**.

1. Seleccione entre los siguientes tipos de vistas:

   * Tabla
   * Cronología
   * Calendario

1. Elija un tipo de vista y luego haga clic en **Crear**. Se añade una nueva vista al menú desplegable.

   >[!TIP]
   >
   >Al crear un tipo de registro, la vista de tabla también se crea de forma predeterminada.
   >
   >Para crear una vista de cronología o de calendario, el tipo de registro para el que genere la vista debe tener al menos dos campos de fecha.
   >
   >De lo contrario, las opciones Cronología y Calendario aparecen atenuadas.
   >  

   ![Crear cuadro de vista](assets/create-view-box.png)

1. (Opcional) Para editar una vista existente, haga clic en el menú desplegable a la derecha del nombre de la vista actual, luego escriba el nombre de una vista en el campo **Buscar** y presione Entrar en el teclado.
1. (Opcional) En el menú desplegable de vista, arrastre y suelte las vistas en orden de sus preferencias.

   ![Lista desplegable de tipos de vista de la lista de tipos de registro](assets/view-types-drop-down-from-record-type-list.png)

1. (Condicional) Haga clic en **Siguiente** al crear una vista de cronología o de calendario.

   De forma predeterminada, Workfront asigna a la vista uno de los nombres siguientes:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   El número es un incremento generado automáticamente.

1. (Condicional) Seleccione las **fechas de inicio** y **de finalización** para los registros que se mostrarán en la vista de cronología o de calendario.

   >[!NOTE]
   >
   >    Puede seleccionar entre los campos de fecha de registro o los campos de fecha de búsqueda de los tipos de objeto o registro conectados.
   >
   >Debe utilizar acumuladores para los campos de fecha (MAX o MIN) al seleccionar campos de búsqueda al conectar tipos de registro. Solo añadir los acumuladores le permite utilizar las fechas de las conexiones como fechas de inicio y finalización para las vistas de cronología y calendario.
   >
   >Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Haga clic en **Crear**.

   La vista se muestra como una nueva pestaña. Las vistas se muestran en orden cronológico a partir del momento en que se crearon o compartieron con el usuario.
1. (Opcional) Haga clic en el menú **Más** ![Más vistas del icono de acento circunflejo invertido](assets/more-caret-down-icon-views.png) junto a la última vista para mostrar todas las vistas del tipo de registro seleccionado.

   Se muestran vistas adicionales en el menú **Más** después de la última pestaña de vista. El número al lado del menú **Más** muestra el número de vistas adicionales.
1. (Opcional) Para cambiar el nombre de una vista una vez creada, haga clic en el menú desplegable de vista y, a continuación, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) > **Cambiar nombre** para actualizar el nombre de la vista

   O

   Haga doble clic en el nombre de la vista y empiece a escribir el nuevo nombre. <!--ensure there is not another saving step here?!-->

1. (Opcional) Haga clic en el icono **Pantalla completa** ![Abrir icono de pantalla completa](assets/open-full-screen-icon.png) para abrir cualquier vista en pantalla completa y, a continuación, en el icono **Salir de pantalla completa** ![Salir del icono de pantalla completa](assets/exit-full-screen-icon.png) o Escape del teclado para salir de la pantalla completa.

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
