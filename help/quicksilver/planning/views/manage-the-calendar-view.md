---
title: Administrar la vista de calendario
description: Puede mostrar registros y sus campos en una vista de calendario. Este artículo describe cómo crear una vista de calendario y editar o eliminar una existente.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 63%

---

# Administrar la vista de calendario

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede mostrar los registros y sus campos en una vista de calendario, desde la página de tipo de registro.

Para obtener información sobre las vistas de Adobe Workfront Planning y cómo administrarlas, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

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
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
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
<p><span class="preview">En el entorno de vista previa, los usuarios estándar y los administradores del sistema tienen Planning habilitado de forma predeterminada.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Administrar una vista de calendario {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Tenga en cuenta lo siguiente:

* Puede crear una vista de calendario únicamente si tiene al menos dos campos de fecha asociados a un tipo de registro. Cuando hay uno o ningún campo de fecha asociado a un tipo de registro, la opción de vista de calendario aparece atenuada.

  Puede seleccionar entre los campos de fecha de registro o los campos de fecha de búsqueda de los tipos de objeto o registro conectados.
* Se dan los siguientes escenarios:

   * Cuando las fechas de inicio y finalización no tienen valores, los registros no se muestran en el calendario.
   * Cuando las fechas de inicio o finalización no tienen valor, el registro se muestra como un evento de un día.
   * Cuando la fecha de inicio es posterior a la fecha de finalización, el registro no se muestra en el calendario.

Para administrar una vista de calendario:

1. Vaya a la página del tipo de registro cuyo calendario desea ver.
1. Cree una vista de calendario, tal como se describe en el artículo [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).

   ![Ejemplo de vista de calendario](assets/calendar-view-example.png)

   Los registros asociados al tipo de registro seleccionado se muestran como barras en un calendario. El color de las barras coincide con el color del icono de registro.

1. Realice una de las siguientes acciones para navegar por el calendario:

   * Haga clic en los iconos izquierdo y derecho o utilice el desplazamiento horizontal para moverse hacia atrás y hacia adelante en el calendario.
   * Haga clic en **Hoy** para centrar el calendario en la fecha de hoy.
   * Seleccione una de las siguientes opciones del menú desplegable de lapso de tiempo para actualizar los incrementos de tiempo:

      * **Mes**: los registros se muestran en un calendario mensual.


      * **Semana**: los registros se muestran en las áreas siguientes:

         * Los registros que se extienden durante varios días se muestran en la parte superior del calendario.
         * Registros que duran un día o menos y que se muestran en la mitad inferior de la vista de calendario. Si ha seleccionado mostrar la hora de las fechas de inicio y finalización, el registro se muestra a la hora adecuada dentro del día en que se produce.


1. Actualice los siguientes elementos de vista como se describe en las subsecciones siguientes:
   * [Filtros](#add-filters)
   * [Configuración](#edit-the-calendar-view-settings)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Añadir filtros

Puede reducir la cantidad de información que se muestra en la pantalla mediante filtros.

Tenga en cuenta lo siguiente al trabajar con filtros en la vista de calendario:

<!-- this list is almost identical to the one for the table view - update both-->

* Los filtros que cree para una vista de calendario funcionarán de forma independiente de los filtros de cualquier otra vista aplicada al mismo tipo de registro.

* Los filtros son exclusivos de la vista que seleccione. Dos vistas de calendario del mismo tipo de registro pueden tener diferentes filtros aplicados.

* Dos usuarios que ven la misma vista de calendario ven el mismo filtro que se está aplicando actualmente.

* No puede asignar un nombre a los filtros que usted genere para una vista de calendario.

* Al eliminar los filtros, se eliminan de todos los usuarios que tengan acceso al mismo tipo de registro que usted y que muestren la misma vista que usted.

* Añadir filtros en la vista de calendario es idéntico a añadir filtros en la vista de tabla.

  Para obtener más información, consulte la sección “Añadir filtros” en el artículo [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

* Puede filtrar por campos de registro conectados o por campos de búsqueda.

* Puede filtrar por campos de búsqueda que muestren varios valores.

### Editar la configuración de vista de calendario

Editar la configuración de vista de calendario es similar a editar la configuración de una vista de cronología.

Para obtener más información, consulte la sección &quot;Editar la configuración de la vista de la cronología&quot; en el artículo [Administrar la vista de la cronología](/help/quicksilver/planning/views/manage-the-timeline-view.md).
