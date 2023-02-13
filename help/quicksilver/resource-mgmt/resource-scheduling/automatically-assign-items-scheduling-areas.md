---
product-area: resource-management
navigation-topic: resource-scheduling
title: Asignación automática de tareas y problemas no asignados en las áreas de programación
description: Al utilizar las herramientas de programación, puede permitir que Adobe Workfront analice las asignaciones de trabajo actuales entre los usuarios disponibles y proponga asignaciones inteligentes y lógicas para cualquier tarea o problema que aún no se haya asignado. Puede modificar las asignaciones propuestas antes de finalizarlas.
author: Alina
feature: Resource Management
exl-id: 087fe3ef-9b85-491b-9fdc-436a01822ede
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 0%

---

# Asignación automática de tareas y problemas no asignados en las áreas de programación

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
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Al utilizar las herramientas de programación, puede permitir que Adobe Workfront analice las asignaciones de trabajo actuales entre los usuarios disponibles y proponga asignaciones inteligentes y lógicas para cualquier tarea o problema que aún no se haya asignado. Puede modificar las asignaciones propuestas antes de finalizarlas.

Workfront examina las tareas y los problemas disponibles en el área Sin asignar dentro del intervalo de fechas seleccionado actualmente y propone asignaciones para cada elemento a la vez. Puede crear un filtro para limitar el número de elementos disponibles en el área Sin asignar.

El administrador del sistema determina cómo calcula Workfront la disponibilidad de los recursos en el nivel del sistema (teniendo en cuenta las horas y la disponibilidad de FTE). Según esta configuración de todo el sistema, la disponibilidad de los recursos se calcula mediante la programación predeterminada o la programación del usuario. Para obtener más información, consulte [Configure cómo calcula Workfront la hora del recurso y la disponibilidad de FTE para el área de programación](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

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
   <td> <p>Ver o tener más acceso a Proyectos, Tareas y Problemas</p> <p><strong>NOTA</strong>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de Contribute o superior a los proyectos, tareas y problemas para los que actualice asignaciones</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos {#prerequisites}

Workfront utiliza un algoritmo propietario para determinar las propuestas de asignación. Para facilitar los mejores resultados, asegúrese de que la siguiente información sea precisa en Workfront:

* Información sobre tareas y problemas, incluidos:

   * Asignaciones de funciones\
      No se formula ninguna propuesta para las tareas y los problemas que no están asignados a una función.
   * Horas planificadas\
      Si una tarea o un problema no tiene horas planificadas actualmente, Workfront supone 4 horas planificadas por día laboral al asignar automáticamente el trabajo. Estas horas no se asignan automáticamente al elemento de trabajo; solo se utilizan para garantizar distribuciones de asignación más realistas.
   * Fechas de inicio y fechas de finalización previstas

* Información de usuario, que incluye:

   * Asignaciones de funciones principales y secundarias en el perfil del usuario
   * Información del equipo del proyecto

## Configuración de límites de funciones

Los límites de funciones controlan el número de usuarios, con una función específica, a los que se puede asignar trabajo automáticamente. Los límites de funciones funcionan por proyecto para garantizar que las tareas basadas en roles no se extiendan entre un gran número de usuarios.

Los siguientes escenarios describen cómo se aplican los límites de funciones a los proyectos:

* **Escenario 1**: Si no hay usuarios asignados al equipo del proyecto, el sistema utiliza el límite de funciones para asignar tareas.\
   Por ejemplo, tiene un proyecto sin usuarios asignados al equipo del proyecto. Este proyecto tiene 10 tareas de administración de proyectos que deben asignarse y ha establecido un límite de funciones de 1 para la función de administrador de proyectos. El sistema asigna las 10 tareas a 1 administrador de proyectos porque el límite de funciones está establecido en 1.

* **Escenario 2**: Si el límite de funciones es bueno que el número de usuarios asignados al equipo del proyecto, se asignan tareas a usuarios adicionales.\
   Por ejemplo, tiene un proyecto con un escritor asignado al equipo del proyecto. Este proyecto tiene 12 tareas de escritura que deben asignarse y tiene un límite de funciones de 2 definido para la función de escritor. El sistema asigna las 12 tareas entre el escritor del equipo del proyecto y un escritor adicional porque el límite de funciones está establecido en 2.

* **Escenario 3**: Si el límite de funciones es menor que el número de usuarios asignados al equipo del proyecto, se anula el límite de funciones.\
   Por ejemplo, tiene un proyecto con 4 diseñadores asignados al equipo del proyecto. Este proyecto tiene 8 tareas de diseñador que deben asignarse y ha establecido un límite de funciones de 2 para la función de Designer. El sistema asigna las 8 tareas entre cada uno de los 4 diseñadores de equipos de proyecto, aunque el límite de funciones esté establecido en 2.

Para establecer límites para las asignaciones de funciones de trabajo:

1. Vaya a la cronología de programación de varios proyectos o de un proyecto individual:

   * **Para varios proyectos**:  Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un proyecto individual**: Vaya a un proyecto y haga clic en el **Equilibrador de carga de trabajo** del panel izquierdo y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.

1. Haga clic en el **Configuración** icono.\
   ![Automode_settings.png](assets/automode-settings.png)

1. En la sección Programación automatizada de recursos , haga clic en la **Límite** en línea con el elemento de la columna **Función** e introduzca un número positivo.\
   Workfront guarda automáticamente los cambios.

   >[!NOTE]
   >
   >Todos los miembros actuales del equipo del proyecto son elegibles automáticamente para todo el trabajo recomendado, independientemente del límite de funciones establecido.

   ![Set_Role_Limits.png](assets/set-role-limits-350x341.png)

1. (Opcional) Haga clic en el **Mostrando** en la parte superior de la columna Límite y seleccione las opciones de visualización que desee.
1. Para volver al área de programación de recursos, haga clic en **Volver a la programación**.

## Asignación automática de tareas y problemas

Puede asignar tareas y problemas a los usuarios en la cronología de programación, tanto si se encuentra en la ficha Programación (al programar recursos para varios proyectos) como en la pestaña Dotación de personal (al programar recursos para un proyecto individual).

Para permitir que Workfront proponga automáticamente asignaciones para tareas y problemas en el área Sin asignar:

1. Vaya a la cronología de programación de varios proyectos o de un proyecto individual:

   * **Para varios proyectos**:  Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Workfront, haga clic en **Recursos > Equilibrio de carga de trabajo** y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.
   * **Para un proyecto individual**: Vaya a un proyecto y haga clic en el **Equilibrador de carga de trabajo** del panel izquierdo y, a continuación, seleccione **Programación** en el menú desplegable superior izquierdo.

1. (Opcional) Cree un filtro para personalizar qué contenido se muestra en el área No asignado de la cronología de programación.\
   Para obtener más información sobre cómo crear un filtro, consulte [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md#creating-and-modifying-filters-on-the-scheduling-tab-for-projects) en [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) [Filtrado de información en el área Programación](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)

   >[!TIP]
   >
   >Para asegurarse de que Workfront asigna trabajo a los usuarios más aptos:
   >
   >* Filtre únicamente la información que afecta a las tareas que se muestran en el área Sin asignar (como Portfolio, Programas y Proyectos).
   >* Se recomienda no filtrar la información que afecte a los usuarios disponibles para asignar en la cronología de programación. Al hacerlo, Workfront no puede ver a todos los posibles destinatarios, lo que puede resultar en asignaciones menos satisfactorias.


1. (Opcional) Modifique el intervalo de fechas que se muestra en la cronología de programación, tal como se describe en [Ajustar el intervalo de fechas de las áreas de programación](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) en [Introducción a la programación de recursos](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). Workfront realiza asignaciones solo para tareas y problemas dentro del intervalo de fechas visible en la cronología de programación.

1. Haga clic en el **Automático** en la esquina superior derecha de la cronología de la programación.\
   ![scheduling_auto.png](assets/scheduling-auto-350x221.png)\
   Workfront propone asignaciones para cada tarea o problema en el **No asignado** .

   >[!TIP]
   >
   >Las tareas y los problemas ya deben asignarse a una función para que se proponga una asignación. Para garantizar los mejores resultados, las tareas y los problemas deben contener la información descrita en [Requisitos previos](#prerequisites).

   Las asignaciones propuestas se diferencian con un contorno punteado alrededor de cada tarea o problema, de la siguiente manera:\
   **Asignación de tarea propuesta:**

   **Asignación de tarea existente:**

1. (Opcional) Puede modificar cualquier asignación propuesta o existente antes de finalizar las asignaciones:

   >[!NOTE]
   >
   >Si modifica una asignación existente, esta cambia a un estado propuesto.

   * Para asignar un artículo a un usuario diferente:

      * Arrastre la tarea o el problema del usuario propuesto a la fila de otro usuario que desee asignar.

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE: lists in this article need to be reformatted and maybe split - too many levels in)      
        </MadCap:conditionalText>      
        -->

         Se muestran un máximo de 10 tareas por día para un usuario determinado. Puede ampliar la lista para ver todas las tareas asignadas actualmente a ese usuario. (Después de realizar asignaciones en la cronología de programación, es posible que se muestren más de 10 tareas de forma temporal).\
         Al arrastrar un elemento, se muestra la siguiente información antes de soltar la tarea o el problema y de completar la asignación:

         * Se muestra un indicador de colocación en la fila del usuario. Esto permite ver dónde se asigna un elemento antes de realizar la asignación.
         * Si las asignaciones de usuario están habilitadas en la cronología de programación, se muestran los indicadores rojos de sobreasignación si al completar la asignación se sobreasigna al usuario.\
            Para obtener más información sobre los indicadores de sobreasignación, consulte [Indicadores de asignación](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators).

         * Los usuarios que no pueden recibir la asignación aparecen atenuados.
      * Expanda la tarea o el problema que desee asignar, haga clic en la flecha desplegable en la **Asignaciones** , empiece a escribir el nombre del usuario que desea asignar y, a continuación, haga clic en el nombre del usuario en la lista desplegable.\
         ![schedule_task_expand.png](assets/schedule-task-expanded-350x170.png)
   * Para posponer la creación de una asignación, arrastre cualquier tarea o problema que aún no esté listo para volver a asignar a la función **No asignado** .



1. Haga clic en el **Realización de asignaciones** en la parte superior de la cronología de programación para finalizar las asignaciones propuestas.\
   O\
   Haga clic en **Cancelar** devolver todas las asignaciones propuestas a sus anteriores puestos.
