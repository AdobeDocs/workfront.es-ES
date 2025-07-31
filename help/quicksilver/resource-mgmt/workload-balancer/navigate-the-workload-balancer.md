---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Navegar por el equilibrador de carga de trabajo
description: Utilice el Distribuidor de cargas de trabajo para comprender la disponibilidad de sus recursos, así como para asignar trabajo a los usuarios. Este artículo le guía mediante los iconos y la configuración disponibles para actualizar la vista del Distribuidor de cargas de trabajo y desplazarse por él.
author: Lisa
feature: Resource Management
exl-id: 60dabfc5-6a2e-4368-9dac-db48d0307895
source-git-commit: 2d674504274dcbb4a44da80694fac331d3f17d88
workflow-type: tm+mt
source-wordcount: '4271'
ht-degree: 8%

---

# Navegar por el equilibrador de carga de trabajo

{{preview-fast-release-general}}

<!--Audited: 12/2024-->

Utilice el Distribuidor de cargas de trabajo en Adobe Workfront para asignar trabajo a los usuarios en función de su disponibilidad. Este artículo describe cómo puede utilizar la configuración y las opciones para desplazarse por el Distribuidor de cargas de trabajo y mostrar la información que le interesa. Los artículos adicionales que se enumeran aquí describen cómo puede utilizar el Distribuidor de cargas de trabajo para administrar los recursos y su asignación al trabajo.

El Distribuidor de cargas de trabajo está disponible en varias áreas de Adobe Workfront. La navegación es similar en todas las áreas.

Para obtener más información sobre dónde se encuentra el Distribuidor de cargas de trabajo, consulte [Localizar el Distribuidor de cargas de trabajo](https://experienceleague.adobe.com/es/docs/workfront/using/manage-resources/the-workload-balancer/locate-workload-balancer).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
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
    </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Ver o permisos superiores en los proyectos, tareas y problemas</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones para la visualización de elementos en el Distribuidor de cargas de trabajo

Tenga en cuenta lo siguiente al ver el Distribuidor de cargas de trabajo:

* El Distribuidor de cargas de trabajo muestra los elementos de trabajo en dos áreas independientes, según sus asignaciones. Los elementos de trabajo y los usuarios se muestran en las siguientes áreas:

   * **Trabajo sin asignar**: elementos que no tienen asignaciones o que se asignan solamente a roles o equipos de trabajo.
   * **Trabajo asignado**: elementos asignados al menos a un usuario. Los elementos asignados se muestran bajo el nombre del usuario asignado.

  >[!NOTE]
  >
  >* Los elementos de trabajo asignados a un rol o a un equipo, y también asignados a un usuario, se muestran en el área de Trabajo no asignado y bajo el nombre del usuario asignado en el área de Trabajo asignado.
  >* Los elementos de trabajo asignados a un usuario y a un rol, donde el rol está seleccionado como el principal asignado del elemento, se muestran en el área de Trabajo no asignado.
  >* Los elementos de trabajo asignados a más de un usuario se muestran con todos los nombres de usuarios asignados en el área Trabajo asignado.
  >* <span class="preview">Las asignaciones de rol se muestran en elementos de trabajo en el área de trabajo no asignado cuando la opción Mostrar asignaciones de rol está habilitada. Para obtener más información, consulte la sección [Personalizar la vista](#customize-the-view) en este artículo.</span>

  Para obtener más información, consulte [Áreas de asignación en el Distribuidor de cargas de trabajo](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md#assignment-areas-in-the-workload-balancer) en [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](/help/quicksilver/resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

* Cuando un proyecto no tiene tareas durante un período de tiempo, la barra en el nivel de proyecto está en blanco para ese período de tiempo.

  ![Proyecto sin tareas durante un período de tiempo](assets/wb-no-tasks-in-time-period.png)

* Cuando no tiene permisos para ver ciertos elementos, se muestran como **elementos de trabajo inaccesibles** o **proyectos inaccesibles**.

  ![Elementos de trabajo inaccesibles](assets/wb-inaccessible-work-items.png)

* Los nombres de los elementos de trabajo se muestran a la izquierda y su cronología, a la derecha.
* El total de horas planificadas para cada elemento de trabajo se muestra a la derecha del nombre del elemento de trabajo y a la izquierda de la barra que representa la cronología del elemento de trabajo.
* El total de horas planificadas para cada proyecto se muestra a la derecha del nombre del proyecto y a la izquierda de la barra que representa la cronología del proyecto.

  La información de horas planificadas para el proyecto es un total de horas planificadas de todos los elementos enumerados en el Distribuidor de cargas de trabajo, y no un total de horas planificadas en el proyecto.

Para obtener más información sobre la visualización de información en el Distribuidor de cargas de trabajo, consulte los siguientes artículos:

* [Buscar el Distribuidor de cargas de trabajo](../workload-balancer/locate-workload-balancer.md)
* [Filtrar información en el distribuidor de cargas de trabajo](../workload-balancer/filter-information-workload-balancer.md)
* [Uso compartido del Distribuidor de cargas de trabajo con un vínculo](../workload-balancer/share-link-for-workload-balancer.md)
* [Actualizar elementos de trabajo en el Distribuidor de cargas de trabajo mediante el resumen](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

Para obtener información sobre la administración de recursos mediante el Distribuidor de cargas de trabajo, consulte también los siguientes artículos:

* [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](https://experienceleague.adobe.com/es/docs/workfront/using/manage-resources/the-workload-balancer/assign-work-in-workload-balancer)
* [Administrar asignaciones de usuario en el Distribuidor de cargas de trabajo](https://experienceleague.adobe.com/es/docs/workfront/using/manage-resources/the-workload-balancer/manage-user-allocations-workload-balancer)


## Vaya al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos

La navegación del Distribuidor de cargas de trabajo es similar en todas las áreas desde las que se accede a él.

Las siguientes subsecciones describen cómo ver la información en el Distribuidor de cargas de trabajo para varios proyectos.

Puede ajustar una serie de configuraciones y opciones en el Distribuidor de cargas de trabajo para mostrar la información en la que debe centrarse en el lapso de tiempo que le resulte más sensato.

Después de seleccionar la configuración que desea aplicar a la vista, el Distribuidor de cargas de trabajo recuerda esta configuración cada vez que accede a ella desde cualquier explorador o dispositivo.

### Acceso al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos

Para desplazarse por el Distribuidor de cargas de trabajo para varios proyectos:

{{step1-to-resourcing}}

1. Haga clic en **Distribuidor de cargas de trabajo** en el panel de la izquierda.

   ![Distribuidor de cargas de trabajo](assets/nwe-balancer-global.png)

   El Distribuidor de cargas de trabajo muestra información sobre la asignación de trabajo a partir de la semana actual en las dos áreas siguientes:

   * El área **Trabajo sin asignar** muestra los siguientes elementos de trabajo:

      * Los elementos de trabajo (tareas y problemas) asignados a funciones, equipos o usuarios sin asignar se muestran después de aplicar los filtros.
El área de Trabajo no asignado no muestra ningún elemento de trabajo de forma predeterminada. Se recomienda utilizar filtros para mostrar información relevante en esta área.

        Para obtener información sobre el uso de filtros, consulte [Información sobre filtros en el Distribuidor de cargas de trabajo](../workload-balancer/filter-information-workload-balancer.md).

      * <span class="preview">Las asignaciones de roles en los elementos de trabajo solo se muestran cuando habilita la opción Mostrar asignaciones de roles. Para obtener más información, consulte la sección [Personalizar la vista](#customize-the-view) en este artículo.</span>

      * Los proyectos solo se muestran cuando se habilita la configuración Agrupar por proyecto. Para obtener más información, consulte la sección [Personalizar la vista](#customize-the-view) en este artículo.

   * El área **Trabajo asignado** muestra los siguientes elementos de trabajo:

      * De forma predeterminada, todos los usuarios activos del sistema se muestran en esta área. Se recomienda utilizar filtros para limitar la cantidad de información en esta área. Si los usuarios están asignados a elementos, los elementos de trabajo también se muestran bajo su nombre.

      * Las tareas y los problemas asignados al menos a un usuario se muestran bajo el nombre del usuario.

        Los elementos de trabajo bajo los nombres de los usuarios en el área Trabajo asignado se ordenan según los siguientes criterios, en este orden:

         1. Fecha planificada de inicio (la más antigua primero)
         1. Fecha planificada de finalización (la más antigua primero)
         1. Alfabético por proyecto (solo cuando los dos primeros criterios son idénticos para varios elementos de trabajo)

            >[!TIP]
            >
            >* Puede personalizar la ordenación del proyecto seleccionando una opción en la configuración Ordenar proyectos por.
            >
            >* Los proyectos solo se muestran cuando se habilita la configuración Agrupar por proyecto.
            > 
            >Para obtener información acerca de cómo personalizar la configuración, vea la sección [Personalizar la vista](#customize-the-view) en este artículo.

1. (Opcional) Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png) en el área de **Trabajo asignado** y, a continuación, seleccione el **Filtro predeterminado** en el área **Sugerido** del cuadro de filtro.

   Al aplicar el filtro Predeterminado, se muestran los usuarios que pertenecen a cualquiera de sus equipos y sus elementos de trabajo. Puede editar una copia de este filtro.

   >[!TIP]
   >
   >El filtro predeterminado solo está disponible en el Distribuidor de cargas de trabajo en el área de Recursos.

1. Continúe con los siguientes pasos para navegar por el Distribuidor de cargas de trabajo:

   * [Seleccione un lapso de tiempo en el Distribuidor de cargas de trabajo](#select-a-time-frame-in-the-workload-balancer)
   * [Personalizar la vista](#customize-the-view)
   * [Asignar elementos de trabajo y ajustar las asignaciones de usuario](#assign-work-items-and-adjust-user-allocations)
   * [Visualización de asignaciones en un gráfico](#view-allocations-in-a-chart)

### Seleccione un lapso de tiempo en el Distribuidor de cargas de trabajo

1. Acceda al Distribuidor de cargas de trabajo en el área **Recursos**, tal como se describe en la sección [Acceso al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) en este artículo.

   El distribuidor de cargas de trabajo muestra información sobre la asignación de trabajo a partir de la semana actual.

1. Utilice el desplazamiento horizontal para ver la cronología de los elementos de trabajo que sobrepasan los límites de la pantalla.
1. Haga clic en los iconos **atrás o adelante** ![Iconos atrás y adelante](assets/back-and-forward-icons.png) en la esquina superior izquierda para navegar por la cronología y, a continuación, haga clic en **Hoy** para regresar a la semana actual.
1. Haga clic en el menú desplegable **lapso de tiempo** de la barra de herramientas y, a continuación, haga clic en la fecha de comienzo del período que desee mostrar. De forma predeterminada, la primera semana seleccionada en el calendario es la semana a la que ha navegado.

   ![Selección de calendario](assets/calendar-date-picker-wb.png)

1. Seleccione el número de semanas que desea mostrar al mismo tiempo en el Distribuidor de cargas de trabajo de las siguientes opciones:
   * 1 semana
   * 2 semanas
   * 4 semanas. Esta es la configuración predeterminada.
   * 6 semanas
   * 3 meses

   ![Seleccionar semanas](assets/3-months-12-weeks-drop-down-wb.png)

1. Haga clic en una de las siguientes opciones de la barra de herramientas para mostrar información por intervalos de tiempo diferentes:
   * **Día**: muestra información por día durante cuatro semanas a partir de la fecha actual, de forma predeterminada.
   * **Semana**: muestra información por semana durante cuatro semanas.
   * **Mes**: muestra información por mes durante tres meses.

1. Continúe navegando por el Distribuidor de cargas de trabajo como se describe en las secciones siguientes.

### Personalizar la vista

1. Acceda al Distribuidor de cargas de trabajo en el área **Recursos**, tal como se describe en la sección [Acceso al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) en este artículo.

   Los nombres de los elementos de trabajo se muestran en el lado izquierdo y se representan con barras en el lado derecho del Distribuidor de cargas de trabajo. La longitud de la barra representa la cronología de un elemento de trabajo.

1. (Opcional y recomendada) Utilice los filtros de las áreas de Trabajo no asignado y Trabajo asignado para mostrar solo los elementos de trabajo o los usuarios que sean relevantes para usted.

   Para obtener más información, consulte [Filtrar información en el Distribuidor de cargas de trabajo](../workload-balancer/filter-information-workload-balancer.md).

   De forma predeterminada, las barras azules representan las escalas de tiempo de los proyectos y las tareas, y las barras granate representan problemas.

   Puede cambiar el color de las barras de los proyectos y las tareas cuando seleccione el tema de color que coincida con el proyecto. Para obtener más información, siga leyendo este procedimiento.

   Los elementos de trabajo del área de Trabajo asignado se ordenan por proyectos según los siguientes criterios, en este orden:
   1. Fecha planificada de inicio (la más antigua primero)
   1. Fecha planificada de finalización (la más antigua primero)
   1. Alfabético por proyecto (solo cuando los dos primeros criterios son idénticos para varios elementos de trabajo)

1. Haga clic en la **flecha que señala a la derecha** situada a la izquierda de las áreas sin asignar o asignadas para expandir todos los elementos bajo los nombres de proyecto (en el área sin asignar) y bajo los nombres de usuario (en el área asignada).

   >[!TIP]
   >
   >Los elementos de trabajo se muestran bajo nombres de proyecto en el área No asignada sólo cuando se habilita la opción &quot;Agrupar por proyecto&quot;.

1. Haga clic en la **flecha hacia abajo** a la izquierda de las áreas sin asignar o asignadas para contraer todos los elementos bajo los nombres de proyecto (en el área sin asignar) y bajo los nombres de usuario (en el área asignada).

1. Pase el ratón sobre él y, a continuación, arrastre y suelte la **línea de separación** entre el panel izquierdo y el área de la cronología para ajustar el tamaño del panel izquierdo.

   ![Línea de separación](assets/wb-adjust-panel-size.png)

1. Haga clic en el icono **Configuración** ![icono Configuración](assets/settings-gear-icon.png).

   El panel Configuración se muestra a la derecha.

   <span class="preview">Imagen de muestra en el entorno de vista previa:</span>
   ![Panel de configuración del Distribuidor de cargas de trabajo](assets/workload-balancer-settings.png)

   Imagen de muestra en el entorno de producción:
   ![Panel de configuración](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Seleccione entre las opciones que se enumeran a continuación para actualizar la información que visualiza en el Distribuidor de cargas de trabajo y, a continuación, haga clic en el icono **X** en la parte superior derecha del cuadro Configuración para cerrarlo.

   * **Agrupar por proyecto**: cuando se selecciona esta opción, los elementos de las áreas de trabajo asignado y no asignado se agrupan por proyecto. Esta opción está seleccionada de forma predeterminada.

   * **Incluir horas de problemas**: cuando se selecciona esta opción, los problemas asignados a usuarios se muestran bajo el nombre del usuario en el área de Trabajo asignado y los problemas que no están asignados a usuarios se muestran en el área de Trabajo no asignado. Las horas planificadas de los problemas se contabilizan hacia las horas planificadas para el proyecto y para el usuario en el área de Trabajo asignado.
   * **Mostrar fechas proyectadas**: cuando se selecciona esta opción, se muestra la escala de tiempo proyectada de los elementos de trabajo además de la escala de tiempo planeada. Observe lo siguiente:
      * La escala de tiempo proyectada del proyecto, las tareas y los problemas se muestra como una línea azul oscura encima de las barras de tareas, problemas y proyectos.
      * La escala de tiempo proyectada que se encuentra fuera de la escala de tiempo planificada se muestra en azul claro, incluso cuando se actualiza el tema de color, como se describe a continuación.
      * La escala de tiempo proyectada para los elementos que no tiene acceso a la vista se muestra en gris claro con una línea debajo.
      * Cuando una tarea o un problema se completan antes de la fecha planificada de finalización de vencimiento, los números de asignación para los días restantes se tachan y no se contabilizan en la asignación del usuario. Esto solo se muestra cuando están activados tanto la configuración Mostrar fechas proyectadas como el icono Mostrar asignación.

     >[!TIP]
     >
     >Tenga en cuenta que los elementos de trabajo se muestran en el Distribuidor de cargas de trabajo cuando sus escalas de tiempo planificadas o proyectadas (no necesariamente ambas al mismo tiempo) se producen durante el lapso de tiempo seleccionado.

   * **Mostrar trabajo completado**: cuando esté habilitado, las tareas y problemas completados se mostrarán en el área Trabajo asignado. Esta opción está activada de forma predeterminada.

     Cuando se completan, aparece un icono de marca de verificación verde en la esquina superior derecha de una tarea o barra de problemas. El mismo icono se muestra para un proyecto cuando se completan las tareas o problemas del lapso de tiempo seleccionado.
   * **Mostrar tiempo restante**: cuando está habilitada, Workfront muestra la diferencia entre el tiempo diario durante el cual el usuario está disponible para trabajar en función de sus programaciones y las horas para las que está asignado en el área Trabajo asignado para los usuarios. Esta opción está desactivada de forma predeterminada y el tiempo asignado se muestra de forma predeterminada.
   * <span class="preview">**Mostrar asignaciones de roles**: cuando esté habilitada, las asignaciones de roles se mostrarán en el área de Trabajo no asignado debajo de los elementos de trabajo asignados. Esto está habilitado de manera predeterminada.</span>

   * En la sección **Seleccionar tema de color**, seleccione el color que desee para las barras de proyecto y de tareas.

     >[!TIP]
     >
     >La configuración para seleccionar el tema de color no afecta al color de las barras de problemas. Los problemas siempre se muestran en una barra de color granate.

     Seleccione entre las siguientes opciones:
      * **Predeterminado**: las barras de todos los proyectos y sus elementos de trabajo se muestran en azul.
      * **Proyecto**: las barras asociadas a cada proyecto y sus tareas cambian según el nombre del proyecto. Todas las tareas que pertenecen al proyecto se muestran en barras que coinciden con el color del proyecto. Las barras de proyecto se muestran en un tono más claro para distinguirlas de las tareas. Las barras de proyecto también incluyen un icono de proyecto al elegir no mostrar las asignaciones.
      * **Estado del proyecto**: las barras asociadas a cada proyecto y sus elementos de trabajo cambian al color del estado del proyecto.

        El estado del proyecto es el asociado al Grupo del proyecto. Si el grupo no tiene estados específicos del grupo, el color de las barras de elementos de trabajo es el del estado del proyecto en el sistema. Se muestran tanto los estados del sistema como los personalizados. Para obtener información acerca de los estados de grupo, vea [Crear o editar un estado de grupo](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

   * En la sección **Mostrar asignación de usuarios en**, seleccione una de las siguientes opciones:
      * **Horas**: muestra el tiempo asignado como horas. Es la opción predeterminada.
      * **Porcentaje**: muestra el tiempo asignado como porcentaje del tiempo total disponible
   * En la sección **Preferencias de clasificación**, seleccione cómo desea que se ordenen los elementos en el Distribuidor de cargas de trabajo. Seleccione entre las siguientes opciones:
      * **Ordenar usuarios por función principal**: los usuarios se muestran en el orden alfabético de sus funciones principales en el área de Trabajo asignado.
      * **Ordenar usuarios alfabéticamente**: los usuarios se muestran en el orden alfabético de sus nombres en el área Trabajo asignado.
      * **Ordenar proyectos por**: seleccione un campo de proyecto del menú desplegable para ordenar los proyectos alfabéticamente por ese campo en las áreas de Trabajo no asignado o asignado.

   >[!TIP]
   >
   >Solo puede ordenar por proyectos cuando la configuración Agrupar por proyecto está habilitada. De lo contrario, este ajuste se atenúa.

1. (Opcional y condicional) Cuando cambie el tema de color a Estado del proyecto, pase el ratón sobre el nombre de un proyecto a la izquierda para ver su estado.

   ![Información sobre el estado del proyecto](assets/hover-over-project-status-tooltip-350x115.png)

### Asignar elementos de trabajo y ajustar las asignaciones de usuario

1. Acceda al Distribuidor de cargas de trabajo en el área de Recursos, tal como se describe en la sección [Acceder al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) en este artículo.
1. Haga clic en el icono **Mostrar asignaciones** ![Mostrar asignaciones](assets/show-allocations-icon-small.png) para ver las horas planificadas diaria o semanalmente para los elementos de trabajo.

   Esto reemplaza el nombre que aparece en las barras de los elementos de trabajo con la cantidad de horas planificadas diaria o semanalmente en las áreas de trabajo no asignado y asignado. Esta opción está desactivada de forma predeterminada.

   Los días que muestran sobreasignaciones se muestran en rojo.

   >[!TIP]
   >
   >* La opción Mostrar asignaciones solo afecta a lo que se muestra para proyectos, tareas, problemas y elementos inaccesibles. Las horas planificadas a diario para los usuarios se muestran de forma predeterminada y no se pueden ocultar.
   >* Debe habilitar la configuración Agrupar por proyecto para mostrar las horas planificadas diariamente para los proyectos.
   >* Cuando ve el Distribuidor de cargas de trabajo por semana, las horas mostradas son las horas planificadas semanalmente.

1. (Opcional) Pase el ratón sobre el tiempo asignado en la línea del usuario para comprender su capacidad y asignación. La capacidad es la disponibilidad del usuario según su programación.

   ![Detalles de tiempo asignado](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Opcional) Haga clic en el icono **Ocultar asignaciones** ![Mostrar asignaciones](assets/show-allocations-icon-small.png) para mostrar el nombre de las tareas y los problemas en las barras de los elementos de trabajo.
1. Haga clic en el icono de **menú Más** ![icono Más](assets/more-icon.png) a la derecha del nombre de una tarea, un problema, <span class="preview">o un rol</span> y, a continuación, haga clic en una de las opciones siguientes.

   ![Menú Más](assets/more-menu-right-of-task-350x104.png)

   * **Asigne esto a** y, a continuación, empiece a escribir el nombre de un usuario, rol o equipo al que desee asignar el elemento de trabajo en el campo **Buscar personas, roles o equipos**.

     Haga clic en **Avanzadas** para acceder a la pantalla Asignaciones avanzadas del elemento de trabajo. Para obtener más información, consulte [Crear asignaciones avanzadas](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

     También puede utilizar los siguientes métodos abreviados para asignar tareas o problemas:

      * En Windows: CTRL + clic en la barra de tareas o problemas.
      * En Mac: CMD + clic en la barra de tareas o problemas.

     Para obtener más información sobre la asignación de elementos de trabajo a los usuarios en el Distribuidor de cargas de trabajo, consulte [Información general sobre la asignación de trabajo en el Distribuidor de cargas de trabajo](../workload-balancer/assign-work-in-workload-balancer.md).

     >[!NOTE]
     >
     ><span class="preview">Las asignaciones de rol solamente se muestran en elementos de trabajo en el área de trabajo no asignado cuando la opción de configuración Mostrar asignaciones de rol está habilitada. Para obtener más información, consulte la sección [Personalizar la vista](#customize-the-view) en este artículo. Las asignaciones de roles solo tienen la opción **Asignar esto a** en el **menú Más**.</span>

     >[!TIP]
     >
     >Si el administrador de su Workfront o de su grupo ha habilitado las delegaciones en su entorno, utilice la pestaña Asignaciones para asignar usuarios a la tarea o al problema. Para obtener información sobre la delegación de trabajo, consulte [Delegar tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Edite asignaciones** y luego edite las asignaciones diarias o semanales para el usuario. Para obtener información acerca de la administración de asignaciones de usuarios, vea [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../workload-balancer/manage-user-allocations-workload-balancer.md).

   * **Abrir resumen**. El panel Resumen se abre a la derecha, luego hace clic en el campo Asignaciones y comienza a escribir el nombre de un usuario, rol o equipo en el campo **Buscar personas, rol o equipos** para asignar el elemento. Para obtener más información, vea la sección [Mostrar más información acerca de tareas y problemas](#display-more-information-about-tasks-and-issues) en este artículo.

1. (Opcional) Haga doble clic en una asignación diaria o semanal para un usuario dentro de la barra de un elemento de trabajo para editar el número de horas asignadas y, a continuación, haga clic en el icono **Guardar** ![Guardar icono](assets/save-allocations-wb.png) para guardar las asignaciones o en el icono **Cancelar** ![Cancelar icono](assets/cancel-allocations-wb.png) para eliminar las asignaciones que ha ajustado.

   >[!TIP]
   >
   >Los iconos Guardar y Cancelar se muestran hacia el final de una tarea o de la barra de cronología de un problema.
   >
   >![Guardar o cancelar asignaciones manuales](assets/cancel-and-save-icon-on-adjust-allocation-bar-wb-highlighted.png)

   Para obtener información acerca de la administración de asignaciones de usuarios, vea [Administrar asignaciones de usuarios en el Distribuidor de cargas de trabajo](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. Haga clic en **Asignaciones en lotes** para asignar elementos de trabajo en lotes.

   Para obtener más información, consulte [Asignar trabajo de forma masiva mediante el Distribuidor de cargas de trabajo](../workload-balancer/assign-work-in-workload-balancer-in-bulk.md).
1. Arrastre elementos del área **Trabajo sin asignar** o de un usuario y suéltelos en otro usuario para asignarlos.

   Para obtener más información, consulte [Asignar trabajo en el Distribuidor de cargas de trabajo arrastrando y soltando](../workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).

### Visualización de asignaciones en un gráfico

En lugar de ver las asignaciones en números diarios o semanales, puede verlas en un gráfico.

1. Acceda al Distribuidor de cargas de trabajo en el área de Recursos, tal como se describe en la sección [Acceder al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) en este artículo.
1. Haga clic en el **icono de gráfico** ![icono de gráfico](assets/user-allocation-chart-icon.png) para mostrar la asignación del usuario en formato de gráfico.

   Los días en los que el usuario está sobreasignado se muestran como bloques rojos y los días en los que el usuario está subasignado o en capacidad se muestran como bloques azules.

   El tamaño de los bloques indica la cantidad de la asignación: cuanto más grande sea el cuadro, más tiempo se asigna al usuario a los elementos de trabajo para ese día o semana.

   ![Asignación de usuarios como gráfico](assets/wb-allocation-as-chart.png)

### Mostrar más información sobre tareas y problemas

Puede ver más información sobre las tareas y los problemas en el Distribuidor de cargas de trabajo.

1. Acceda al Distribuidor de cargas de trabajo en el área de Recursos, tal como se describe en la sección [Acceder al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) en este artículo.
1. Para ver más información en el panel Resumen, siga uno de estos procedimientos:

   * Haga clic en la barra de una tarea o un problema para abrir el panel de resumen a la derecha.
   * Haga clic en el icono **Abrir resumen** ![Abrir icono de resumen](assets/summary-panel-icon.png) y, a continuación, haga clic en la barra de una tarea o problema para abrir el Panel de resumen.
   * Haga clic en el menú **Más** que se encuentra a la derecha de una tarea o problema y, a continuación, haga clic en **Abrir resumen**.

   Para obtener información acerca de cómo actualizar la información de tareas en el resumen del Distribuidor de cargas de trabajo, consulte [Actualizar elementos de trabajo en el Distribuidor de cargas de trabajo mediante el resumen](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

1. Pase el ratón sobre el nombre de una tarea o un problema para ver más información al respecto. Aparece un cuadro encima de la tarea o del problema con la siguiente información:

   * El nombre de la tarea o del problema.
   * El nombre del proyecto.
   * Las fechas planificadas de inicio y finalización.
   * Número de horas planificadas.
   * Para las tareas, el número de predecesora.
   * Para las tareas, un indicador en la esquina superior del cuadro que indica si la tarea está lista para trabajar o no.

   ![Detalles de la tarea](assets/task-bar-hover-over-detail-wb.png)

1. Haga clic en el nombre de un elemento de trabajo en la parte izquierda para acceder a él. El elemento de trabajo se abre en una nueva pestaña del explorador.

### Visualizar el Distribuidor de cargas de trabajo en pantalla completa

1. Acceda al Distribuidor de cargas de trabajo en el área de Recursos, tal como se describe en la sección [Acceder al Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) en este artículo.

1. Haga clic en el icono **Pantalla completa** ![Icono de pantalla completa](assets/full-screen.png) para mostrar el Distribuidor de cargas de trabajo en pantalla completa.

   El Distribuidor de cargas de trabajo ocupa toda la pantalla. Las ventanas y pestañas del explorador se excluyen de la vista.

1. Haga clic en el icono **Salir de pantalla completa** ![Salir del icono de pantalla completa](assets/exit-full-screen.png) para volver a la pantalla predeterminada y ver el Distribuidor de cargas de trabajo dentro de la pestaña del explorador.

## Desplazamiento por el Distribuidor de cargas de trabajo de un equipo

La navegación por el Distribuidor de cargas de trabajo de un equipo es similar a la navegación por el Distribuidor de cargas de trabajo para varios proyectos. Para obtener más información, consulte la sección [Navegar por el Distribuidor de cargas de trabajo para varios proyectos](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) en este artículo.

{{step1-to-team}}

La página de su equipo de inicio se muestra de forma predeterminada.

1. Haga clic en **Distribuidor de cargas de trabajo** en el panel de la izquierda.

   ![Distribuidor de cargas de trabajo de un equipo](assets/nwe-balancer-team-350x172.png)

   El Distribuidor de cargas de trabajo de un equipo muestra la siguiente información de forma predeterminada:

   * En el área **Trabajo sin asignar**: elementos de trabajo asignados al equipo o a los roles de equipo y trabajo y que no están asignados a usuarios. <span class="preview">Las asignaciones de roles se muestran en elementos de trabajo en el área de trabajo no asignado cuando la opción Mostrar asignaciones de roles está habilitada.</span>
   * En el área **Trabajo asignado**: los elementos de trabajo asignados a los usuarios se muestran bajo los nombres de los usuarios.

1. Continúe navegando por el Distribuidor de cargas de trabajo de un equipo como se describe en [Navegar por el Distribuidor de cargas de trabajo para varios proyectos en el área de Recursos](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) sección de este artículo.

## Navegar por el Distribuidor de cargas de trabajo de un solo proyecto

{{step1-to-projects}}

1. Haga clic en el nombre de un proyecto para abrir su página.
1. Haga clic en **Distribuidor de cargas de trabajo** en el panel de la izquierda.

   ![Distribuidor de cargas de trabajo de un proyecto](assets/nwe-balancer-project-350x152.png)

   El Distribuidor de cargas de trabajo del proyecto muestra la siguiente información de forma predeterminada:

   * En el área **Trabajo sin asignar**: elementos de trabajo del proyecto que están asignados a roles o equipos y no están asignados a usuarios. <span class="preview">Las asignaciones de roles se muestran en elementos de trabajo en el área de trabajo no asignado cuando la opción Mostrar asignaciones de roles está habilitada.</span>
   * En el área **Trabajo asignado**: elementos de trabajo en el proyecto que estén asignados al menos a un usuario.

   Se recomienda utilizar filtros para mostrar solo los usuarios que son importantes para usted.

   Por ejemplo, podría considerar la posibilidad de mostrar solo los usuarios que pertenecen a sus equipos o grupos. Para obtener más información, consulte [Filtrar información en el Distribuidor de cargas de trabajo](../workload-balancer/filter-information-workload-balancer.md).

1. (Opcional) Haga clic en el icono **Filtro** ![Icono de filtro](assets/filter-icon.png) en el área de Trabajo asignado y seleccione la opción **Elementos de trabajo de este proyecto** en el área **Sugeridos** del panel de filtro. Este filtro está desactivado de forma predeterminada.

   Si se selecciona esta opción, sólo se muestran los elementos asignados a los usuarios del proyecto seleccionado.

   Cuando la opción no está seleccionada, se muestran todos los elementos asignados a los usuarios del proyecto, independientemente de los proyectos a los que pertenezcan los elementos.

1. (Opcional y recomendada) Aplique un filtro en el área de Trabajo asignado para mostrar los usuarios que son importantes para usted pero que podrían no estar asignados a elementos del proyecto y, a continuación, haga clic en el icono **Mostrar todos los usuarios** ![Mostrar todos los usuarios](assets/show-all-users-icon-project-workload-balancer.png).

   Al mostrar todos los usuarios, puede mostrar todos los usuarios de Workfront que aún no están asignados al trabajo u otras funciones en el proyecto.

   Primero puede aplicar un filtro para reducir el número de usuarios que se muestran.

   Por ejemplo, es posible que desee filtrar primero por usuarios que pertenezcan a sus equipos o grupos y, a continuación, mostrar todos esos usuarios.

   Para obtener información sobre cómo generar un filtro, consulte [Información sobre filtros en el Distribuidor de cargas de trabajo](../workload-balancer/filter-information-workload-balancer.md).

   >[!NOTE]
   >
   > La opción Mostrar todos los usuarios solo está disponible para el Distribuidor de cargas de trabajo de un proyecto.

1. (Opcional) Haga clic en el icono **Mostrar asignaciones de roles** ![Mostrar asignaciones de roles](assets/show-role-allocation-icon.png).

   Se muestra el panel Asignación de funciones.

   Puede ver información sobre las horas planificadas asociadas con los roles del proyecto y los roles asociados con las iniciativas vinculadas a los proyectos desde el Scenario Planner.

   Para obtener más información, consulte [Información general sobre la conciliación de asignaciones de recursos entre proyectos e iniciativas](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).


   >[!NOTE]
   >
   >No puede ver la información de función de la iniciativa si su organización no ha adquirido una licencia para el Scenario Planner de Workfront. En este caso, solo puede ver las horas planificadas asociadas con los roles del proyecto. Para obtener más información, consulte [Acceso necesario para usar el Scenario Planner](../../scenario-planner/access-needed-to-use-sp.md).

1. Continúe navegando por el Distribuidor de cargas de trabajo de un proyecto como se describe en la sección [Navegar por el Distribuidor de cargas de trabajo para varios proyectos](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) de este artículo.

<!--old content below - this used to be a one-large-procedure article - outdated, and rewrote it above with several smaller procedures: 

# Navigate the Workload Balancer

<!-drafted note for 22.4 release: remove all production/ preview references at Prod release>

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

Use the Workload Balancer to understand the availability of your resources as well as to assign work to your users. This article walks you through using the icons and settings available to update the view for and navigate the Workload Balancer.

>[!NOTE]
>
>The Workload Balancer is a resource scheduling tool that will eventually replace the current resource scheduling tools which are currently deprecated. 
>
>For more information about removing the resource scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).
>
>We recommend that you use the Workload Balancer for scheduling your resources.

The Workload Balancer is available in multiple areas of Adobe Workfront. Navigating it is similar in all areas. This article describes how to navigate the Workload Balancer for multiple projects in the Resourcing area. For more information about where the Workload Balancer is located, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

For information about managing resources using the Workload Balancer, also consider reading the following articles:

* [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
* [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, when using the Workload Balancer in all areas in the Production environment</p>
   <p><span class="preview">Work, when using the Workload Balancer of a project, in the Preview environment</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for viewing items in the Workload Balancer

Consider the following when viewing the Workload Balancer:

* Projects display in the Workload Balancer only when the Group by Project setting is enabled. This setting is enabled by default.
* Mousing over a task or an issue displays the following additional information about the task or issue:

  * Project name

  * Task or issue name

  * Parent task

  * Planned Start and Completion Dates

  * Number of Planned Hours

  * Ready to start or Not ready status

  ![task-pop-up-with-additional-info-in-workload-balancer](assets/task-pop-up-with-additional-info-in-global-wb.png)

* When a project has no tasks during a period of time, the bar at the project level becomes a dimmed color.

  ![Break in project timeline](assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png)

* When you don't have permissions to see certain items, they display as **Inaccessible work items** or **Inaccessible projects**.

  ![Inaccessible items](assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png)

* The names of the work items display on the left and within the timeline selected on the right. 
* The total of Planned Hours for each work item displays to the right of the name of the work items on the left. 
* The total of the Planned Hours for each project displays to the right of the name of the project on the left.

  The Planned Hours information for the project is a total of Planned Hours from all items listed in the Workload Balancer, and not a total of Planned Hours on the project.

## Overview of the Unassigned Work and Assigned Work areas

The Workload Balancer displays work items in two separate areas, depending on their assignments.

The two areas of the Workload Balancer display the following information:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Unassigned Work</td> 
   <td> <p>This area displays tasks <span class="preview">and issues</span> unassigned to users. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>This area does not display any work items by default. We recommend using filters to display relevant information for you in this area.</p> <p>After you apply a filter, this area displays the following work items:</p> 
    <ul> 
     <li>unassigned</li> 
     <li>assigned to a team </li> 
     <li>assigned to a job role</li> 
     <li> <p>assigned to a team and a role at the same time</p> </li> 
    </ul> <p>Tip: Items assigned to a user as the primary assignee do not display in the Unassigned Work area. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assigned Work</td> 
   <td> <p> All active users in the system display in this area by default. We recommend using filters to limit the amount of information in this area.  </p> <p>Both tasks and issues display in the Assigned Work area. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>The work items that the users are assigned to display under their names. </p> <p>If a work item is assigned to multiple users, the item displays under each assigned user. </p> </td> 
  </tr> 
 </tbody> 
</table>

For information about applying a filter in the Workload Balancer, see [Filter information in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

![Empty unassigned area](assets/balancer-empty-unassiged-area-350x179.png)

## Navigate the Workload Balancer

You can update the view in the Workload Balancer to display exactly the information you need to focus on in the time frame that makes the most sense to you.

After selecting the settings you want to apply to your view, the Workload Balancer remembers these settings every time you access it from any browser or device.

1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Resourcing**.
1. Click **Workload Balancer** in the left panel.

   The Workload Balancer displays work assignment information starting with the current week. The names of work items are listed on the left side as well as represented by bars on the right side of the of the Workload Balancer within their respective timelines. By default, blue bars represent the timelines of projects and tasks and maroon bars represent issues.

   >[!TIP]
   >
   >You can change the color of the bars for projects and tasks when you select your color scheme to match the project. For more information, continue reading this procedure.

   The work items that display under the name of users in the Workload Balancer are sorted by the following criteria, in this order:

   1. Planned Start Date (oldest first)
   1. Planned Completion Date (oldest first)
   1. Alphabetical by project (only when the first two criteria are identical for multiple work items)

1. Click the right-pointing arrow to the left of the Unassigned or Assigned areas to expand all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Click the down-pointing arrow to the left of the Unassigned or Assigned areas to collapse all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Use the horizontal scroll to navigate the timelines of work items that extends beyond the limits of the screen. 
1. Use the vertical scroll to display additional users and work items. 
1. Drag and drop the separation line between the left panel and the timeline areas to adjust the size of the left panel.

   ![Separation between left panel and timeline](assets/separation-line-between-left-panel-and-timeline-highlighted-nwe-350x174.png)

1. Click the **Filter icon** ![Filter icon](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or the **Assigned Work** areas to select the type of information to display in the Workload Balancer.

   For information about filtering information in the Workload Balancer, see [Manage filters in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md). 

1. Click the right-pointing arrow next to **Unassigned Work** to expand this area or the down-pointing arrow to collapse it.

   >[!TIP]
   >
   >No items display in this area by default. You must apply a filter to view unassigned work items.

1. Drag and drop the separation line between the **Unassigned Work** and **Assigned Work** areas to adjust their size.

   ![Separation line between areas](assets/modern-scheduler-separation-line-between-areas-350x278.png)

1. Click the back or forward icons ![Back and forward icons](assets/back-and-forward-icons.png) to navigate the timeline, then click **Today** to return to the current week. 

1. Click the **time frame drop-down menu** on the toolbar, then click the beginning date of the period you want to display. By default, the first week selected on the calendar is the week you navigated to.

   ![Calander date picker](assets/calendar-date-picker-wb.png)


1. Click one of the following options in the toolbar to display information by different time frames:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Day</td> 
      <td>Displays information by day for four weeks starting with today's date, by default. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Week</td> 
      <td>Displays information by week for four weeks. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Month</td> 
      <td> <p><span>Displays information by month for three months.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Select the number of weeks you want to display at one time in the Workload Balancer from the following options:

   * 1 week
   * 2 weeks
   * 4 weeks. This is the default setting.
   * 6 weeks
   * 3 months
   ![3 months dropdown](assets/3-months-12-weeks-drop-down-wb.png)     

1. Click the **Settings** icon ![Settings icon](assets/settings-gear-icon.png).

   The Settings panel displays.

   ![Settings box](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Select from the options listed below to update the information you view in the Workload Balancer, then click the **X icon** in the upper-right of the Settings box to close it.

   * **Group by Project**: When this is selected, the items in the Unassigned and Assigned Work areas are grouped by project. This is selected by default.

     ![Group by project](assets/group-by-project-350x530.png)

   * **Include hours from issues**: When this is selected, issues assigned to users display under the user's name in the Assigned Work area <span class="preview">and issues that are not assigned to users display in the Unassigned Work area</span>. The Planned Hours from the issues count towards the Planned Hours for the project and for the user in the Assigned Work area. 

        ![Issue on Workload Balancer](assets/issue-on-workload-balancer-350x20.png)

   
      * **Show Projected Dates**: When this is selected, the projected timeline of work items displays in addition to the planned timeline. Notice the following:

         * The projected timeline of project, tasks, and issues displays as a dark blue line above the task, issue, and project bars.
         * The projected timeline that is outside of the planned timeline displays in light blue, even when you update the color theme, as described below.
         * The projected timeline for the items that you have no access to view displays in light gray with a line underneath.
         * When a task or issue completes before the due Planned Completion Date the allocation numbers for the remaining days are struck through and do not count towards the user's allocation. This displays only when both the Show Projected Dates setting and the Show allocation icon are enabled.

         ![Task issue projected timelines](assets/task-issue-projected-timelines-350x91.png)

         >[!TIP]
         >
         >Notice that work items display in the Workload Balancer when either their planned or the projected timelines (not necessarily both at the same time) occur during the timeframe selected.

   * **Show completed work**: When this is enabled, tasks and issues that are completed display in the Assigned Work area. This is enabled by default.

     A green checkmark icon ![Checkmark icon](assets/green-checkmark-icon.png) displays to the upper-right corner of a task or issue bar when they are completed. The same icon displays for a project when the tasks or issues for the selected time frame of the project are completed. 
   
   * **Show remaining time**: When this is enabled, Workfront displays the difference between the daily time for which the user is available to work based on their schedules and the hours for which they are allocated in the Assigned Work area for the users. This is disabled by default and allocated time displays by default.

   * In the **Select color theme** section, select the color that you want for the project and task bars.  

      >[!NOTE]
      >
      >The setting for selecting the color theme  does not affect the color of the issue bars. Issues always display in a maroon-color bar. 


      Select from the following:

      * **Default**: The bars for all projects and their work items display in blue.  
      * **Project**: The bars associated with each project and its tasks change according to the name of the project. All tasks that belong to the project display in bars that match the color of the project. The project bars display in a lighter shade to distinguish them from the tasks. The project bars also include a project icon when choosing not to display allocations.
      * **Project Status**: The bars associated with each project and its work items change to the color of the status of the project.

        >[!TIP]
        >
        >* The project status is that associated with the Group of the project. If the Group does not have group-specific statuses, the color of the work item bars is that of the system-level project status. Both system as well as custom statuses display. For information about group statuses, see [Create or edit a group status](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
        
   * In the **Display user allocation in** section, select from the following:

      * **Hours**: Displays allocated time as hours. This is the default. 
      * **Percentage**: Displays allocated time as a percentage of the total available time

   * In the **Sorting preferences** section, select how you want the items to be sorted in the Workload Balancer. Select from the following options: 

      * **Sort users by Primary Role**: Users display in the alphabetical order of their Primary Roles in the Assigned Work area.

      * **Sort users alphabetically**: Users display in the alphabetical order of their first names in the Assigned Work area.

      * **Sort projects by**: Select a project field from the drop-down menu to sort projects alphabetically by that field in the Unassigned or Assigned Work areas. 

      >[!TIP]
      >
      >You can sort by projects only when the Group by Project setting is enabled. Otherwise, this setting is dimmed.


1. (Optional and conditional) If you changed the color theme to Project Status, hover over the name of a project on the left to view the status of the project.

   ![Project status tooltip](assets/hover-over-project-status-tooltip-350x115.png)

1. <span class="preview">(Conditional and recommended) In the Workload Balancer of a project, apply a filter in the Assigned Work area to display users that are important to you but might not be assigned to items on the project, then click the **Show all users** icon ![Show all users   ](assets/show-all-users-icon-project-workload-balancer.png). This displays other users in the system that are not yet assigned on the project. For information about how to build a filter, see [Manage filters in the Workload Balancer](../workload-balancer/filter-information-workload-balancer.md).</span>

 
   >[!TIP]
   >
   ><span class="preview">The Show all users icon is available only for the Workload Balancer of a project.</span> 

1. Click the **Chart icon** ![Chart icon](assets/user-allocation-chart-icon.png) to display the user allocation in a chart format. Days where the user is overallocated display as red blocks, and days where the user is underallocated or at capacity display as blue blocks. The size of the blocks indicates the amount of the allocation: the larger the box, the more time the user is allocated to work items for that day or week.

   ![User allocation chart](assets/user-allocation-chart-350x237.png)

1. Click the **Show allocations icon** ![Show allocations icon](assets/show-allocations-icon-small.png) to view the daily or weekly Planned Hours for work items.

   This replaces the name in the bars of the work items with the amount of daily or weekly Planned Hours in the Unassigned and Assigned Work areas. This setting is disabled by default.

   >[!TIP]
   >
   >* The Show allocations setting only affects what displays for projects, tasks, issues and inaccessible items. Daily Planned Hours for users display by default and cannot be hidden.
   >* You must enable the Group by Project setting to display daily Planned Hours for projects. 
   >* When you view the Workload Balancer by week, the hours displayed are the weekly Planned Hours. 

   Days that show overallocations display in red. 

1. (Optional) Hover over the allocated time in the user line to understand what the capacity and allocation of the user. The capacity is the availability of the user according to their schedule.

   ![Overallocation vs capacity](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Optional) Click the **Hide allocations icon** ![Show allocations icon](assets/show-allocations-icon-small.png) to display the name of the tasks in the bars of the work items. 
1. Click the **More menu** icon ![More icon](assets/more-icon.png) to the right of a task or issue name, then click one of options below. 

   ![More menu](assets/more-menu-right-of-task-350x104.png)

      * **Assign this to**, then start typing the name of a user, role, or team you want to assign the work item to in the **Search people, role, or teams** field.
    
      >[!TIP]
      >
      >You can also use the following shortcuts to assign tasks or issues:
      >
      >* In Windows: CTRL+click the task or issue bar.
      >* In Mac: CMD+click the task or issue bar.

      For more information about assigning work items to users in the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md). 

      >[!TIP]
      >
      >If your Workfront or group administrator enabled delegations in your environment, use the Assignments tab to assign users to the task or issue. For information about delegating work, see [Manage task and issue delegation](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Edit allocations**, then edit the daily or weekly allocations for the user. For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

1. Click the bar of a task or issue to open the Summary panel on the right

   Or

   Click **Open Summary** icon ![Open Summary icon](assets/summary-panel-icon.png), then click the bar of a task or issue to open the Summary panel

   Or

   Click the **More** menu ![More icon](assets/more-icon.png) to the right of a task or issue, then click **Open Summary**.

   For information about updating task information in the Summary in the Workload Balancer, see [Update work items in the Workload Balancer using the Summary](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

    The Summary panel opens on the right. 

1. Click **Bulk Assignments** to assign work items in bulk.

   For more information, see [Assign work in bulk using the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md). 

1. Click the **Full screen** icon ![Full screen icon](assets/full-screen.png) to display the Workload Balancer in full screen, then click the **Exit full screen** icon ![Exit full screen](assets/exit-full-screen.png) to return to the default screen. 
1. (Optional) Double-click a daily or weekly allocation for a user inside the bar of a work item to edit the number of allocated hours, then click the **Save** icon ![Save icon](assets/save-allocations-wb.png) to save the allocations or the **Cancel** icon ![Cancel icon](assets/cancel-allocations-wb.png) to remove the allocations you adjusted.

   >[!TIP]
   >
   >The Save and Cancel icons display towards the end of a task or an issue's timeline bar.

   For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md). 

1. Click the name of a work item on the left to access it. 
1. Click the **Shareable link icon** ![](assets/wb-shearable-link-icon-small.png) to copy the direct URL for the Workload Balancer to your clipboard. 
1. (Optional) Share the link with any user who does not have direct access to the Workload Balancer.

   For information about sharing the Workload Balancer with a link, see [Share the Workload Balancer with a link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md). 

1. (Conditional) From the Workload Balancer of a project, click the **Show role allocations** icon ![Show role allocations](assets/show-role-allocation-icon.png).

   The Role Allocation panel displays. You can view information about Planned Hours associated with job roles on the project and job roles associated with initiatives from the Scenario Planner. For more information, see [Overview of reconciling resource allocations between projects and initiatives](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

   >[!TIP]
   >
   >You cannot view initiative job role information if your organization has not purchased a license for the Workfront Scenario Planner. In this case, you can only view the planned hours associated with job roles on the project. For more information, see [Access needed to use the Scenario Planner](../../scenario-planner/access-needed-to-use-sp.md).

-->
