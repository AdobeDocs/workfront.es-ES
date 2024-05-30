---
title: Administrar la vista de calendario
description: Puede mostrar registros y sus campos en una vista de calendario.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# Administrar la vista de calendario

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{planning-important-intro}}

Puede mostrar los registros y sus campos en una vista de calendario, desde la página de tipo de registro.

Para obtener información sobre las vistas de funcionalidades de Adobe Workfront Planning y cómo administrarlas, consulte [Administrar vistas de registros](../views/manage-record-views.md).

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
<p>Su organización debe estar inscrita en el programa beta de Adobe Workfront Planning. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>  
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


## Administrar una vista de calendario {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Tenga en cuenta lo siguiente:

* Puede crear una vista Calendario únicamente si tiene al menos dos campos de fecha asociados a un tipo de registro. Cuando hay uno o ningún campo de fecha asociado a un tipo de registro, la opción de vista Calendario aparece atenuada.
* Existen los siguientes escenarios:

   * Cuando las fechas de inicio y finalización no tienen valores, los registros no se muestran en el calendario
   * Cuando las fechas Start o End no tienen valor, el registro se muestra como un evento de un día
   * Cuando la fecha de inicio es posterior a la fecha de finalización, el registro no se muestra en el calendario.

Para administrar una vista de calendario:

1. Vaya a la página del tipo de registro cuyo calendario desea ver.
1. Cree una vista de calendario como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   Los registros asociados al tipo de registro seleccionado se muestran como barras en un calendario. El color de las barras coincide con el color del icono de registro.

1. Realice una de las siguientes acciones para navegar por el calendario:

   * Haga clic en los iconos izquierdo y derecho o utilice el desplazamiento horizontal para moverse hacia atrás y hacia adelante en el calendario.
   * Clic **Hoy** para centrar el calendario en la fecha actual.
   * Seleccione una de las siguientes opciones del menú desplegable lapso de tiempo para actualizar los incrementos de tiempo:

      * Mes
1. Actualice los siguientes elementos de vista como se describe en las subsecciones siguientes:
   * [Filtros](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Añadir filtros

Puede reducir la cantidad de información que se muestra en la pantalla mediante filtros.

Tenga en cuenta lo siguiente al trabajar con filtros en la vista de calendario:

<!-- this list is almost identical to the one for the table view - update both-->

* Los filtros que cree para una vista de calendario funcionarán de forma independiente de los filtros de cualquier otra vista aplicada al mismo tipo de registro.

* Los filtros son exclusivos de la vista seleccionada. Dos vistas de calendario del mismo tipo de registro pueden tener diferentes filtros aplicados.

* Dos usuarios que ven la misma vista de calendario ven el mismo filtro que se aplica actualmente.

* No puede asignar un nombre a los filtros que genere para una vista de calendario.

* Al eliminar los filtros, se eliminan de todos los que tengan acceso al mismo tipo de registro que usted y que muestren la misma vista que usted.

* Añadir filtros en la vista de calendario es idéntico a añadir filtros en la vista de tabla.

  Para obtener más información, consulte la sección &quot;Agregar filtros&quot; en el artículo [Administrar la vista de tabla](/help/quicksilver/maestro/views/manage-the-table-view.md).

* Puede filtrar por campos de registro conectados o campos de búsqueda, pero no por los campos que permiten la vinculación a varios registros.
