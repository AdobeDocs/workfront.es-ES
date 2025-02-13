---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Filtrar información en el Distribuidor de cargas de trabajo
description: Para encontrar de forma eficaz los elementos de trabajo y centrarse en los usuarios o elementos que administra, le recomendamos encarecidamente que utilice filtros en el Distribuidor de cargas de trabajo.
author: Lisa
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 23c6d9335b0adcafc4e2ecdd8ef2d0ab09709fa8
workflow-type: tm+mt
source-wordcount: '2526'
ht-degree: 84%

---

# Filtrar información en el distribuidor de cargas de trabajo

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

Como administrador de recursos, puede utilizar el Distribuidor de cargas de trabajo para ver y administrar la carga de trabajo de los usuarios. Para obtener más información general sobre el Distribuidor de cargas de trabajo, consulte los siguientes artículos:

* [Información general del Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Para encontrar de forma eficaz los elementos de trabajo y centrarse en los usuarios o elementos que administra, le recomendamos encarecidamente que utilice filtros en el Distribuidor de cargas de trabajo. Esto le permite mostrar la información correcta antes de empezar a administrar las asignaciones de los recursos.
>
>Al guardar y aplicar un filtro nuevo, y luego salir del Distribuidor de cargas de trabajo, el filtro se conserva incluso después de haber cerrado la sesión y volver a iniciarla.

Este artículo contiene información sobre los filtros del Distribuidor de cargas de trabajo. Para obtener información sobre los filtros de Workfront, consulte [Información general sobre los filtros](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: Planificar, al usar el Distribuidor de cargas de trabajo en el área de Recursos;</br>
       Trabaje con el Distribuidor de cargas de trabajo de un equipo o proyecto</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a lo siguiente:</p> 
    <ul> 
     <li>Administración de recursos</li> 
     <li>Proyectos</li> 
     <li>Tareas</li> 
     <li>Problemas</li>
     <li>Filtros, vistas y agrupaciones</li>
    </ul>
    <p>Editar el acceso a filtros, vistas y agrupaciones al crear o editar filtros </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de visualización o superiores para proyectos, tareas y problemas</p>
   <p>Permisos de administración para los filtros que desee editar o eliminar</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Información general sobre los filtros en el Distribuidor de cargas de trabajo

Tenga en cuenta lo siguiente al trabajar con filtros en el Distribuidor de cargas de trabajo:

* Según desde dónde acceda al Distribuidor de cargas de trabajo, es posible que Workfront ya esté filtrando la información por usted. Para obtener información acerca de los filtros preaplicados, consulte la sección [Filtros preaplicados en el Distribuidor de cargas de trabajo](#pre-applied-filters-in-the-workload-balancer) en este artículo.
* Puede crear y aplicar un filtro sin guardarlo, o bien puede guardar un filtro para reutilizarlo más adelante.
* Cuando aplique un filtro sin guardarlo, puede volver a las listas originales al actualizar la página.
* Puede ver los filtros que ha creado o los filtros que otros usuarios han creado y compartido con usted.
* Al eliminar o editar un filtro compartido, ese filtro también se elimina o edita para todas las personas con las que se comparte.
* Cuando se crean filtros en el Distribuidor de cargas de trabajo de un área, no están disponibles en otras áreas.

  Por ejemplo, los filtros creados en el área Asignando recursos no están disponibles en el Distribuidor de cargas de trabajo de un proyecto o equipo.

  Para obtener información sobre dónde ubicar el Distribuidor de cargas de trabajo, consulte [Localizar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* Solo puede ver los elementos que coincidan con los filtros seleccionados y que también coincidan con las fechas dentro de la cronología mostrada en la pantalla del Distribuidor de cargas de trabajo.

## Filtros preaplicados en el Distribuidor de cargas de trabajo {#pre-applied-filters-in-the-workload-balancer}

El Distribuidor de cargas de trabajo muestra información en dos áreas independientes:

* **Área de trabajo sin asignar**: elementos de trabajo que aún no se han asignado a los usuarios.
* **Área de trabajo asignado**: elementos de trabajo asignados a usuarios.

  Para obtener información acerca de lo que se muestra en cada una de las áreas, consulte [Navegar por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

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
   <td><b>Elementos que se muestran en el área de Trabajo sin asignar de manera predeterminada</b> </td> 
   <td><b>Elementos que se muestran en el área de Trabajo asignado de manera predeterminada</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">El área de Recursos</td> 
   <td>De forma predeterminada, aquí no se muestra ningún elemento. Debe personalizar los filtros para ver los elementos de trabajo en esta área.</td> 
   <td>Usuarios que son miembros de cualquiera de sus equipos y sus elementos de trabajo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un equipo</td> 
   <td>Elementos de trabajo asignados al equipo o al equipo y una función. </td> 
   <td> <p>Usuarios que son miembros del equipo seleccionado y sus elementos de trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un proyecto</td> 
   <td> <p>En esta área se muestran los elementos de trabajo sin asignar o los elementos asignados a equipos o funciones del proyecto seleccionado.</p> </td> 
   <td> <p>Usuarios asignados al menos a un elemento de trabajo del proyecto seleccionado y sus elementos de trabajo en el proyecto cuando el filtro predeterminado del sistema <b>Elementos de trabajo de este proyecto</b> está seleccionado. </p>

<p>Cuando el filtro predeterminado del sistema <b>Elementos de trabajo de este proyecto</b> no está seleccionado, el área Trabajo asignado de un proyecto mostrará todos los elementos de trabajo de los usuarios asignados al menos a un elemento del proyecto seleccionado.  </p> Este filtro está desactivado de forma predeterminada.

<b>NOTA</b>
<p>Puede habilitar la opción Mostrar todos los usuarios en el Distribuidor de cargas de trabajo de un proyecto para mostrar todos los usuarios del sistema. Para obtener más información, consulte <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navegar por el Distribuidor de cargas de trabajo</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## Crear filtros del Distribuidor de cargas de trabajo

El proceso de creación de filtros para las áreas de Trabajo sin asignar y Trabajo asignado en el Distribuidor de cargas de trabajo es idéntico, independientemente de desde dónde acceda al Distribuidor de cargas de trabajo. Para obtener información sobre cómo localizar el Distribuidor de cargas de trabajo, consulte [Localizar el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Puede crear un filtro desde cero o editar uno de los filtros predefinidos. Para obtener información sobre los filtros existentes que puede editar, consulte la sección [Editar un filtro existente en el Distribuidor de cargas de trabajo](#edit-an-existing-filter-in-the-workload-balancer) de este artículo.

1. Vaya al equilibrador de carga de trabajo.

   Para obtener información sobre el acceso al Distribuidor de cargas de trabajo, consulte [Navegar por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png) en la esquina superior derecha de las áreas **Trabajo sin asignar** o **Trabajo asignado**.

   El cuadro Generador de filtros se muestra a la derecha. El nombre del área para la que crea el filtro se muestra en el encabezado del cuadro.

   ![Lista de filtros](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Opcional y condicional) Si accede al Distribuidor de cargas de trabajo en el área Asignando recursos, es posible que el filtro Predeterminado predefinido ya se haya aplicado al área Trabajo asignado. Puede editar y guardar una copia del filtro predeterminado.

   >[!TIP]
   >
   >El filtro predeterminado muestra los usuarios que pertenecen a cualquiera de sus equipos y sus elementos de trabajo. Puede editar una copia de este filtro.

   Si accede al [!UICONTROL Distribuidor de cargas de trabajo] desde un proyecto, es posible que ya se haya aplicado el filtro “[!UICONTROL Elementos de trabajo de este proyecto]”. Esto muestra solamente los elementos de trabajo asignados a los usuarios de este proyecto. Puede duplicar y guardar una copia de este filtro.

   De manera predeterminada, el [!UICONTROL Distribuidor de cargas de trabajo] de un proyecto muestra todos los elementos de trabajo asignados a todos los usuarios del proyecto.


1. Haga clic en **Nuevo filtro.**

1. Para crear un filtro, haga lo siguiente:

   1. Seleccione un nombre de campo en el primer menú desplegable o haga clic en **Examinar campos** para empezar a escribir el nombre de un campo que no se muestra de forma predeterminada.

      >[!IMPORTANT]
      >
      >Al hacer referencia a campos personalizados, debe escribir el nombre del campo y no la etiqueta del campo. La etiqueta de campo se muestra en un formulario personalizado adjunto a un objeto. Para obtener información acerca de la diferencia entre la etiqueta y el nombre de un campo personalizado, vea [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   1. (Condicional) Si ha hecho clic en **Examinar campos**, escriba el nombre de un campo en el campo **Buscar** y selecciónelo cuando se muestre en la lista.

      ![Buscar un campo](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >Puede seleccionar un campo de las siguientes secciones:
      >
      >* **Selecciones recientes**: los campos para los que ha filtrado recientemente.
      >* **Sugeridos**: los campos más utilizados.


   1. Seleccione un modificador en el segundo menú desplegable. Para obtener información acerca de los modificadores de filtro de Workfront, consulte [Filtros y modificadores de condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Seleccione o escriba un valor para el campo que está filtrando.

      >[!NOTE]
      >
      > Si desea mostrar objetos de trabajo de un portafolio específico, puede aplicar el siguiente filtro: &quot;Portfolio ID es igual a &lt; el nombre del portafolio >&quot;.
      >
      >![Instrucción de filtro de nombre de Portfolio](assets/portfolio-name-filter-statement-wb-350x262.png)
      >
      >Para excluir proyectos en un estado de En espera, debe aplicar el siguiente filtro: &quot;Proyecto: El estado no es igual a En espera&quot;. De este modo se evita que los elementos de trabajo de los proyectos en espera se muestren en el Distribuidor de cargas de trabajo.
      >
      >![Declaración de filtro de estado del proyecto](assets/project-status-filter-statement-wb.png)

   1. (Opcional) Haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png) para quitar un criterio de filtro.

1. (Opcional) Haga clic en **Añadir filtro** para añadir otros criterios de filtro y, a continuación, repita las acciones del paso 4.

   <!--(NOTE: ensure this stays correct)-->

1. Haga clic en **Aplicar** para aplicar los resultados del filtro al área seleccionada del Distribuidor de cargas de trabajo sin guardarlo.

   La lista de elementos de trabajo se actualiza a la izquierda.

   >[!IMPORTANT]
   >
   >Los resultados se muestran en el Distribuidor de cargas de trabajo cuando todas las instrucciones de filtro añadidas son verdaderas simultáneamente.

   El filtro se conserva hasta que se actualiza la página.

   El botón **Aplicar** se ha reemplazado por el botón **Guardar como nuevo**.

1. Haga clic en **Guardar como nuevo** para guardar el filtro y utilizarlo en el futuro.

   ![Filtrar Guardar como](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Si hace clic en **Cancelar** en cualquier momento, volverá al área de creación de filtros.

1. Haga clic dentro del campo **Filtro sin título** e introduzca el nombre del nuevo filtro.
1. (Opcional) Seleccione un icono para el nuevo filtro en el menú desplegable **Icono**.

   ![Seleccionar icono](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Opcional) Añada una descripción del filtro para indicar por qué es único. La descripción se muestra debajo del nombre del filtro en la lista de filtros.
1. Haga clic en **Guardar**.

   Los filtros guardados se muestran en el área Mis filtros del cuadro de filtro.

   Para obtener información acerca de cómo aplicar filtros guardados, consulte la sección [Eliminar un filtro guardado en el Distribuidor de cargas de trabajo](#delete-a-saved-filter-in-the-workload-balancer) de este artículo.

1. (Condicional) Pase el ratón sobre el **icono Filtro** ![Icono de filtro](assets/filter-icon.png) en la esquina superior derecha de las áreas de **Trabajo sin asignar** o **Trabajo asignado** para mostrar información de objeto con el nombre o el número de filtros aplicados actualmente.

   ![Icono de filtro con el nombre del filtro](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Duplicar un filtro

Puede duplicar y editar un filtro para crear uno nuevo.

1. Vaya al equilibrador de carga de trabajo.

   Para obtener información sobre el acceso al Distribuidor de cargas de trabajo, consulte [Navegar por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png) en la esquina superior derecha de las áreas **Trabajo sin asignar** o **Trabajo asignado**.

   El cuadro Generador de filtros se muestra a la derecha. El nombre del área para la que crea el filtro se muestra en el encabezado del cuadro.

1. Pase el cursor sobre un filtro existente, haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Duplicar**.

   ![Filtrar más opciones de menú](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Mientras edita un filtro, puede hacer clic en el menú **Más** en la esquina inferior izquierda del cuadro Editar filtro y luego hacer clic en **Duplicar**.

1. Edite la siguiente información para el filtro duplicado:

   * Nombre

     De forma predeterminada, el nuevo nombre de filtro es “(Nombre del filtro original) Copia”.

   * Icono
   * Descripción
   * Cualquiera de los campos, modificadores o valores.

1. (Opcional) Haga clic en **Añadir filtro** para añadir más instrucciones al filtro duplicado.
1. Haga clic en **Guardar** para guardar el filtro duplicado en el área de **Mis filtros**.

   El filtro original permanece sin cambios y el filtro duplicado se guarda como un nuevo filtro.

## Editar un filtro existente en el Distribuidor de cargas de trabajo {#edit-an-existing-filter-in-the-workload-balancer}

Puede editar un filtro guardado en el Distribuidor de cargas de trabajo.

>[!TIP]
>
>Al editar un filtro compartido con otros usuarios, también verán los cambios que realice.

1. Vaya al equilibrador de carga de trabajo.

   Para obtener información sobre el acceso al Distribuidor de cargas de trabajo, consulte [Navegar por el Distribuidor de cargas de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en el **icono de filtro** ![icono de filtro](assets/filter-icon.png) en la esquina superior derecha de las áreas de **Trabajo sin asignar** o **Trabajo asignado**.\
   El generador de filtros se muestra a la derecha.

1. Pase el ratón sobre el filtro que quiera editar y luego haga clic en el **icono Editar filtro** ![Editar filtro](assets/wb-edit-filter-icon.png).

   ![Filtrar más del menú](assets/filter-more-menu-options-wb.png)

1. Realice una de las siguientes acciones:

   * Modifique cualquiera de las instrucciones del filtro
   * Haga clic en **Agregar filtro** para agregar nuevas instrucciones de filtro
   * Haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png) para eliminar las instrucciones de filtro existentes.

1. (Opcional) Haga clic en **Aplicar**.

   Los resultados se actualizan en el Distribuidor de cargas de trabajo de la izquierda para reflejar los cambios realizados en el filtro.

1. Haga clic en **Guardar**.

   Los resultados se actualizan en el Distribuidor de cargas de trabajo de la izquierda y el filtro se actualiza con la nueva información seleccionada.

## Eliminar un filtro guardado en el Distribuidor de cargas de trabajo {#delete-a-saved-filter-in-the-workload-balancer}

Tenga en cuenta lo siguiente antes de eliminar un filtro:

* Los filtros eliminados no se pueden recuperar.
* Los filtros predefinidos no se pueden eliminar.
* No se puede eliminar un filtro sin guardar. Se eliminan automáticamente después de cerrar la sesión y volver a iniciarla en Workfront.
* Al eliminar un filtro compartido, también se elimina para todos los usuarios con los que se comparte.
* Después de eliminar todos los filtros guardados, el Distribuidor de cargas de trabajo se muestra según los valores predeterminados originales.

>[!NOTE]
>
>Cuando elimine un filtro compartido con otros, también se eliminará para ellos.

1. Vaya al Distribuidor de cargas de trabajo.
1. Haga clic en el **icono Filtro** ![icono Filtro](assets/filter-icon.png) en la esquina superior derecha de las áreas de **Trabajo sin asignar** o **Trabajo asignado**.\
   El cuadro Generador de filtros se muestra a la derecha.

1. Pase el cursor sobre un filtro, luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y luego haga clic en **Eliminar**.
   ![Filtrar más del menú](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Mientras edita un filtro, puede hacer clic en el menú **Más** en la esquina inferior izquierda del cuadro Editar filtro y luego hacer clic en **Eliminar**.

1. (Opcional) Haga clic en **Cancelar** para anular la eliminación y regresar a la lista de filtros.
1. Haga clic en **Eliminar** para confirmar la eliminación.

   El filtro se elimina para usted y todos los usuarios que tenían permisos para utilizarlo.

## Compartir un filtro en el Distribuidor de cargas de trabajo

Puede compartir un filtro que haya creado o que otros usuarios hayan compartido con usted.

Tenga en cuenta lo siguiente al compartir filtros en el Distribuidor de cargas de trabajo:

* Puede compartir filtros con usuarios, equipos, funciones y compañías activos, o bien puede hacerlos visibles para todos los usuarios de la instancia de Workfront.
* Los filtros que comparte en el área Asignando recursos no son visibles en el Distribuidor de cargas de trabajo de un proyecto o equipo.
* Los filtros del Distribuidor de cargas de trabajo que comparte con otros usuarios no son visibles en otras áreas de Workfront.

Para compartir un filtro:

1. Vaya al Distribuidor de cargas de trabajo.
1. Haga clic en el **icono Filtro** ![icono Filtro](assets/filter-icon.png) en la esquina superior derecha de las áreas de **Trabajo sin asignar** o **Trabajo asignado**.\
   El cuadro Generador de filtros se muestra a la derecha.

1. Pase el cursor sobre un filtro, luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Compartir.**

   ![Filtrar más del menú](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Mientras edita un filtro, puede hacer clic en el menú **Más** en la esquina inferior izquierda del cuadro Editar filtro y luego hacer clic en **Compartir**.

   Se muestra el cuadro Compartir filtros.

1. Habilitar la configuración **Ver todo el sistema**. Esto concede permiso a todos los usuarios de Workfront para ver el filtro.

   O

   Empiece a escribir los nombres de los usuarios, equipos, funciones, grupos o compañías con los que desea compartir el filtro en el campo **Conceder acceso a**.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Opcional) Haga clic en la flecha que señala hacia la derecha junto al nombre de una entidad para editar sus permisos en el filtro y, a continuación, habilite la opción **Visualización** o **Administración**.

   ![Permisos de filtro](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Opcional) Habilite o deshabilite los permisos adicionales para una entidad mediante uno de los procedimientos siguientes:

   1. Haga clic en **Visualización** y deshabilite la opción **Compartir**. Está habilitada de forma predeterminada.

   1. Haga clic en **Administración** y deshabilite la opción **Compartir** o **Eliminar**. Están habilitadas de forma predeterminada.

   >[!TIP]
   >
   >Los usuarios no pueden recibir un permiso superior a su nivel de acceso. Si no tienen acceso a Editar filtros en su nivel de acceso, no pueden recibir permisos para administrar un filtro. Workfront deshabilita la opción Administrar para estos usuarios y la opción aparece atenuada.

1. Haga clic en **Compartir**. El filtro se comparte con las entidades especificadas.

   Los filtros que compartió se muestran en el área **Compartido conmigo** del cuadro de filtros.

   ![Shared with me](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![Filter icon](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![Favorites icon](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
