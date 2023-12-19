---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Filtrado de información en el Distribuidor de cargas de trabajo
description: Para encontrar de forma eficaz los elementos de trabajo y centrarse en los usuarios o elementos que administra, le recomendamos encarecidamente que utilice filtros en el Distribuidor de cargas de trabajo.
author: Alina
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '2463'
ht-degree: 0%

---

# Filtrado de información en el Distribuidor de cargas de trabajo

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

Como administrador de recursos, puede utilizar el Distribuidor de cargas de trabajo para ver y administrar la carga de trabajo de los usuarios. Para obtener información más general sobre el Distribuidor de cargas de trabajo, consulte los siguientes artículos:

* [Resumen del Distribuidor de cargas](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Para encontrar de forma eficaz los elementos de trabajo y centrarse en los usuarios o elementos que administra, le recomendamos encarecidamente que utilice filtros en el Distribuidor de cargas de trabajo. Esto le permite mostrar la información correcta antes de empezar a administrar las asignaciones de los recursos.
>
>Al guardar y aplicar un filtro nuevo y luego salir del Distribuidor de cargas de trabajo, el filtro se conserva incluso después de cerrar la sesión y volver a iniciarla.


Este artículo contiene información sobre los filtros del Distribuidor de cargas de trabajo. Para obtener información sobre los filtros de Workfront, consulte [Información general sobre filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquier plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, al utilizar el Distribuidor de cargas de trabajo en el área de Recursos</p>
   <p>Trabaje con el Distribuidor de cargas de trabajo de un equipo o proyecto</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Vea o acceda a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filtros, vistas y agrupaciones</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Editar el acceso a filtros, vistas y agrupaciones al crear o editar filtros</span> </p> <p><b>NOTA</b>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores en los proyectos, tareas y problemas</p>
   <p>Administre permisos para los filtros que desee editar o eliminar</p>
     </p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Información general sobre los filtros del Distribuidor de cargas de trabajo

Tenga en cuenta lo siguiente al trabajar con filtros en el Distribuidor de cargas de trabajo:

* Según desde dónde acceda al Distribuidor de cargas de trabajo, es posible que Workfront ya esté filtrando la información por usted. Para obtener información sobre los filtros preaplicados, consulte la sección [Filtros preaplicados en el Distribuidor de cargas de trabajo](#pre-applied-filters-in-the-workload-balancer) en este artículo.
* Puede crear y aplicar un filtro sin guardarlo, o bien puede guardar un filtro para reutilizarlo más adelante.
* Cuando aplique un filtro sin guardarlo, puede volver a las listas originales al actualizar la página.
* Puede ver los filtros que ha creado o los filtros que otros usuarios han creado y compartido con usted.
* Al eliminar o editar un filtro compartido, también se elimina o edita para todas las personas con las que se comparte.
* Cuando se crean filtros en el Distribuidor de cargas de trabajo en una área, no están disponibles en otras áreas.

  Por ejemplo, los filtros creados en el área de Recursos no están disponibles en el Distribuidor de cargas de trabajo de un proyecto o equipo.

  Para obtener información sobre dónde encontrar el Distribuidor de cargas de trabajo, consulte [Localización del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* Solo puede ver los elementos que coincidan con los filtros seleccionados y que también coincidan con las fechas dentro de la cronología mostrada en la pantalla del Distribuidor de cargas de trabajo.

## Filtros preaplicados en el Distribuidor de cargas de trabajo {#pre-applied-filters-in-the-workload-balancer}

El Distribuidor de cargas de trabajo muestra información en dos áreas independientes:

* **El área de trabajo sin asignar**: elementos de trabajo que aún no se han asignado a los usuarios.
* **El área Trabajo asignado**: elementos de trabajo asignados a usuarios.

  Para obtener información sobre lo que se muestra en cada una de las áreas, consulte [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Cada área del Distribuidor de cargas de trabajo tiene su propio conjunto de filtros que funcionan de forma independiente entre sí. Debe configurar ambos filtros para indicar qué información desea ver en cada área.

El Distribuidor de cargas de trabajo muestra los usuarios y sus elementos de trabajo.
Los elementos de trabajo asignados a los usuarios solo se muestran cuando las fechas de los elementos coinciden con el lapso de tiempo mostrado en la pantalla.

Según desde dónde acceda al Distribuidor de cargas de trabajo, las áreas sin asignar y asignadas ya están filtradas según determinados criterios, como se describe en la siguiente tabla:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Área de Workfront donde se accede al Distribuidor de cargas de trabajo</strong></td> 
   <td><b>Elementos que se muestran en el área Trabajo no asignado de forma predeterminada</b> </td> 
   <td><b>Elementos que se muestran en el área Trabajo asignado de forma predeterminada</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">El área de recursos</td> 
   <td>Aquí no se muestran elementos de forma predeterminada. Debe personalizar los filtros para ver los elementos de trabajo de esta área.</td> 
   <td>Usuarios que son miembros de cualquiera de sus equipos y sus elementos de trabajo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un equipo</td> 
   <td>Elementos de trabajo asignados al equipo o al equipo y un rol. </td> 
   <td> <p>Usuarios que son miembros del equipo seleccionado y sus elementos de trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un proyecto</td> 
   <td> <p>En esta área se muestran los elementos de trabajo no asignados o los elementos asignados a equipos o roles en el proyecto seleccionado.</p> </td> 
   <td> <p>Usuarios asignados al menos a un elemento de trabajo del proyecto seleccionado y sus elementos de trabajo en el proyecto cuando se aplica el filtro predeterminado del sistema <b>Elementos de trabajo de este proyecto</b> está seleccionado. </p>

<p>Cuando el filtro predeterminado del sistema <b>Elementos de trabajo de este proyecto</b> Si no está seleccionada, el área de Trabajo asignado de un proyecto muestra todos los elementos de trabajo de los usuarios asignados al menos a un elemento del proyecto seleccionado.  </p> De forma predeterminada, este filtro no está seleccionado.

<b>NOTA</b>
<p>Puede activar la opción Mostrar todos los usuarios en el Distribuidor de cargas de trabajo de un proyecto para mostrar todos los usuarios del sistema. Para obtener más información, consulte <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navegación por el Distribuidor de cargas de trabajo</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## Crear filtros del Distribuidor de cargas de trabajo

El proceso de creación de filtros para las áreas de Trabajo no asignado y Trabajo asignado en el Distribuidor de cargas de trabajo es idéntico, independientemente de desde dónde acceda al Distribuidor de cargas de trabajo. Para obtener información sobre cómo localizar el Distribuidor de cargas de trabajo, consulte [Localización del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Puede crear un filtro desde cero o editar uno de los filtros predefinidos. Para obtener información sobre los filtros existentes que puede editar, consulte la [Editar un filtro existente en el Distribuidor de cargas de trabajo](#edit-an-existing-filter-in-the-workload-balancer) de este artículo.

1. Vaya al Distribuidor de cargas de trabajo.

   Para obtener información sobre el acceso al Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en **Filtrar** icono ![](assets/filter-icon.png) en la esquina superior derecha de cualquiera de las **Trabajo sin asignar** o el **Trabajo asignado** áreas.

   El cuadro Generador de filtros se muestra a la derecha. El nombre del área para la que se crea el filtro se muestra en el encabezado del cuadro.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Opcional y condicional) Si accede al Distribuidor de cargas de trabajo en el área de Recursos, es posible que el filtro Predeterminado predefinido ya se haya aplicado al área de Trabajo asignado. Puede editar y guardar una copia del filtro predeterminado.

   >[!TIP]
   >
   >El filtro predeterminado muestra los usuarios que pertenecen a cualquiera de sus equipos y sus elementos de trabajo. Puede editar una copia de este filtro.

   Si accede al [!UICONTROL Distribuidor de cargas de trabajo] de un proyecto, el &quot;[!UICONTROL Elementos de trabajo de este proyecto]Es posible que el filtro &quot; ya se haya aplicado. Esto muestra solamente los elementos de trabajo asignados a los usuarios de este proyecto. Puede duplicar y guardar una copia de este filtro.

   De forma predeterminada, la variable [!UICONTROL Distribuidor de cargas de trabajo] de un proyecto muestra todos los elementos de trabajo asignados a todos los usuarios del proyecto.


1. Clic **Nuevo filtro.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. Para crear un filtro, haga lo siguiente:

   1. Seleccione un nombre de campo en el primer menú desplegable o haga clic en **Examinar campos** para empezar a escribir el nombre de un campo que no se muestra de forma predeterminada.

      >[!IMPORTANT]
      >
      >Al hacer referencia a campos personalizados, debe escribir el nombre del campo y no la etiqueta del campo. La etiqueta de campo se muestra en un formulario personalizado adjunto a un objeto. Para obtener información sobre la diferencia entre la etiqueta y el nombre de un campo personalizado, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (Condicional) Si hizo clic en **Examinar campos**, escriba el nombre de un campo en la **Buscar** y selecciónelo cuando se muestre en la lista.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >Puede seleccionar un campo de las siguientes secciones:
      >
      >* **Selecciones recientes**: los campos para los que ha filtrado recientemente.
      >* **Campos sugeridos**: los campos más utilizados.


   1. Seleccione un modificador en el segundo menú desplegable. Para obtener información sobre los modificadores de filtro de Workfront, consulte [Filtros y modificadores de condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Seleccione o escriba un valor para el campo que está filtrando.

      >[!NOTE]
      >
      > Si desea visualizar objetos de trabajo de un portafolio específico, puede aplicar el siguiente filtro: &quot;El nombre del Portfolio contiene marketing&quot;. Esto muestra los elementos de trabajo que pertenecen a cualquier portafolio que contenga &quot;marketing&quot; en el nombre.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

   1. (Opcional) Haga clic en **Eliminar** icono ![](assets/delete.png) para eliminar un criterio de filtro.

1. (Opcional) Haga clic en **Añadir filtro** para agregar otro criterio de filtro, repita las acciones del paso 4.

   <!--(NOTE: ensure this stays correct)-->

1. Clic **Aplicar** para aplicar los resultados del filtro al área seleccionada del Distribuidor de cargas de trabajo sin guardarla.

   La lista de elementos de trabajo se actualiza a la izquierda.

   >[!IMPORTANT]
   >
   >Los resultados se muestran en el Distribuidor de cargas de trabajo cuando todas las instrucciones de filtro agregadas son verdaderas simultáneamente.

   El filtro se conserva hasta que se actualiza la página.

   El **Aplicar** El botón se sustituye por una **Guardar como nuevo** botón.

1. Clic **Guardar como nuevo** para guardar el filtro para uso futuro.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Clic **Cancelar** en cualquier momento, le lleva de nuevo al área de creación de filtros.

1. Seleccionar **Filtro sin título** e introduzca en su lugar el nombre del nuevo filtro.
1. Seleccione un icono para el nuevo filtro en la **Icono** menú desplegable.

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Opcional) Agregue una descripción para el filtro para indicar qué tiene de único. La descripción se muestra debajo del nombre del filtro en la lista de filtros.
1. Haga clic en **Guardar**.

   Los filtros guardados se muestran en el área Mis filtros del cuadro de filtro.

   Para obtener información sobre cómo aplicar filtros guardados, consulte la sección [Eliminar un filtro guardado en el Distribuidor de cargas de trabajo](#delete-a-saved-filter-in-the-workload-balancer) en este artículo.

1. (Condicional) Pase el ratón sobre **Icono de filtro** ![](assets/filter-icon.png) en la esquina superior derecha de la **Trabajo sin asignar** o el **Trabajo asignado** áreas para mostrar información sobre herramientas con el nombre o el número de filtros que se aplican actualmente.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Duplicación de un filtro

Puede duplicar y editar un filtro para crear uno nuevo.

1. Vaya al Distribuidor de cargas de trabajo.

   Para obtener información sobre el acceso al Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en **Filtrar** icono ![](assets/filter-icon.png) en la esquina superior derecha de cualquiera de las **Trabajo sin asignar** o el **Trabajo asignado** áreas.

   El cuadro Generador de filtros se muestra a la derecha. El nombre del área para la que se crea el filtro se muestra en el encabezado del cuadro.

1. Pase el ratón sobre un filtro existente y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Duplicar**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Al editar un filtro, puede hacer clic en el **Más** , en la esquina inferior izquierda del cuadro Editar filtro, y haga clic en **Duplicar**.

1. Edite la siguiente información para el filtro duplicado:

   * Nombre

     De forma predeterminada, el nuevo nombre de filtro es &quot;(Nombre del filtro original) Copiar&quot;.

   * Icono
   * Descripción
   * Cualquiera de los campos, modificadores o valores.

1. (Opcional) Haga clic en **Añadir filtro** para agregar más instrucciones al filtro duplicado.
1. Clic **Guardar** para guardar el filtro duplicado en **Mis filtros** área.

   El filtro original permanece sin cambios y el filtro duplicado se guarda como un nuevo filtro.

## Editar un filtro existente en el Distribuidor de cargas de trabajo {#edit-an-existing-filter-in-the-workload-balancer}

Puede editar un filtro guardado en el Distribuidor de cargas de trabajo.

>[!TIP]
>
>Al editar un filtro compartido con otros usuarios, también verán los cambios que realice.

1. Vaya al Distribuidor de cargas de trabajo.

   Para obtener información sobre el acceso al Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en **Icono de filtro** ![](assets/filter-icon.png) en la esquina superior derecha de la **Sin asignar** o **Trabajo asignado** áreas.\
   El generador de filtros se muestra a la derecha.

1. Pase el ratón sobre el filtro que quiere editar y luego haga clic en **Editar** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. Realice una de las siguientes acciones:

   * Modifique cualquiera de las instrucciones de filtro
   * Clic **Añadir filtro** para agregar nuevas instrucciones de filtro
   * Haga clic en **Eliminar** icono ![](assets/delete.png) para eliminar las instrucciones de filtro existentes.

1. (Opcional) Haga clic en **Aplicar**.

   Los resultados se actualizan en el Distribuidor de cargas de trabajo de la izquierda para ilustrar los cambios realizados en el filtro.

1. Clic **Guardar.**

   Los resultados se actualizan en el Distribuidor de cargas de trabajo de la izquierda y el filtro se actualiza con la nueva información seleccionada.

## Eliminar un filtro guardado en el Distribuidor de cargas de trabajo {#delete-a-saved-filter-in-the-workload-balancer}

Tenga en cuenta lo siguiente antes de eliminar un filtro:

* No puede recuperar los filtros eliminados.
* No puede eliminar filtros predefinidos.
* No puede eliminar un filtro sin guardar. Se eliminan automáticamente después de cerrar la sesión y volver a iniciarla en Workfront.
* Al eliminar un filtro compartido, también se elimina para todos los usuarios con los que se comparte.
* Después de eliminar todos los filtros guardados, el Distribuidor de cargas de trabajo se muestra según los valores predeterminados originales.

>[!NOTE]
>
>Cuando elimine un filtro compartido con otros, también se eliminará para ellos.

1. Ir al Distribuidor de cargas de trabajo
1. Haga clic en **Icono de filtro** ![](assets/filter-icon.png) en la esquina superior derecha de la **Trabajo sin asignar** o **Trabajo asignado** áreas.\
   El cuadro Generador de filtros se muestra a la derecha.

1. Pase el ratón sobre un filtro y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Eliminar**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Al editar un filtro, puede hacer clic en el **Más** , en la esquina inferior izquierda del cuadro Editar filtro, y haga clic en **Eliminar**.

1. (Opcional) Haga clic en **Cancelar** para evitar la eliminación y volver a la lista de filtros.
1. Clic **Eliminar** para confirmar la eliminación.

   El filtro se elimina en su nombre y en el de todos los usuarios que tenían permisos para utilizarlo.

## Uso compartido de filtros en el Distribuidor de cargas de trabajo

Puede compartir un filtro que haya creado o que otros usuarios hayan compartido con usted.

Tenga en cuenta lo siguiente al compartir filtros en el Distribuidor de cargas de trabajo:

* Puede compartir filtros con usuarios, equipos, funciones y empresas activos, o bien puede hacerlos visibles para todos los usuarios de la instancia de Workfront.
* Los filtros que comparte en el área de Recursos no son visibles en el Distribuidor de cargas de trabajo de un proyecto o equipo.
* Los filtros del Distribuidor de cargas de trabajo que comparte con otros usuarios no son visibles en otras áreas de Workfront.

Para compartir un filtro:

1. Ir al Distribuidor de cargas de trabajo
1. Haga clic en **Icono de filtro** ![](assets/filter-icon.png) en la esquina superior derecha de la **Trabajo sin asignar** o **Trabajo asignado** áreas.\
   El cuadro Generador de filtros se muestra a la derecha.

1. Pase el ratón sobre un filtro y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Compartir.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Al editar un filtro, puede hacer clic en el **Más** , en la esquina inferior izquierda del cuadro Editar filtro, y haga clic en **Compartir**.

   Se muestra el cuadro Compartir filtros.

1. Habilite la **Ver todo el sistema** configuración. Esto otorga permiso a los usuarios de Workfront para ver el filtro.

   O

   Empiece a escribir los nombres de los usuarios, equipos, roles, grupos o empresas con los que desea compartir el filtro en **Conceder acceso a** field.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Opcional) Haga clic en la flecha que señala a la derecha junto al nombre de una entidad para editar sus permisos en el filtro y, a continuación, habilite el **Ver** o **Administrar** opción.

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Opcional) Habilite o deshabilite los permisos adicionales para una entidad mediante uno de los procedimientos siguientes:

   1. Clic **Ver** y deshabilite la **Compartir** opción. Está activada de forma predeterminada.

   1. Clic **Administrar** y deshabilite las **Compartir** o el **Eliminar** opción. Están habilitadas de forma predeterminada.

   >[!TIP]
   >
   >Los usuarios no pueden recibir un permiso superior a su nivel de acceso. Si no tienen acceso a Editar filtros en su nivel de acceso, no pueden recibir permisos para administrar un filtro. Workfront deshabilita la opción Administrar para estos usuarios y la opción aparece atenuada.

1. Haga clic en **Compartir**. El filtro se comparte con las entidades especificadas.

   Los filtros que ha compartido se muestran en **Compartido conmigo** del cuadro de filtro.

   ![](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
