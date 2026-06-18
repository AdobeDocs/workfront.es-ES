---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Crear asignaciones avanzadas
description: Puede administrar asignaciones de tareas o problemas mediante Asignaciones avanzadas.
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
autotag-review: '2026-06-18T17:43:58.800Z'
TQID: 'https://experienceleague.adobe.com/qZvXwTMlCd5p08duYVqbyHpkML4oXtbijHuCzlukywg'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: 3361
ht-degree: 31%

---

# Crear asignaciones avanzadas

<!-- Audited: 11/2025-->

<!--remove the bullet indicated when we get rid of the new/old experience of editing tasks-->


<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

Puede administrar asignaciones de tareas o problemas mediante Asignaciones avanzadas.

Puede ajustar la siguiente información de asignación al realizar asignaciones avanzadas:

* Asignar usuarios a la tarea o problema (esto puede realizarse fuera de una asignación avanzada).
* Ajuste y redistribuya el número de horas que se asignan a cada usuario asignado.
* Determine qué usuario debe designarse como propietario o principal asignado a la tarea o al problema.
* Especifique la función que cumple cada usuario al trabajar en la tarea o el problema.
* Agregar información de facturación y de tasa de costo al nivel de asignación.
* Revise los siguientes detalles de cada asignación: horas planificadas, costo total e ingresos totales.

>[!NOTE]
>
>Al asignar usuarios para trabajar, su disponibilidad según sus programaciones afecta a las fechas planificadas y proyectadas de las tareas y problemas. Para obtener información acerca de las programaciones, consulte [Crear una programación](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td> <p>Para agregar tarifas de facturación y de costo en asignaciones de tareas, use la búsqueda avanzada: Flujo de trabajo Ultimate</p> <p>Para crear asignaciones avanzadas: Cualquier paquete de flujo de trabajo o Workfront</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p>
   <p>Trabajo o superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role>Configuraciones de nivel de acceso</td> 
   <td> <p>Editar el acceso a Tareas y Problemas</p>  </td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Aportar o permisos superiores a la tarea o al problema</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Áreas de Adobe Workfront donde puede realizar asignaciones avanzadas

Este artículo describe cómo acceder a las asignaciones avanzadas en el encabezado de la tarea o del problema.

Además, puede realizar asignaciones avanzadas en las siguientes áreas de Workfront:

* En listas e informes cuando el campo Asignaciones aparece en la vista.
* En la sección Asignaciones al editar una tarea. Para obtener más información, consulte [Editar tareas](../../../manage-work/tasks/manage-tasks/edit-tasks.md). <!--When we remove the old/ new experience: take this bullet out completely; in the new Edit Task experience, this is no longer possible-->
* En el encabezado de la tarea o del problema, en el área Asignaciones.
* En el Distribuidor de cargas de trabajo. Para obtener más información, consulte [Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

La creación de asignaciones avanzadas difiere según el paquete de Workfront que haya adquirido su organización.

## Crear asignaciones avanzadas para paquetes de Ultimate de flujo de trabajo

Este diseño de Asignaciones avanzadas se aplica solo a tareas. Para problemas, consulte la sección [Crear asignaciones avanzadas para todos los demás paquetes](#create-advanced-assignments-for-all-other-packages) en este artículo.

>[!NOTE]
>
>La experiencia antigua de Asignaciones avanzadas es la predeterminada. Debe activar manualmente la nueva experiencia con el botón en la parte superior derecha de la ventana Asignaciones avanzadas.
>Para obtener información sobre la experiencia anterior, consulte la sección [Crear asignaciones avanzadas para todos los demás paquetes](#create-advanced-assignments-for-all-other-packages) en este artículo.

1. Vaya al proyecto donde desea asignar una tarea.
1. Haga clic en **Tareas** o **Problemas** en el panel izquierdo y, a continuación, haga clic en el nombre de una tarea de la lista.

   >[!TIP]
   >
   >Puede realizar asignaciones avanzadas directamente en la lista de tareas. Haga clic dentro del campo **Asignaciones** en la misma línea que la tarea y, a continuación, haga clic en **Avanzadas** en la parte inferior de la lista o en el **icono Personas** en la esquina superior derecha del cuadro de asignaciones para abrir la ventana Asignaciones avanzadas. Pase al paso 5 para continuar creando asignaciones avanzadas.
   >![Haga clic en Avanzadas o en el icono Personas](assets/access-aa-from-lists.png)

1. Haga clic en **Asignar a** en el campo **Asignaciones** del encabezado de la tarea

   O

   Haga clic en uno de los nombres asignados si la tarea ya está asignada.

1. Haga clic en **Avanzadas**.

   ![Haga clic en Avanzadas](assets/assignments-from-task-header-0825.png)

   Se abre la ventana Asignaciones avanzadas.

   ![Ventana de asignaciones avanzadas](assets/advanced-assignments-031826.png)

1. Revise la información de duración de la tarea según sea necesario. Todos estos campos son de solo lectura desde Asignaciones avanzadas y puede actualizarlos en la tarea.

   Para obtener información acerca de la duración de la tarea, los tipos de duración, las unidades de tiempo y las horas planificadas, vea [Información general sobre la duración de la tarea y el tipo de duración](/help/quicksilver/manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   >[!NOTE]
   >
   >Si no se muestra una columna de datos que desee ver, puede agregarla. Consulte [Agregar y eliminar columnas en la lista de asignaciones avanzadas](#add-and-remove-columns-on-the-advanced-assignments-list), a continuación.

1. (Opcional) Seleccione **Horas**, **ETC** o **Porcentaje** para ver las asignaciones.

   Se puede ver la asignación de un usuario en horas planificadas, como porcentaje de su capacidad, o en FTE (equivalente a tiempo completo, escala 0-1). El valor predeterminado es Horas.

   Para obtener información sobre FTE, consulte [Configurar las preferencias de administración de recursos](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

1. Haga clic en **Nueva fila** para agregar una asignación a la tarea.

1. Haga clic en la columna **Usuario asignado** para agregar un usuario o equipo. Empiece a escribir el nombre del usuario o equipo y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!NOTE]
   >
   >Si el nombre contiene un carácter especial, debe incluirlo en el campo de búsqueda.

   Cuando agrega un usuario que tiene un rol principal, entonces se rellena el **Rol asignado**.

   Si el usuario tiene atributos asignados a su perfil, los atributos se rellenan en la asignación de tareas.

1. Para agregar un rol cuando no conozca al usuario que trabajará en la tarea, haga clic en la columna **Rol asignado**. Empiece a escribir el nombre de la función y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!NOTE]
   >
   >Si el nombre contiene un carácter especial, debe incluirlo en el campo de búsqueda.

   Si la función tiene atributos asignados de la tarjeta de tasas de un proyecto, los atributos se rellenan en la asignación de la tarea.

   Cuando asigne un usuario más adelante mediante el campo Usuario asignado, la búsqueda básica sigue este algoritmo:

   * Coincidencia completa: Función del puesto y todos los atributos
   * Coincidencia parcial: Función del puesto y algunos atributos
   * Coincidencia de rol solamente

   Para obtener información acerca de la búsqueda avanzada, consulte [Usar la búsqueda avanzada](#use-the-advanced-search) en este artículo.

1. (Opcional) Siga agregando usuarios asignados en filas nuevas para agregar varios recursos a la tarea.

   >[!TIP]
   >
   >* Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos. Se permite un máximo de 200 usuarios asignados por tarea.
   >
   >
   >* Al añadir una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos.
   >Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
   >Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Si un usuario, un rol o un equipo se han asignado antes de que se desactiven, permanecerán asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >   
   >   * Reasignar el elemento de trabajo a los recursos activos.
   >   * Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

1. Para marcar a un usuario asignado como el propietario de la tarea, seleccione la casilla de verificación de la fila y haga clic en **Definir principal** en la barra de acciones de la parte inferior de la ventana Asignaciones avanzadas.

   De forma predeterminada, Workfront marca el primer usuario o rol que asigna a una tarea como Propietario o Asignación principal. No se puede designar a un equipo como propietario principal de una tarea.

   Si no aparece el Propietario principal de la tarea, puede agregar la columna **Es principal** a la tabla.

   >[!IMPORTANT]
   >
   >Según la forma en que el administrador de Workfront o el administrador del grupo hayan configurado las preferencias del proyecto, Workfront podría utilizar la programación del propietario de la tarea para calcular la cronología de la tarea cuando tenga varios usuarios asignados a la tarea. Para obtener información acerca de varias personas asignadas a tareas, vea la sección [Consideraciones sobre asignaciones múltiples a roles, equipos y usuarios](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) del artículo [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

1. Especifique la siguiente información para cada usuario de la columna **Usuario asignado**:

   * (Opcional) **Rol para la facturación**: busque y seleccione el rol para la facturación de este usuario asignado y tarea específicos.

     La función de trabajo para facturación solo se utiliza en esta asignación y no se aplica automáticamente a las demás asignaciones del usuario. Por ejemplo, la función principal de un usuario es Designer, pero en una tarea actúa como Designer sénior y la tasa de facturación debería reflejarlo. La función del puesto para facturación se aplica solo a los usuarios y no se puede utilizar en otras funciones del puesto.

     Cuando se aplica una función de trabajo para la facturación en la asignación del usuario, se puede utilizar la tarifa adjunta a la función de trabajo para la facturación en lugar de las tarifas de usuario o función de trabajo en los cálculos de facturación e ingresos.

     También se puede establecer una función de trabajo de nivel de proyecto para la facturación de un usuario, y ese valor se utiliza en todas las asignaciones del usuario a ese proyecto.

     Para obtener más información, consulte [Configurar un rol para facturación](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

   * **Asignación**: cuando el tipo de duración de una tarea sea Simple, especifique el número de horas que cada usuario o rol debe asignarse a la tarea. La suma de todas las horas asignadas a cada usuario es igual al número que aparece en el campo **Horas planificadas** en la parte superior de la ventana Asignaciones avanzadas. En todos los demás casos, especifique el porcentaje de tiempo (o asignación) que desea que el usuario asignado dedique a resolver la tarea.

     >[!TIP]
     >
     >Después de modificar manualmente las asignaciones de las tareas, las horas planificadas de las tareas podrían actualizarse en consecuencia. Tenga en cuenta que no puede modificar manualmente las asignaciones de los equipos asignados a tareas. Para obtener más información, consulte la sección [Actualizar las horas planificadas de una tarea al administrar las asignaciones de usuario](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) en el artículo [Información general de Horas planificadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

   * **Atributos**: todos los atributos disponibles para el usuario se muestran en los campos de atributos. El administrador configura los atributos y estos se añaden al perfil de usuario o se asocian a un rol en una tarjeta de tasas. Para obtener más información, consulte [Definir atributos de tasa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) y [Editar el perfil de un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

     Actualmente, los atributos son de solo lectura en las asignaciones de usuario. Se pueden editar para los roles.

   * **Divisa de tarifa**: La divisa de las tarifas de facturación y de costo es la predeterminada del proyecto, pero puede cambiar la divisa de esta asignación.

   * (Opcional) **Tarifa de facturación**: La tarifa de facturación puede provenir de otras áreas del sistema, como las tarjetas de tarifas. Para obtener más información, consulte [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). Puede anular manualmente la tarifa de facturación para esta asignación específica en este campo y anulará todas las demás tarifas para el usuario en los cálculos de ingresos.
   * (Opcional) **Tasa de costo**: La tasa de costo puede provenir de otras áreas del sistema. Para obtener más información, consulte [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). Puede reemplazar manualmente la tasa de costo de esta asignación específica en este campo y reemplazará todas las demás tasas para el usuario en los cálculos de costos.
   * **Es facturable**: seleccione esta opción para incluir la asignación en los cálculos financieros. Desactive esta opción para excluir la asignación de los cálculos financieros.

     Este campo está activado de forma predeterminada para todas las asignaciones cuando la tarea tiene un tipo de ingresos.

1. (Opcional) Para ver los datos de asignación por fecha de un usuario o rol, seleccione la fila de la tabla y haga clic en **Ver por fechas** en la barra de acciones de la parte inferior de la ventana Asignaciones avanzadas. Para obtener más información, vea [Ver datos de asignación por fechas](#view-assignment-data-by-dates) en este artículo.
1. (Opcional) Para eliminar una o más asignaciones de la lista, active la casilla de verificación de cada fila y haga clic en **Eliminar** en la barra de acciones de la parte inferior de la ventana Asignaciones avanzadas.
1. Haga clic en **Guardar** o en **Guardar y cerrar** cuando termine de editar las asignaciones avanzadas.

### Agregar y quitar columnas de la lista Asignaciones avanzadas

Los campos deben existir antes de poder agregarlos a la lista.

1. Haga clic en **+** en la parte superior derecha de la lista para abrir el **Administrador de columnas**.

   ![Administrador de columnas de asignaciones avanzadas](assets/aa-column-manager.png)

1. Seleccione la ficha **Propiedades** o la ficha **KPI** para elegir el tipo de campo que desea agregar.

   Las propiedades como ubicación o centro de coste proporcionan información contextual. KPI con fases temporales, como valores de desglose de ingresos o costes, entre períodos de tiempo.

1. Busque un campo de objeto existente en la sección **Disponible** y, a continuación, haga clic en **+** a la derecha del nombre del campo para agregarlo a la columna **Seleccionado**.
1. Haga clic en **-** a la derecha de un campo en la sección **Seleccionado** para quitarlo de la lista.
1. Haga clic en **Guardar**.

   Para obtener más información sobre el administrador de columnas, vea [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Aplicar una vista a la lista Asignaciones avanzadas

Una vista es un conjunto personalizado de disposiciones de columnas que se puede aplicar a la lista.

1. Haga clic en el menú desplegable **Vistas** y seleccione la vista que desee aplicar a la lista.

   **Vistas del sistema** son vistas que agregó el administrador del sistema y no se pueden cambiar. **Mis vistas** son vistas que creó o que compartieron con usted.

1. Haga clic en **Nueva vista** en el menú desplegable **Vistas** para crear una vista.

   Al agregar, quitar o reordenar las columnas, los cambios se guardan automáticamente en la vista. La próxima vez que aplique esta vista, las columnas permanecerán tal como las configuró.

   Para obtener más información sobre las vistas, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Uso de la búsqueda avanzada

La búsqueda avanzada le ayuda a localizar el usuario o la función de trabajo correcta que agregar a la asignación.

1. Para abrir la ventana de búsqueda avanzada, siga uno de estos procedimientos:

   * Haga clic en **Búsqueda avanzada** en la parte superior derecha de la ventana Asignaciones avanzadas.
   * Seleccione una fila de asignación y haga clic en **Búsqueda avanzada** en la barra de acciones de la parte inferior de la ventana Asignaciones avanzadas. Se abrirá la búsqueda avanzada con filtros aplicados automáticamente a esa asignación específica.

1. Seleccione la pestaña Usuarios o Funciones del puesto en la ventana de búsqueda avanzada.
1. Aplique los filtros según sea necesario:

   1. Haga clic en **Filtro** sobre la lista.
   1. En el cuadro Filtro, haga clic en **Agregar condición**.
   1. Seleccione un campo por el que filtrar.
   1. Seleccione un modificador de filtro, como &quot;Tiene cualquiera de&quot;, &quot;No tiene ninguno de&quot;, &quot;Es anterior a&quot; o &quot;Es posterior a&quot;. Las opciones del modificador son diferentes según el tipo de campo por el que esté filtrando.
   1. Seleccione el valor o los valores del campo. Según el tipo de campo por el que filtre, se le puede pedir que seleccione el elemento de una lista, lo busque o utilice un calendario para seleccionar un intervalo de fechas.

   El filtro se aplica automáticamente a la lista. Para obtener más información sobre los filtros, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

1. Busque un rol o un usuario.

   Al buscar un usuario que coincida con una asignación de rol, solo se muestran las coincidencias completas (rol y todos los atributos).

1. Haga clic en **+** para agregar columnas a la tabla. Para obtener más información, consulte [Agregar y quitar columnas en la lista de asignaciones avanzadas](#add-and-remove-columns-on-the-advanced-assignments-list).
1. Seleccione uno o más usuarios o roles y haga clic en **Agregar usuarios** o **Agregar roles** en la barra de acciones de la parte inferior de la ventana.

   Las asignaciones se añaden a la ventana Asignaciones Avanzadas.

### Ver datos de asignación por fechas

La ventana **Ver por fechas** para asignaciones avanzadas muestra todo el historial con fecha en vigor de la asignación de un usuario o rol específico. Se muestran los cambios pasados y futuros.

Algunos ejemplos de elementos con fecha en vigor que podrían afectar al historial de asignaciones son:

* Funciones principales/otras funciones del usuario
* Rol de nivel de proyecto para facturación
* Tarifas de facturación/coste del perfil de usuario
* Tarifas de facturación/costo de anulación del proyecto (usuario o rol)
* Tasar tasas de tarjeta por rol/atributos
* Atributos del usuario
* Programación de usuario

Tenga en cuenta que no se trata de una lista completa y que el campo que ha cambiado no se muestra necesariamente en la tabla de datos de asignación, pero afecta a las tasas de facturación y de costo o a los atributos del usuario o rol.

Sólo puede ver datos de asignación por fechas para un único usuario o rol.

1. Seleccione la fila de tabla de un usuario o rol y haga clic en **Ver por fechas** en la barra de acciones de la parte inferior de la ventana Asignaciones avanzadas.

   Aparece la ventana **Ver por fechas**. Los datos son de solo lectura.

   Cada fila de la tabla representa un cambio con fecha en vigor en la asignación. Si no se han realizado cambios con fecha efectiva, la tabla tendrá una fila que mostrará los datos actuales. Los campos resaltados indican lo que ha cambiado y se indica la fecha de inicio y finalización de cada actualización. Por ejemplo, si la tasa de facturación cambió de 202 el 20 de agosto a 205 el 21 de agosto, la tasa se resaltará. El texto entre paréntesis indica dónde se realizó el cambio en la tasa, como un proyecto.

   ![Ver por ventana de fechas](assets/resource-changes-view-by-dates.png)

   Cuando termine de revisar los datos, haga clic en la flecha situada en la parte superior izquierda para volver a la ventana Asignaciones avanzadas.

## Crear asignaciones avanzadas para todos los demás paquetes

Este diseño de Asignaciones avanzadas se aplica tanto a tareas como a problemas.

1. Vaya al proyecto donde desea asignar una tarea o un problema.
1. Haga clic en **Tareas** o **Problemas** en el panel izquierdo y, a continuación, haga clic en el nombre de una tarea o problema en la lista.

   >[!TIP]
   >
   >Puede realizar asignaciones avanzadas directamente en la lista de tareas o problemas. Haga clic dentro del campo **Asignaciones** en la misma línea que la tarea o el problema y, a continuación, haga clic en **Avanzadas** en la parte inferior de la lista o en el **icono Personas** en la esquina superior derecha del cuadro de asignaciones para abrir la ventana Asignaciones avanzadas. Pase al paso 5 para continuar creando asignaciones avanzadas.
   >![Haga clic en Avanzadas o en el icono Personas](assets/access-aa-from-lists.png)

1. Haga clic en **Asignar a** en el campo **Asignaciones** del encabezado de la tarea o el problema

   O

   Haga clic en uno de los nombres asignados si la tarea o el problema ya están asignados.

1. Haga clic en **Avanzadas**.

   ![Haga clic en Avanzadas](assets/assignments-from-task-header-0825.png)

1. En el campo **Buscar personas, roles y equipos**, empiece a escribir el nombre de un usuario, rol o equipo y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.

   >[!NOTE]
   >
   >Si el nombre del usuario contiene un carácter especial, debe incluirlo en el campo de búsqueda.

1. (Opcional) Siga agregando usuarios asignados en el cuadro **Buscar personas, roles y equipos** para agregar varios recursos a la tarea o al problema.

   >[!TIP]
   >
   >* Puede asignar varios usuarios, funciones o equipos. Solo puede asignar usuarios, funciones y equipos activos.
   >
   >
   >* Al añadir una asignación de usuario, observe el avatar, la función principal del usuario o su dirección de correo electrónico para distinguir entre usuarios con nombres idénticos.
   >Los usuarios deben estar asociados con al menos una función para verla a medida que los añade.
   >Debe tener habilitada la configuración Ver información de contacto en su nivel de acceso para que los usuarios vean los correos electrónicos de los usuarios. Para obtener más información, consulte [Conceder acceso a usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Si un usuario, un rol o un equipo se han asignado antes de que se desactiven, permanecerán asignados al elemento de trabajo. En este caso, se recomienda lo siguiente:
   >   
   >   * Reasignar el elemento de trabajo a los recursos activos.
   >   * Asocie los usuarios de un equipo desactivado a un equipo activo y reasigne el elemento de trabajo al equipo activo.

1. Especifique la siguiente información para cada usuario de la columna **Usuario asignado**:

   * **Propietario**: pase el puntero por encima del nombre del usuario asignado y haga clic en **Convertir en principal** en el campo Propietario si desea marcar al usuario asignado como propietario de la tarea o problema. La casilla de verificación verde indica que el usuario especificado es el contacto principal de la tarea o el problema. Adobe Workfront marca el primer usuario o función que asigna a una tarea o problema como Asignación principal o Propietario. No se puede designar a un equipo como propietario principal de una tarea o un problema.

     >[!IMPORTANT]
     >
     >Según la forma en que el administrador de Workfront o el administrador del grupo hayan configurado las preferencias del proyecto, Workfront podría utilizar la programación del propietario de la tarea para calcular la cronología de la tarea cuando tenga varios usuarios asignados a la tarea. Para obtener información acerca de varias personas asignadas a tareas, vea la sección [Consideraciones sobre asignaciones múltiples a roles, equipos y usuarios](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) del artículo [Asignar tareas](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Asignaciones**: cuando el tipo de duración de una tarea sea Simple, especifique el número de horas que cada usuario o rol debe asignarse a la tarea. La suma de todas las horas asignadas a cada usuario es igual al número que aparece en el campo **Horas planificadas** en la parte inferior de la columna Asignaciones. En todos los demás casos, especifique el porcentaje de tiempo (o asignación) que desea que el usuario asignado dedique a resolver la tarea o el problema.

     >[!TIP]
     >   
     >   * Después de modificar manualmente las asignaciones de las tareas, las horas planificadas de las tareas podrían actualizarse en consecuencia. Para obtener más información, consulte la sección [Actualizar las horas planificadas de una tarea al administrar las asignaciones de usuario](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) en el artículo [Información general de Horas planificadas](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).
     >   * No se pueden modificar manualmente las asignaciones de los problemas.
     >   * No se pueden modificar manualmente las asignaciones de los equipos asignados a las tareas.

   * **Función del usuario asignado:** seleccione la función que el usuario debe usar al desempeñar esta asignación.  La función principal del usuario se muestra de forma predeterminada. Haga clic en el cuadro **Rol de asignado** para seleccionar otro rol. Al asignar primero la tarea o el problema a una función y, a continuación, añadir un usuario que pueda cumplir dicha función como segunda asignación, la lista de usuarios sugeridos se filtra para los usuarios que pueden cumplir las funciones ya asignadas a la tarea y al problema.

     ![Función del usuario asignado](assets/advanced-assignments-select-role.png)

   * **Tipo de duración**: esta opción solo está disponible para tareas. Haga clic en el nombre del tipo de duración y seleccione un tipo de duración en el menú desplegable. Para obtener más información sobre los tipos de duración, consulte [Información general sobre la duración de la tarea y los tipos de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duración:** puede actualizar este campo para una tarea cuando disponga de permisos de administración para la tarea.

     Para obtener más información, consulte [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Al editar en lotes la información de la asignación, aparece un cuadro de diálogo similar para asignar usuarios, horas, asignación y el propietario de la tarea.

   * **Horas planificadas**: cuando el tipo de duración sea Asignación calculada o Simple, actualice el número de horas planificadas. Como resultado, los porcentajes de asignación o las horas de cada recurso se distribuyen de forma uniforme. Workfront calcula las horas planificadas cuando el tipo de duración es Trabajo calculado o Condicionado por el esfuerzo. Para obtener más información, consulte [Información general sobre la duración de la tarea y el tipo de duración](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. Haga clic en **Guardar**.


