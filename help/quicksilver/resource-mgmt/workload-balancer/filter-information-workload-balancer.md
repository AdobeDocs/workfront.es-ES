---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Filtrar información en el equilibrador de carga de trabajo
description: Para encontrar eficazmente elementos de trabajo y centrarse en los usuarios o elementos que administra, le recomendamos encarecidamente que utilice filtros en el equilibrador de carga de trabajo.
author: Alina
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 10b905c8a66f2507cbfac7c15a01f38d40ab3e00
workflow-type: tm+mt
source-wordcount: '2466'
ht-degree: 0%

---

# Filtrar información en el equilibrador de carga de trabajo

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

Como gestor de recursos, puede utilizar el equilibrador de carga de trabajo para ver y administrar la carga de trabajo de sus usuarios. Para obtener información más general sobre el equilibrador de carga de trabajo, consulte los siguientes artículos:

* [Información general del equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Para encontrar eficazmente elementos de trabajo y centrarse en los usuarios o elementos que administra, le recomendamos encarecidamente que utilice filtros en el equilibrador de carga de trabajo. Esto le permite mostrar la información correcta antes de comenzar a administrar las asignaciones de sus recursos.
>
>Cuando guarda y aplica un filtro nuevo y luego sale del equilibrador de carga de trabajo, el filtro se conserva incluso después de cerrar la sesión y volver a iniciarla.


Este artículo contiene información sobre filtros en el equilibrador de carga de trabajo. Para obtener información sobre los filtros en Workfront, consulte [Información general sobre filtros en Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquier plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, al utilizar el equilibrador de carga de trabajo para un equipo o en el área de recursos </p>
   <p>Trabajar, al utilizar el equilibrador de carga de trabajo de un proyecto </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver o acceso superior a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filtros, vistas y agrupamientos</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Editar acceso a filtros, vistas y grupos al crear o editar filtros</span> </p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores para proyectos, tareas, problemas</p>
   <p>Administre permisos para los filtros que desee editar o eliminar</p>
     </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Información general sobre los filtros en el equilibrador de carga de trabajo

Tenga en cuenta lo siguiente al trabajar con filtros en el equilibrador de carga de trabajo:

* Según desde dónde acceda al equilibrador de carga de trabajo, es posible que Workfront ya esté filtrando la información por usted. Para obtener información sobre los filtros preaplicados, consulte la sección [Filtros preaplicados en el equilibrador de carga de trabajo](#pre-applied-filters-in-the-workload-balancer) en este artículo.
* Puede crear y aplicar un filtro sin guardarlo, o guardar un filtro para reutilizarlo más tarde.
* Al aplicar un filtro sin guardarlo, puede volver a las listas originales actualizando la página.
* Puede ver los filtros que ha creado o los filtros que otros usuarios han creado y compartido con usted.
* Cuando elimina o edita un filtro compartido, también se elimina o edita para todas las personas con las que se comparte.
* Cuando se crean filtros en el equilibrador de carga de trabajo en una zona, no están disponibles en otras áreas.

   Por ejemplo, los filtros creados en el área Recursos no están disponibles en el equilibrador de carga de trabajo de un proyecto o un equipo.

   Para obtener información sobre dónde ubicar el equilibrador de carga de trabajo, consulte [Localizar el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* Puede ver únicamente los elementos que coinciden con los filtros seleccionados que también coinciden con las fechas dentro de la cronología mostradas en la pantalla del equilibrador de carga de trabajo.

## Filtros preaplicados en el equilibrador de carga de trabajo {#pre-applied-filters-in-the-workload-balancer}

El equilibrador de carga de trabajo muestra información en dos áreas independientes:

* **Área de trabajo sin asignar**: elementos de trabajo que aún no están asignados a usuarios.
* **Área de trabajo asignada**: elementos de trabajo asignados a usuarios.

   Para obtener información sobre qué se muestra en cada una de las áreas, consulte [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Cada área del equilibrador de carga de trabajo tiene su propio conjunto de filtros que funcionan de forma independiente entre sí. Debe configurar ambos filtros para indicar qué información desea ver en cada área.

El equilibrador de carga de trabajo muestra usuarios y sus elementos de trabajo.
Los elementos de trabajo asignados a los usuarios solo se muestran cuando las fechas de los elementos coinciden con el lapso de tiempo mostrado en la pantalla.

Según el lugar desde el que acceda al equilibrador de carga de trabajo, las áreas sin asignar y asignadas ya se han filtrado según ciertos criterios, como se describe en la siguiente tabla:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Área de Workfront donde se accede al equilibrador de carga de trabajo</strong></td> 
   <td><b>Elementos que se muestran en el área Trabajo sin asignar de forma predeterminada</b> </td> 
   <td><b>Elementos que se muestran en el área Trabajo asignado de forma predeterminada</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">El área de recursos</td> 
   <td>De forma predeterminada, no se muestra ningún elemento aquí. Debe personalizar los filtros para ver los elementos de trabajo de esta área.</td> 
   <td>Usuarios que son miembros de cualquiera de sus equipos y sus elementos de trabajo. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un equipo</td> 
   <td>Elementos de trabajo asignados al equipo o al equipo y una función de trabajo. </td> 
   <td> <p>Usuarios que son miembros del equipo seleccionado y sus elementos de trabajo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Un proyecto</td> 
   <td> <p>Los elementos de trabajo no asignados o asignados a equipos o funciones de trabajo en el proyecto seleccionado se muestran en esta área.</p> </td> 
   <td> <p>Usuarios asignados a al menos un elemento de trabajo del proyecto seleccionado y sus elementos de trabajo en el proyecto cuando el filtro predeterminado del sistema <b>Elementos de trabajo de este proyecto</b> está seleccionado. </p>

<p>Cuando el filtro predeterminado del sistema <b>Elementos de trabajo de este proyecto</b> no está seleccionada, el área Trabajo asignado de un proyecto muestra todos los elementos de trabajo de los usuarios asignados al menos a un elemento del proyecto seleccionado.  </p> Este filtro está deseleccionado de forma predeterminada.

<b>NOTA</b>
<p>Puede activar la opción Mostrar todos los usuarios en el equilibrador de carga de trabajo de un proyecto para mostrar todos los usuarios del sistema. Para obtener más información, consulte <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navegar por el equilibrador de carga de trabajo</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## Crear filtros del equilibrador de carga de trabajo

El proceso de creación de filtros para las áreas Trabajo no asignado y Trabajo asignado en el equilibrador de carga de trabajo es idéntico, independientemente de desde dónde se acceda al equilibrador de carga de trabajo. Para obtener información sobre cómo localizar el equilibrador de carga de trabajo, consulte [Localizar el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Puede crear un filtro desde cero o editar uno de los filtros predefinidos. Para obtener información sobre los filtros existentes que puede editar, consulte la [Editar un filtro existente en el equilibrador de carga de trabajo](#edit-an-existing-filter-in-the-workload-balancer) en este artículo.

1. Vaya al equilibrador de carga de trabajo.

   Para obtener información sobre el acceso al equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en el **Filtro** icono ![](assets/filter-icon.png) en la esquina superior derecha de **Trabajo no asignado** o **Trabajo asignado** áreas.

   El cuadro Generador de filtros aparece a la derecha. El nombre del área para la que se crea el filtro se muestra en el encabezado del cuadro.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Opcional y condicional) Si accede al equilibrador de carga de trabajo en el área Recursos, es posible que el filtro predeterminado predefinido ya se haya aplicado al área Trabajo asignado. Puede editar y guardar una copia del filtro Predeterminado.

   >[!TIP]
   >
   >El filtro Predeterminado muestra los usuarios que pertenecen a cualquiera de sus equipos y sus elementos de trabajo. Puede editar una copia de este filtro.

   Si accede a la variable [!UICONTROL Equilibrador de carga de trabajo] desde un proyecto, el[!UICONTROL Elementos de trabajo de este proyecto]&quot; puede que ya se haya aplicado. Esto muestra solo los elementos de trabajo asignados a los usuarios de este proyecto. Puede duplicar y guardar una copia de este filtro.

   De forma predeterminada, la variable [!UICONTROL Equilibrador de carga de trabajo] de un proyecto muestra todos los elementos de trabajo asignados a todos los usuarios del proyecto.


1. Haga clic en **Nuevo filtro.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. Para crear un filtro, haga lo siguiente:

   1. Seleccione un nombre de campo en el primer menú desplegable o haga clic en **Campos de exploración** para empezar a escribir el nombre de un campo que no se muestra de forma predeterminada.

      >[!IMPORTANT]
      >
      >Al hacer referencia a campos personalizados, debe escribir el nombre del campo y no la etiqueta del campo. La etiqueta de campo aparece en un formulario personalizado adjunto a un objeto. Para obtener información sobre la diferencia entre la etiqueta y el nombre de un campo personalizado, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (Condicional) Si ha hecho clic en **Campos de exploración**, escriba el nombre de un campo en la **Buscar** y selecciónelo cuando aparezca en la lista.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >Puede seleccionar un campo de las siguientes secciones:
      >
      >* **Selecciones recientes**: los campos para los que ha filtrado recientemente.
      >* **Campos sugeridos**: los campos más utilizados.



   1. Seleccione un modificador en el segundo menú desplegable. Para obtener información sobre los modificadores de filtros de Workfront, consulte [Filtros y modificadores de condición](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Seleccione o escriba un valor para el campo que está filtrando.

      >[!NOTE]
      >
      > Si desea mostrar objetos de trabajo de un portafolio específico, puede aplicar el siguiente filtro: &quot;El nombre del Portfolio contiene marketing.&quot; Se muestran los elementos de trabajo que pertenecen a cualquier portafolio que contenga &quot;marketing&quot; en el nombre.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

   1. (Opcional) Haga clic en el **Eliminar** icono ![](assets/delete.png) para quitar un criterio de filtro.

1. (Opcional) Haga clic en **Añadir filtro** para agregar otro criterio de filtro, repita las acciones del paso 4.

   <!--(NOTE: ensure this stays correct)-->

1. Haga clic en **Aplicar** para aplicar los resultados del filtro al área seleccionada del equilibrador de carga de trabajo sin guardarla.

   La lista de elementos de trabajo se actualiza a la izquierda.

   >[!IMPORTANT]
   >
   >Los resultados se muestran en el equilibrador de carga de trabajo cuando todas las instrucciones de filtro añadidas son verdaderas simultáneamente.

   El filtro se conserva hasta que se actualiza la página.

   La variable **Aplicar** se reemplaza con **Guardar como nuevo** botón.

1. Haga clic en **Guardar como nuevo** para guardar el filtro para uso futuro.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Hacer clic **Cancelar** en cualquier momento, le lleva de nuevo al área de creación de filtros.

1. Select **Filtro sin título** e introduzca el nombre del nuevo filtro en su lugar.
1. Seleccione un icono para el nuevo filtro en el **Icono** menú desplegable.

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Opcional) Añada una descripción para el filtro para indicar qué es lo único que tiene al respecto. La descripción se muestra bajo el nombre del filtro en la lista de filtros.
1. Haga clic en **Guardar**.

   Los filtros guardados se muestran en el área Mis filtros del cuadro de filtro.

   Para obtener información sobre la aplicación de filtros guardados, consulte la sección [Eliminar un filtro guardado en el equilibrador de carga de trabajo](#delete-a-saved-filter-in-the-workload-balancer) en este artículo.

1. (Condicional) Pase el ratón sobre el **Icono de filtro** ![](assets/filter-icon.png) en la esquina superior derecha del **Trabajo no asignado** o **Trabajo asignado** áreas para mostrar una información del objeto con el nombre o el número de filtros que se están aplicando actualmente.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Duplicar un filtro

Puede duplicar y editar un filtro para crear uno nuevo.

1. Vaya al equilibrador de carga de trabajo.

   Para obtener información sobre el acceso al equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en el **Filtro** icono ![](assets/filter-icon.png) en la esquina superior derecha de **Trabajo no asignado** o **Trabajo asignado** áreas.

   El cuadro Generador de filtros se muestra a la derecha. El nombre del área para la que se crea el filtro se muestra en el encabezado del cuadro.

1. Pase el ratón sobre un filtro existente y haga clic en la **Más** menú ![](assets/more-menu.png)y haga clic en **Duplicar**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Durante la edición de un filtro, puede hacer clic en el botón **Más** en la esquina inferior izquierda del cuadro Editar filtro y, a continuación, haga clic en **Duplicar**.

1. Edite la siguiente información para el filtro duplicado:

   * Nombre

      De forma predeterminada, el nuevo nombre de filtro es &quot;(Nombre del filtro original) Copiar.&quot;

   * Icono
   * Descripción
   * Cualquiera de los campos, modificadores o valores.

1. (Opcional) Haga clic en **Añadir filtro** para agregar más instrucciones al filtro duplicado.
1. Haga clic en **Guardar** para guardar el filtro duplicado en el **Mis filtros** .

   El filtro original permanece sin cambios y el filtro duplicado se guarda como un nuevo filtro.

## Editar un filtro existente en el equilibrador de carga de trabajo {#edit-an-existing-filter-in-the-workload-balancer}

Puede editar un filtro guardado en el equilibrador de carga de trabajo.

>[!TIP]
>
>Al editar un filtro compartido con otros, también verán los cambios que realice.

1. Vaya al equilibrador de carga de trabajo.

   Para obtener información sobre el acceso al equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Haga clic en el **Icono de filtro** ![](assets/filter-icon.png) en la esquina superior derecha del **No asignado** o **Trabajo asignado** áreas.\
   El generador de filtros aparece a la derecha.

1. Pase el cursor sobre el filtro que desee editar y, a continuación, haga clic en la **Editar** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. Realice una de las siguientes acciones:

   * Modificar cualquiera de las instrucciones de filtro
   * Haga clic en **Añadir filtro** adición de nuevas instrucciones de filtro
   * Haga clic en el **Eliminar** icono ![](assets/delete.png) para quitar instrucciones de filtro existentes.

1. (Opcional) Haga clic en **Aplicar**.

   Los resultados se actualizan en el equilibrador de carga de trabajo de la izquierda para ilustrar los cambios realizados en el filtro.

1. Haga clic en **Guardar.**

   Los resultados se actualizan en el equilibrador de carga de trabajo a la izquierda y el filtro se actualiza con la nueva información seleccionada.

## Eliminar un filtro guardado en el equilibrador de carga de trabajo {#delete-a-saved-filter-in-the-workload-balancer}

Tenga en cuenta lo siguiente antes de eliminar un filtro:

* No se pueden recuperar los filtros eliminados.
* Los filtros predefinidos no se pueden eliminar.
* No se puede eliminar un filtro sin guardar. Se eliminan automáticamente después de cerrar la sesión y volver a iniciarla en Workfront.
* Cuando elimina un filtro compartido, también se elimina para todos los usuarios con los que se comparte.
* Después de eliminar todos los filtros guardados, el equilibrador de carga de trabajo se muestra según los valores predeterminados originales.

>[!NOTE]
>
>Cuando elimine un filtro compartido con otros, también se eliminará para ellos.

1. Vaya al equilibrador de carga de trabajo
1. Haga clic en el **Icono de filtro** ![](assets/filter-icon.png) en la esquina superior derecha del **Trabajo no asignado** o **Trabajo asignado** áreas.\
   El cuadro Generador de filtros aparece a la derecha.

1. Pase el ratón sobre un filtro y, a continuación, haga clic en el botón **Más** menú ![](assets/more-menu.png)y haga clic en **Eliminar**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Durante la edición de un filtro, puede hacer clic en el botón **Más** en la esquina inferior izquierda del cuadro Editar filtro y, a continuación, haga clic en **Eliminar**.

1. (Opcional) Haga clic en **Cancelar** para evitar la eliminación y volver a la lista de filtros.
1. Haga clic en **Eliminar** para confirmar la eliminación.

   El filtro se elimina para usted y para todos los usuarios que tengan permisos para él.

## Uso compartido de un filtro en el equilibrador de carga de trabajo

Puede compartir un filtro que haya creado o que otros usuarios hayan compartido con usted.

Tenga en cuenta lo siguiente al compartir filtros en el equilibrador de carga de trabajo:

* Puede compartir filtros con usuarios, equipos, funciones y empresas activos, o puede hacerlos visibles para todos en la instancia de Workfront.
* Los filtros que comparta en el área Recursos no son visibles en el equilibrador de carga de trabajo de un proyecto o equipo.
* Los filtros del equilibrador de carga de trabajo que comparta con otros no son visibles en otras áreas de Workfront.

Para compartir un filtro:

1. Vaya al equilibrador de carga de trabajo
1. Haga clic en el **Icono de filtro** ![](assets/filter-icon.png) en la esquina superior derecha del **Trabajo no asignado** o **Trabajo asignado** áreas.\
   El cuadro Generador de filtros aparece a la derecha.

1. Pase el ratón sobre un filtro y, a continuación, haga clic en el botón **Más** menú ![](assets/more-menu.png)y haga clic en **Compartir.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Durante la edición de un filtro, puede hacer clic en el botón **Más** en la esquina inferior izquierda del cuadro Editar filtro y, a continuación, haga clic en **Compartir**.

   Se muestra el cuadro Compartir filtros .

1. Active la variable **Ver todo el sistema** configuración. Esto da permiso a cualquier usuario de Workfront para ver el filtro.

   O

   Comience a escribir los nombres de los usuarios, equipos, funciones, grupos o empresas con los que desee compartir el filtro en la **Dar acceso a** campo .

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Opcional) Haga clic en la flecha que apunta a la derecha junto al nombre de una entidad para editar sus permisos para el filtro y, a continuación, active la opción **Ver** o **Administrar** .

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Opcional) Habilite o deshabilite los permisos adicionales para una entidad haciendo una de las siguientes acciones:

   1. Haga clic en **Ver** y deshabilite **Compartir** . Está activada de forma predeterminada.

   1. Haga clic en **Administrar** y deshabilite **Compartir** o **Eliminar** . Están activados de forma predeterminada.
   >[!TIP]
   >
   >Los usuarios no pueden recibir permisos superiores a su nivel de acceso. Si no tienen acceso a los filtros de edición en su nivel de acceso, no pueden recibir permisos para administrar un filtro. Workfront deshabilita la opción Administrar para estos usuarios y la opción está atenuada.

1. Haga clic en **Compartir**. El filtro se comparte con las entidades especificadas.

   Los filtros que ha compartido se muestran en la **Compartido conmigo** del cuadro de filtro.

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
