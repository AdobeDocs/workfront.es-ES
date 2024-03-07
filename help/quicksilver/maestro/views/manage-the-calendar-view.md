---
title: Administrar la vista de calendario
description: Puede mostrar registros y sus campos en una vista de calendario.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ff52e43fc5ed5a7939b9e28b2bda195e94e81724
workflow-type: tm+mt
source-wordcount: '338'
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

{{maestro-important-intro}}

Puede mostrar los registros y sus campos en una vista de calendario, desde la página de tipo de registro.

Para obtener información acerca de las vistas de Maestro y cómo administrarlas, vea [Administrar vistas de registros](../views/manage-record-views.md).

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
   <td role="rowheader">Configuración del nivel de acceso</td>
   <td> <p>No hay controles de nivel de acceso para Maestro </p>  
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


## Administrar una vista de calendario {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Tenga en cuenta lo siguiente:

* Puede crear una vista Calendario únicamente si tiene al menos dos campos de fecha asociados a un tipo de registro. Cuando hay uno o ningún campo de fecha asociado a un tipo de registro, la opción de vista Calendario aparece atenuada.
* Los siguientes escenarios:

   * Cuando las fechas de inicio y finalización no tienen valores, los registros no se muestran en el calendario
   * Cuando las fechas Start o End no tienen ningún valor, el registro se muestra como un evento de un día
   * Cuando la fecha de inicio es posterior a la fecha de finalización, el registro no se muestra en el calendario.

Para administrar una vista de calendario:

1. Vaya a la página del tipo de registro cuyo calendario desea ver.
1. Cree una vista de calendario como se describe en el artículo [Administrar vistas de registros](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   Los registros asociados al tipo de registro seleccionado se muestran como barras en un calendario.

1. Realice una de las siguientes acciones para navegar por el calendario:

   * Haga clic en los iconos izquierdo y derecho o utilice el desplazamiento horizontal para moverse hacia atrás y hacia adelante en el calendario.
   * Clic **Hoy** para centrar el calendario en la fecha actual.
   * Seleccione una de las siguientes opciones del menú desplegable lapso de tiempo para actualizar los incrementos de tiempo:

      * Mes