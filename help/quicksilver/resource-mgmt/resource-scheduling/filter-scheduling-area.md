---
product-area: resource-management
navigation-topic: resource-scheduling
title: Filtrado de información en el área Programación
description: El uso de un filtro en el área Programación de recursos permite determinar qué elementos de trabajo se muestran en la cronología de programación. Esto incluye qué tareas y problemas se muestran en el área Sin asignar, así como qué usuarios se muestran.
author: Alina
feature: Resource Management
exl-id: 974b2515-ed10-459d-a317-36e62c52afc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2452'
ht-degree: 0%

---

# Filtrado de información en el área Programación

>[!IMPORTANT]
>  
><span class="preview">La funcionalidad Programación descrita en este artículo se ha desaprobado y eliminado de Adobe Workfront a partir de la versión 23.1 de enero de 2023.   </span>
>  
> <span class="preview"> Este artículo también se eliminará poco después de la versión 23.1, a principios de 2023. En este momento, le recomendamos que actualice los marcadores según corresponda. </span>
> 
><span class="preview"> Ahora puede utilizar el equilibrador de carga de trabajo para programar el trabajo para sus recursos. </span>
>  
> <span class="preview">Para obtener información sobre la programación de recursos mediante el equilibrador de carga de trabajo, consulte la sección [El equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<p>(SEVERAL SECTIONS BELOW LINKED TO THE PRODUCT. SEE NOTES</p>
-->

El uso de un filtro en el área Programación de recursos permite determinar qué elementos de trabajo se muestran en la cronología de programación. Esto incluye qué tareas y problemas se muestran en el área Sin asignar, así como qué usuarios se muestran.

Antes de comenzar a filtrar el contenido como se describe en esta sección, familiarícese con el funcionamiento de la programación de recursos en Adobe Workfront.\
Para obtener información sobre la programación de recursos en Workfront, consulte el artículo [Introducción a la programación de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).\
Para obtener más información sobre la cronología de la programación, consulte el artículo [Introducción a la programación de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

Puede programar recursos o un equipo individual del que sea miembro o para cualquier proyecto para el que sea administrador de recursos.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Ver acceso o superior a Proyectos, tareas y problemas</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos o superiores para proyectos, tareas y problemas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

<!--
<p>(NOTE: sections below - LINKED TO THE ui. DO NOT RENAME/ DELETE)</p>
-->

## Crear un filtro en la sección Programación (para equipos)

Las tareas y los problemas de los proyectos, usuarios y funciones que defina en el filtro se muestran en la cronología de programación de la pestaña Trabajar en . Utilice las opciones del filtro para determinar qué proyectos, usuarios y funciones se representan en la cronología de programación.

>[!NOTE]
>
>No puede guardar un filtro en la ficha Trabajar en (para un equipo). Cuando actualiza la página o sale de ella, el filtro vuelve a la configuración predeterminada.

Para crear un filtro para la cronología de programación en la ficha Trabajo en los equipos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Equipos**, seleccione un equipo, haga clic en **Equilibrador de carga de trabajo** en el panel izquierdo, seleccione **Programación** en el menú desplegable superior izquierdo.
1. Haga clic en **Filtro**.
1. Determine qué proyectos están representados en el área No asignado especificando la siguiente información:

   <!--
   <p>(NOTE: Alina: there was a note that [This step is linked to from the context-sensitive help] but I could not find from where in the UI it is linked.)&nbsp;</p>
   -->

   * **Prioridades del proyecto:** Seleccione la prioridad de los proyectos que desea que se representen en la cronología de programación. Las tareas y los problemas de los proyectos con las prioridades seleccionadas se muestran en la cronología de programación.\
      En este menú solo están disponibles las prioridades de los proyectos que incluyen tareas o problemas asignados al equipo.
   * **Estados del proyecto:** Seleccione el estado de los proyectos que desea que se representen en la cronología de programación. Las tareas y los problemas de los proyectos con los estados seleccionados se muestran en la cronología de programación.\
      En este menú solo están disponibles los estados de proyectos que incluyen tareas o problemas asignados al equipo.
   * **Proyectos:** Seleccione los proyectos que desee que se representen en la cronología de programación. Las tareas y los problemas de los proyectos seleccionados se muestran en la cronología de la programación.\
      Las selecciones en los campos anteriores determinan los proyectos que se pueden seleccionar.\
      Solo los proyectos que incluyen tareas o problemas asignados al equipo están disponibles para elegir en este menú.

1. Determine qué usuarios se muestran en la cronología de programación especificando la siguiente información. De forma predeterminada, se muestran todos los integrantes del equipo.

   <!--
   <p>(NOTE: this step is linked in the UI.)</p>
   -->

   * **Funciones:** Seleccione las funciones que desea que se representen en la cronología de programación.\
      En el área Sin asignar solo se muestran las tareas asignadas a esa función. Solo se muestran los usuarios con las funciones que seleccione que puedan asignarse a esas tareas.\
      Los usuarios se muestran en la cronología de la programación, organizados por función del trabajo.
   * **Usuarios:** Seleccione los usuarios individuales que desea que se representen en la cronología de programación.\
      Solo se muestran los usuarios seleccionados, independientemente de si tienen una asignación de función que coincida con la asignación de funciones de tareas del área No asignado.\
      Esta opción no afecta a las tareas y los problemas que se muestran en el área No asignado.

      <!--   
     <p>(NOTE: Alina: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])</p>   
     -->

1. (Opcional) Para realizar más modificaciones en la cronología de la programación (como cambiar el intervalo de fechas) y para realizar modificaciones en las asignaciones de usuarios, consulte el artículo [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

<!--
<p>(NOTE: below - LINKED TO THE UI, DO NOT RENAME/ DELETE/ CHANGE)</p>
-->

## Crear y modificar filtros en la sección Programación (para varios proyectos)

Puede crear un filtro nuevo, aplicar un filtro que haya creado anteriormente, modificar un filtro que haya creado anteriormente o eliminar un filtro. No puede compartir filtros que cree con otros usuarios.

* [Crear un filtro en la sección Programación (para proyectos)](#create-a-filter-in-the-scheduling-section-for-projects)
* [Aplicar un filtro guardado](#apply-a-saved-filter)
* [Modificación de un filtro guardado](#modify-a-saved-filter)
* [Eliminar un filtro guardado](#delete-a-saved-filter)

### Crear un filtro en la sección Programación (para proyectos) {#create-a-filter-in-the-scheduling-section-for-projects}

<!--
<p>(NOTE: *****LINKED TO THE PRODUCT FROM THE GLOBAL SCHEDULER >> BOTH THE FIRST AND THE SECOND AREAS) </p>
-->

Las tareas y los problemas de los proyectos, usuarios y funciones que defina en el filtro se muestran en la cronología de programación en la pestaña Programación . Utilice las opciones del filtro para determinar qué proyectos, usuarios y funciones se representan en la cronología de programación.

Para crear un filtro para la cronología de programación en la ficha Programación de varios proyectos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
1. Haga clic en **Filtro**.\
   ![](assets/scheduling-filter-350x351.png)

1. Deje el **Filtros guardados** campo en blanco.
1. Determine qué proyectos están representados en el área No asignado especificando la siguiente información:

   <!--
   <p>(NOTE: Alina: this step is linked in the UI.) </p>
   -->

   * **Portfolio:** Seleccione cualquier portafolios que incluya programas y proyectos que desee que se representen en la cronología de programación.

      Solo los programas dentro de los portafolios que seleccione estarán disponibles para seleccionarlos en la **Programa** campo .

   * **Programas:** Seleccione cualquier programa que incluya proyectos que desee que se representen en la cronología de programación.\
      Las selecciones en la **Portfolio** determine los programas que están disponibles para seleccionar.\
      Solo los proyectos dentro de los programas que seleccione estarán disponibles para seleccionarlos en la **Proyectos** campo .

   * **Prioridades del proyecto:** Seleccione la prioridad de los proyectos que desea que se representen en la cronología de programación.\
      Solo se representan los proyectos con las prioridades seleccionadas.

   * **Estados del proyecto:** Seleccione el estado de los proyectos que desea que se representen en la cronología de programación.\
      Solo se representan los proyectos con los estados seleccionados.

   * **Compañías de proyectos:** Las tareas y los problemas se muestran en la cronología de la programación solo cuando pertenecen a un proyecto que coincide con la empresa seleccionada.

   * **Grupos de proyectos:** Las tareas y los problemas se muestran en la cronología de la programación solo cuando pertenecen a un proyecto que coincide con un grupo seleccionado.

   * **Proyectos:** Seleccione los proyectos que desee que se representen en la cronología de programación. Las tareas y los problemas de los proyectos seleccionados se muestran en la cronología de la programación.\
      Las selecciones en los campos anteriores determinan los proyectos que se pueden seleccionar.\
      Las tareas y los problemas de los proyectos seleccionados se muestran en la cronología de la programación. Solo los proyectos que incluyen tareas o problemas asignados al equipo están disponibles para elegir en este menú.

1. Determine qué usuarios se muestran en la cronología de programación especificando la siguiente información: (De forma predeterminada, solo se muestran los usuarios que cumplen los requisitos para recibir una tarea o un problema desde el área Sin asignar. Al seleccionar usuarios individuales, los usuarios se muestran en la cronología de la programación independientemente de si cumplen los requisitos para recibir una tarea o un problema del área No asignada). 

   <!--
   <p>(NOTE: Alina: this step had a note that it is linked in the UI but I could not find from where.) </p>
   -->

   * **Compañías de usuarios:** Este campo permite restringir la visualización de usuarios de otras empresas en la cronología de la programación.\
      Deje este campo vacío si desea agregar usuarios de cualquier empresa. Si especifica empresas individuales, solo se pueden agregar usuarios de esas empresas a la cronología de la programación. Al especificar una empresa, no se agregan automáticamente usuarios de esa empresa a la cronología de programación. En su lugar, utilice los campos siguientes para añadir usuarios específicos.\
      Esta opción no afecta a las tareas y los problemas que se muestran en el área No asignado.****

   * **Grupos de usuarios:** Todos los usuarios de cualquier grupo de usuarios que especifique se mostrarán en la cronología de la programación.

   * **Equipos:** Todos los usuarios de cualquier equipo que especifique se mostrarán en la cronología de la programación.\
      Esta opción no afecta a las tareas y los problemas que se muestran en el área No asignado.

   * **Funciones:** Seleccione las funciones que desea que se representen en la cronología de programación.\
      En el área Sin asignar solo se muestran las tareas asignadas a esa función. Solo se muestran los usuarios con las funciones que seleccione que puedan asignarse a esas tareas.\
      Los usuarios se muestran en la cronología de la programación, organizados por función del trabajo.

   * **Usuarios:** Seleccione los usuarios individuales que desea que se representen en la cronología de programación.\
      Solo se muestran los usuarios seleccionados, independientemente de si tienen una asignación de función que coincida con la asignación de funciones de tareas del área No asignado.\
      Esta opción no afecta a las tareas y los problemas que se muestran en el área No asignado.
   <!--
   <p>NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->

1. Haga clic en **Guardar nuevo filtro**.\
   Los datos se muestran en la cronología de la programación.

1. (Opcional) Para realizar más modificaciones en la cronología de la programación (como cambiar el intervalo de fechas) y para realizar modificaciones en las asignaciones de usuarios, consulte el artículo [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Aplicar un filtro guardado {#apply-a-saved-filter}

>[!NOTE]
>
>Esta opción solo se aplica cuando se programan recursos para varios proyectos (desde la pestaña Scheduling ); no se puede aplicar un filtro guardado al programar recursos para un equipo (en la pestaña Trabajar en ) o al programar recursos para un único proyecto (en la pestaña Dotación de personal ).

Puede aplicar un filtro que haya creado anteriormente.

Para aplicar un filtro guardado a varios proyectos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
1. Haga clic en **Filtro**.
1. En el **Filtros guardados** , seleccione el filtro que desee aplicar.\
   Los datos se muestran en la cronología de la programación.

1. (Opcional) Para realizar más modificaciones en la cronología de la programación (como cambiar el intervalo de fechas) y para realizar modificaciones en las asignaciones de usuarios, consulte el artículo [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Modificación de un filtro guardado {#modify-a-saved-filter}

>[!NOTE]
>
>Esta opción solo se aplica cuando se programan recursos para varios proyectos (desde la pestaña Scheduling ); no se puede modificar un filtro guardado al programar recursos para un equipo (en la pestaña Trabajar en ) o al programar recursos para un único proyecto (en la pestaña Dotación de personal ).

Puede modificar un filtro que haya creado anteriormente.

Para modificar un filtro guardado para varios proyectos:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
1. Haga clic en **Filtro**.
1. En el **Filtros guardados** , seleccione el filtro que desee modificar en la lista desplegable.
1. Especifique qué datos mostrar en la cronología de programación.
1. Haga clic en **Guardar**.\
   Los datos se muestran en la cronología de la programación.

1. (Opcional) Para realizar más modificaciones en la cronología de la programación (como cambiar el intervalo de fechas) y para realizar modificaciones en las asignaciones de usuarios, consulte el artículo [Asignación manual de tareas y problemas no asignados en las áreas de programación](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Eliminar un filtro guardado {#delete-a-saved-filter}

>[!NOTE]
Esta opción solo se aplica cuando se programan recursos para varios proyectos (desde la pestaña Scheduling ); no se puede eliminar un filtro guardado al programar recursos para un equipo (en la pestaña Trabajar en ) o al programar recursos para un solo proyecto (en la pestaña Dotación de personal ).

Puede eliminar un filtro que haya creado anteriormente.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
1. Haga clic en **Filtro**.
1. En el **Filtros guardados** , en la lista desplegable , haga clic en (x) junto al filtro que desea eliminar. 

## Crear y modificar filtros en la sección Programación (para un solo proyecto)

<!--
<p>(NOTE: **** LINKED FROM THE PRODUCT FROM THE PROJECT> STAFFING> SCHEDULING AREA) </p>
-->

Las tareas y los problemas de los usuarios, equipos y funciones que defina en el filtro se muestran en la cronología de programación de la pestaña Dotación de personal. Utilice las opciones del filtro para determinar qué usuarios, equipos y funciones están representados en la cronología de programación.

>[!NOTE]
No se puede guardar un filtro en la ficha Dotación de personal (para un solo proyecto). Cuando actualiza la página o sale de ella, el filtro vuelve a la configuración predeterminada.

Para crear un filtro para la cronología de programación en la ficha Dotación de personal para un solo proyecto:

1. Vaya a un proyecto y haga clic en el **Equilibrador de carga de trabajo** del panel izquierdo y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
1. Determine qué usuarios se muestran en la cronología de programación especificando la siguiente información: (De forma predeterminada, solo se muestran los usuarios que cumplen los requisitos para recibir una tarea o un problema desde el área Sin asignar. Al seleccionar usuarios individuales, los usuarios se muestran en la cronología de la programación independientemente de si cumplen los requisitos para recibir una tarea o un problema del área No asignada). 

   <!--
   <p><span>(NOTE: Alina: [This step is linked to from the context-sensitive help]) </span> </p>
   -->

   * **Compañías de usuarios:** Este campo permite restringir la visualización de usuarios de otras empresas en la cronología de la programación.\
      Deje este campo vacío si desea agregar usuarios de cualquier empresa. Si especifica empresas individuales, solo se pueden agregar usuarios de esas empresas a la cronología de la programación. Al especificar una empresa, no se agregan automáticamente usuarios de esa empresa a la cronología de programación. En su lugar, utilice los campos siguientes para añadir usuarios específicos.\
      Esta opción no afecta a las tareas y los problemas que se muestran en el área No asignado.

   * **Grupos de usuarios:** Todos los usuarios de cualquier grupo de usuarios que especifique se mostrarán en la cronología de la programación.

   * **Equipos:** Todos los usuarios de cualquier equipo que especifique se mostrarán en la cronología de la programación.\
      Esta opción no afecta a las tareas y los problemas que se muestran en el área No asignado.

   * **Funciones:** Seleccione las funciones que desea que se representen en la cronología de programación.\
      En el área Sin asignar solo se muestran las tareas asignadas a esa función. Solo se muestran los usuarios con las funciones que seleccione que puedan asignarse a esas tareas.\
      Los usuarios se muestran en la cronología de la programación, organizados por función del trabajo.

   * **Usuarios:** Seleccione los usuarios individuales que desea que se representen en la cronología de programación.\
      Solo se muestran los usuarios seleccionados, independientemente de si tienen una asignación de función que coincida con la asignación de funciones de tareas del área No asignado.\
      Esta opción no afecta a las tareas y los problemas que se muestran en el área No asignado.
   <!--
   <p>(NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->
