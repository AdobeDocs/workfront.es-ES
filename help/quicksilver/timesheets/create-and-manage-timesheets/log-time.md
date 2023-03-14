---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Tiempo de registro
description: Puede registrar el tiempo para los elementos de trabajo en &nbsp;Adobe Workfront para indicar la cantidad de horas que emplea trabajando en ellos. También puede registrar el tiempo que no está relacionado con el trabajo, como vacaciones, tiempo de enfermedad o tiempo que pasa en reuniones. La hora de registro se muestra en el parte de horas.
author: Alina
feature: Timesheets
exl-id: 120173a8-95f1-4233-ab40-d3bcfe38c977
source-git-commit: b2859f3d268bd947fba5bb0280677465b3039d93
workflow-type: tm+mt
source-wordcount: '2992'
ht-degree: 0%

---

# Tiempo de registro

Puede registrar el tiempo para los elementos de trabajo en Adobe Workfront para indicar la cantidad de horas que emplea trabajando en ellos. También puede registrar el tiempo que no está relacionado con el trabajo, como vacaciones, tiempo de enfermedad o tiempo que pasa en reuniones. La hora de registro se muestra en el parte de horas.

Para obtener más información sobre el tipo de horas en las que puede iniciar sesión en Workfront, consulte [Administrar tipos de hora](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Requisitos de acceso

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p>
   <p>Legacy license: 
   <ul><li>Review or higher to log General Hours in a timesheet</li>
   <li>Work or higher to log hours on a project, task, or issue</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the type of work item you log time for </p> <p>For example, you need Edit access to Issues, to log time for issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions on the work item you log time for that includes permissions to Log Hours</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Debe tener el siguiente acceso para realizar los pasos de este artículo y registrar las horas específicas del proyecto:

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
   <td> <ul><li>Revise o superior para registrar las horas generales en un parte de horas</li>
   <li> Trabajo o superior para iniciar sesión en un proyecto, tarea o problema</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso al tipo de elemento de trabajo para el que se registra la hora </p> <p>Por ejemplo, necesita editar el acceso a problemas para registrar la hora de los problemas</p> <p>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores en el elemento de trabajo para el que registra tiempo que incluye permisos para horas de registro.</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones al iniciar sesión en Workfront

* Puede registrar la hora de los proyectos, tareas o problemas, o puede registrar la hora directamente en su parte de horas.

   Para obtener información sobre la creación de partes de horas, consulte [Crear un parte de horas de un solo uso](../../timesheets/create-and-manage-timesheets/create-tmshts.md).

* Todo el tiempo registrado mediante herramientas que no sean la hoja de horas aparece en el parte de horas del período de tiempo correspondiente.
* Las tareas y los problemas de un proyecto que no es actual no se rellenan previamente en un parte de horas.
* El tiempo registrado en el parte de horas se aplica inmediatamente a la tarea, el problema o el proyecto.
* Las hojas de tiempo incluyen el tiempo total de todas las fechas registradas. Los fines de semana siempre se incluyen, incluso cuando los cálculos de la cronología se han configurado para excluirlos (como se describe en [Configurar las preferencias de proyecto de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)).
* El número máximo de elementos mostrados en un parte de horas es de 45. Si hay más de 45 elementos cuyas fechas coinciden con el lapso de tiempo del parte de horas, solo se muestran los elementos actualizados más recientemente.
* Las entradas de hora incluidas en los registros de facturación están atenuadas y no se pueden editar en el parte de horas. Para obtener más información, consulte [Crear registros de facturación](../../manage-work/projects/project-finances/create-billing-records.md).

## Tiempo de registro

Puede iniciar sesión en las siguientes áreas de Workfront:

* [Hoja de horas](#timesheet)
* [Página de inicio](#home)
* [Proyecto, tarea o problema](#project-task-or-issue)
* [Panel de resumen](#summary-panel)
* [Tableros](#boards)
* [Aplicación móvil](#mobile-app)

### Hoja de horas {#timesheet}

Puede registrar horas generales u horas específicas del proyecto en un parte de horas.

>[!NOTE]
>
>Los usuarios de revisión asignados a un perfil de parte de horas pueden ver la ficha Hojas de horas y registrar las horas generales. Sin embargo, no pueden registrar horas en ninguna tarea o problema asignado que aparezca en el parte de horas.

1. Haga clic en el [!UICONTROL **Menú principal**] icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront.

1. Haga clic en [!UICONTROL **Hojas de tiempo**]. El parte de horas actual se muestra de forma predeterminada.
   ![Hoja de horas](assets/timesheet-redesigned-nwe.png)

   El parte de horas se rellena previamente con elementos asignados a usted durante el lapso de tiempo del parte de horas. Para obtener información sobre cómo se rellenan previamente las partes de horas, consulte [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md). Si no ve un elemento en el parte de horas, puede agregarlo.

   >[!NOTE]
   >
   >El parte de horas rellena previamente solo con elementos asignados a usted. No se rellena previamente con elementos asignados a sus equipos o funciones de trabajo.
   >
   >Al hacer clic en Trabajar en él en un elemento asignado a sus equipos, se le asigna el elemento y éste se mostrará en su parte de horas.


1. (Opcional) Haga clic en el **pantalla completa** icono ![](assets/full-screen.png) para mostrar el parte de horas en modo de pantalla completa, haga clic en el botón **exit-full-screen** ![](assets/exit-full-screen.png) para volver al parte de horas.

   <!-- drafted for the resize columns in timesheet story: 1. (optional) Click on the separator lines between weeks or between the time frame area and the work item area to resize the columns of the timesheet.-->

1. (Opcional) Para agregar un proyecto, tarea o problema al parte de horas, haga clic en el botón **Agregar elemento** menú desplegable en la esquina superior izquierda del parte de horas y haga clic en **Agregar proyectos**, **Agregar tareas** o **Agregar problemas**.

   Se muestra una lista de proyectos, tareas o problemas.

   <!--drafted for full screen mode for add projects story - align it with the rest of the steps when you enable this:: 1. (Optional) Click the **full-screen** icon ![](assets/full-screen.png) to display the list of objects in full-screen mode.-->

1. (Opcional) Haga clic en el icono de búsqueda ![Buscar un elemento](assets/search-icon.png) para buscar un elemento específico usando una palabra clave que agregar al parte de horas.

1. (Opcional) Expanda los menús desplegables de filtro, vista o agrupación para aplicar o personalizar uno y para ver la información del elemento que desee.

1. Seleccione uno o varios elementos de la lista y haga clic en **Agregar**.

   >[!NOTE]
   >
   >Al agregar tareas o problemas al parte de horas, también se agrega el proyecto.


1. (Condicional) Si agrega 50 o más elementos al mismo tiempo, aparece un mensaje de confirmación que muestra el número de elementos agregados a su parte de horas.

   Haga clic en **Agregar todo** para agregar todos los elementos o haga clic en **Cancelar** para detener la adición de los elementos seleccionados, **Cancelar** para cerrar la lista de elementos.

   Las tareas y los problemas se enumeran bajo el nombre del proyecto.

   >[!NOTE]
   >
   >Los elementos que agregue manualmente al parte de horas están anclados y permanecerán en las partes de horas actuales y futuras hasta que los desfije manualmente para eliminarlos. Para obtener información sobre cómo desanclar elementos para eliminarlos del parte de horas, continúe con el paso 10.

   <!--(ensure this stays accurate)-->

1. (Opcional) Haga clic en el **Contraer** ![](assets/collapse-icon.png) o **Expandir** ![](assets/expand-icon.png) junto al nombre del proyecto para mostrar u ocultar la lista de tareas y problemas del proyecto.


   >[!TIP]
   >
   >   Cuando utilice un teclado QWERTY estándar y después de hacer clic en el nombre de un proyecto en el parte de horas, presione el siguiente conjunto de teclas para contraer o expandir el proyecto:
   >   * Para expandir el proyecto y mostrar sus elementos de trabajo:
      >     * Mayús + Alt + flecha arriba para equipos con Windows
      >     * Mayús + Opción + Flecha arriba para equipos Mac
   >   * Para contraer el proyecto y ocultar sus elementos de trabajo:
      >     * Mayús + Alt + flecha abajo para equipos con Windows
      >     * Mayús + Opción + Flecha abajo para equipos Mac.



1. (Opcional) Para fijar manualmente un elemento que se muestra en el parte de horas automáticamente, pase el ratón sobre el nombre del elemento y haga clic en el botón **pin** icono ![](assets/empty-pin-icon.png).

   >[!TIP]
   >
   >   Cuando utilice un teclado QWERTY estándar después de hacer clic en un elemento del parte de horas, presione el siguiente conjunto de teclas para fijar un elemento:
   >   * Opción + P para equipos con Windows y Mac.



1. (Opcional) Haga clic en el icono de búsqueda ![](assets/search-icon.png) y empiece a escribir una palabra clave para encontrar un proyecto, una tarea o un problema en el parte de horas.

1. (Opcional) Puede quitar un elemento (proyecto, tarea o problema) del parte de horas si ha agregado manualmente el elemento (como se describe en los pasos 3 a 6) y si todavía no ha registrado el tiempo en su contra desmontándolo. <!--ensure this stays accurate-->

   No puede quitar elementos que se incluyan automáticamente en el parte de horas de acuerdo con las preferencias del parte de horas del sistema o grupo de Workfront que estén configurados para rellenar previamente los partes de horas (como se describe en [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   Para quitar un elemento del parte de horas que se agregó manualmente:

   1. Asegúrese de que no se haya registrado ningún tiempo en el elemento.
   1. Haga clic en el **desanclar** icono ![Incrustar un elemento](assets/pin-icon.png) junto al elemento para desanclar el elemento del parte de horas.

   >[!TIP]
   >
   >   Cuando utilice un teclado QWERTY estándar después de hacer clic en un elemento del parte de horas, presione el siguiente conjunto de teclas para desanclar un elemento:
   >   * Opción + P para equipos con Windows y Mac.



   El elemento se elimina del parte de horas después de actualizar la página.

1. (Condicional) Si su administrador de Workfront o de grupo ha habilitado la variable **Asignar roles de trabajo a las entradas de hora manualmente** , seleccione una función de trabajo en el menú desplegable. La función especificada cuando se le asigna el elemento de trabajo se muestra de forma predeterminada. Si no se le asigna una función en el objeto, la función principal se mostrará como predeterminada. Para obtener más información sobre esta configuración, consulte el artículo [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

   ![Tiempo de registro de varias funciones en el parte de horas](assets/job-role-plus-sign-and-boxes-in-redesigned-timesheet.png)


1. (Opcional) Haga clic en el **+** para agregar otra fila, seleccione un tipo de hora nueva en el menú desplegable del [!UICONTROL Tipo de hora] para registrar la hora de un tipo de hora diferente.

   ![Menú desplegable Tipo de hora](assets/hour-type-drop-down-expanded-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Según el sistema operativo o navegador y cuando utilice un teclado QWERTY estándar, presione el siguiente conjunto de teclas para añadir otra fila:
   >   * Ctrl + Opción + + para equipos con Windows
   >   * Cmd + Opción + + para equipos Mac


   Los tipos de hora están disponibles en función de lo que se haya definido en los niveles de sistema, proyecto y usuario, tal como se describe en [Definir tipos de hora y disponibilidad para hojas de hora](define-hour-types-and-availability.md).

   El tipo de hora no se puede cambiar después de cerrar un parte de horas.

   >[!TIP]
   >
   >Si anteriormente registró la hora y el tipo de hora seleccionado está ahora desactivado, toda la fila de la hora registrada se verá atenuada. Al seleccionar otro tipo de hora y actualizar la página, se elimina la opción de tipo hora desactivada de la lista desplegable, por lo que no se pueden agregar horas adicionales a ese tipo de hora.
   >
   >Considere la posibilidad de agregar una nueva línea para el elemento de trabajo para el que desee registrar tiempos adicionales y seleccionar un nuevo tipo de hora, si desea mantener el tipo de hora desactivado asociado con la hora registrada anterior.

1. Haga clic en el **delete** icono  ![](assets/delete.png) junto a la función de trabajo para eliminarla. También se eliminará cualquier tiempo registrado para la función.

   >[!TIP]
   >
   >   Según el sistema operativo o navegador y cuando utilice un teclado QWERTY estándar, presione el siguiente conjunto de teclas para eliminar una fila:
   >   * Ctrl + Opción + - para equipos con Windows
   >   * Cmd + Opción + - para equipos Mac



1. Especifique la cantidad de tiempo durante la cual desee iniciar sesión en un día determinado en la sección de cronología del parte de horas y, a continuación, haga clic fuera del cuadro de hora para guardar la entrada de hora. Las horas se guardan automáticamente. La fila para la que se registra la hora se resalta en azul claro y el cuadro de entrada de la hora se muestra en azul oscuro.

   ![Cuadro de tiempo de registro en la hoja de horas](assets/log-time-with-blue-hightlight-redesigned-timesheet.png)

   La hora se registra en horas o días. Esta configuración la configuran los usuarios con una licencia de Plan o el administrador del sistema, tal como se describe en [Configure si la hora se registra en horas o días](../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md).

   >[!IMPORTANT]
   >
   >Si la función de trabajo para la que ha registrado ha cambiado y la variable **Asignar roles de trabajo a las entradas de hora manualmente** se ha desactivado, debe guardar manualmente las entradas de tiempo. El parte de horas volverá a ahorrar tiempo automáticamente solo cuando ya no haya ningún tiempo registrado para la función de trabajo que ha cambiado.
   >
   >Si la función ha cambiado y la variable **Asignar roles de trabajo a las entradas de hora manualmente** está activada, puede registrar la hora o actualizar la función y los cambios se guardarán automáticamente.

1. (Opcional) Especifique la cantidad de horas extra en el campo Horas extra del encabezado del parte de horas.

   >[!TIP]
   >
   >No puede registrar un número mayor de horas extra que el total actual de horas en el parte de horas. Por ejemplo, si ha registrado 7 horas en el parte de horas hasta ahora, no puede registrar 8 horas extra.

1. (Opcional) Haga clic en **Comentario** para agregar un comentario para la entrada de hora.

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Cuando utilice un teclado QWERTY estándar después de hacer clic en el cuadro de entrada de hora, presione el siguiente conjunto de teclas para abrir el cuadro de comentarios:
   >   * Mayús + F2 para equipos con Windows y Mac.


1. Haga clic en **Listo** para guardar el comentario.

   >[!TIP]
   >
   >   Cuando utilice un teclado QWERTY estándar, desde el cuadro de comentarios, presione el siguiente conjunto de teclas para guardar el comentario:
   >   * Ctrl + Intro para equipos con Windows.
   >   * Cmd + Retorno para equipos Mac.



1. (Opcional) Haga clic en **Mostrar comentarios** en la barra de herramientas para mostrar los comentarios de entrada por hora en el elemento de trabajo.

   ![Comentarios enumerados bajo elemento en hoja de horas](assets/comments-expanded-under-tasks-redesigned-timesheet.png)

   >[!TIP]
   >
   >   Todos los cambios realizados en el parte de horas se guardan automáticamente.

1. (Opcional) Haga clic en la fila de una tarea o problema y, a continuación, haga clic en **Abrir resumen** en la esquina superior derecha del parte de horas para añadir una actualización o actualizar información sobre la tarea o el problema. El panel Resumen se abre a la derecha.

   ![summary-panel-for-task-opened-in-timesheet](assets/summary-panel-for-task-opened-in-timesheet-redesigned-timesheet.png)

   La actualización se muestra en el área Actualizaciones del elemento de trabajo asociado con la hora registrada.

   >[!TIP]
   >
   >No se pueden comentar proyectos ni entradas de hora de la hora general.

1. Haga clic en [!UICONTROL **Cerrar resumen**] para cerrar el panel Resumen y volver al parte de horas.

1. (Opcional) Haga clic en [!UICONTROL **Actualizaciones**] en el panel izquierdo, agregue una actualización al parte de horas. Para obtener más información sobre las actualizaciones de Workfront, consulte [Actualizar trabajo](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   ![enter-an-update-in-redesign-timesheet-left-panel](assets/enter-an-update-in-redesigned-timesheet-left-panel.png)

   * **Cerrar**: Cierre el parte de horas cuando termine de actualizarlo. Esta opción solo está disponible cuando el parte de horas no está asociado con un aprobador.

   * **Enviar para aprobación:** Esta opción solo está disponible si hay un aprobador en el parte de horas. Guarde los cambios y envíe para su aprobación. Puede abrir el parte de horas después de cerrarlo haciendo clic en **Recordar**, si todavía no se ha concedido una aprobación. Para obtener más información, consulte [Enviar un parte de horas para su aprobación](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md).

   * **Rechazar**: Esta opción se muestra cuando es aprobador de hojas de horas y el parte de horas se le ha enviado para su aprobación. Al hacer clic en él, se cambia el estado del parte de horas a Rechazado y el parte de horas permanece abierto.

   * **Aprobar**: Esta opción se muestra cuando es aprobador de hojas de horas y el parte de horas se le ha enviado para su aprobación. Al hacer clic en él, se cambia el estado del parte de horas a Aprobado y se cierra el parte de horas.
   >[!TIP]
   >
   >Las opciones Rechazar y Aprobar también se muestran en el parte de horas cuando es administrador del sistema y el parte de horas está asociado con un aprobador.

1. (Condicional) Si ha cerrado o enviado su parte de horas para su aprobación, haga clic en una de las siguientes opciones:

   * **Volver a abrir**: Esta opción está disponible para hojas de tiempo que ya se han cerrado y que no tienen aprobadores o partes de horas que ya se han aprobado. Vuelva a abrir el parte de horas para modificar las entradas de hora.
   * **Recordar**: Esta opción está disponible para hojas de tiempo que se han enviado para aprobación pero que aún no se han aprobado ni rechazado. Haga clic en **Recordar** para volver a abrir el parte de horas y modificar las entradas de hora.

### Página de inicio {#home}

Puede registrar la hora específica del proyecto en Inicio.

Para obtener información general sobre el uso del área principal, consulte [Uso del área de inicio](../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md).

Para iniciar sesión en un elemento de trabajo del área de inicio:

1. En el **Lista de trabajo** , seleccione el elemento en el que desea registrar la hora.
1. En el panel derecho, haga clic en **Tiempo de registro**.

   ![](assets/log-time-home-350x181.png)

1. En el **Introducir horas** menú desplegable, seleccione el tipo de hora correspondiente.\
   Los tipos de hora están disponibles en función de lo que se haya definido en los niveles de sistema, proyecto y usuario, tal como se describe en [Definir tipos de hora y disponibilidad para hojas de hora](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
1. (Condicional) Si su administrador de Workfront o de grupo ha habilitado la variable **Asignar roles de trabajo a las entradas de hora manualmente** , seleccione una función de trabajo en el menú desplegable. La función especificada cuando se le asigna el elemento de trabajo se muestra de forma predeterminada. Si no se le asigna una función en el objeto, la función principal se mostrará como predeterminada. Para obtener más información sobre esta configuración, consulte el artículo [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).
1. Especifique la hora a la que desee registrar y haga clic en **Tiempo de registro**.

### Proyecto, tarea o problema {#project-task-or-issue}

Puede registrar la hora específica del proyecto en un proyecto, tarea o problema.

#### Permisos necesarios para el tiempo de registro

Para registrar horas en un proyecto, tarea o problema, debe tener permisos específicos. Puede registrar la hora en dos lugares de un proyecto, tarea o problema:

* [Ficha Actualizaciones](#updates-tab)
* [Ficha Horas](#hours-tab)

##### Ficha Actualizaciones{#updates-tab}

Para poder registrar horas en la ficha Actualizaciones de un proyecto, tarea o problema, es necesario lo siguiente:

* Debe tener una licencia de trabajo o de plan.
* Debe tener al menos permisos de Contribute para el proyecto, la tarea o el problema con acceso a Horario de registro.\
   Para obtener más información sobre la concesión de permisos en proyectos, consulte [Uso compartido de un proyecto en Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* Si desea registrar la hora directamente en un proyecto, su administrador de Workfront debe habilitar el tiempo de registro directamente en los proyectos que se establecen en [!UICONTROL **Hoja de horas y horas** ]> [!UICONTROL **Preferencias**].\
   Para obtener más información sobre cómo permitir que los usuarios registren horas directamente en los proyectos, consulte [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

##### Ficha Horas{#hours-tab}

Para poder registrar horas en la ficha Horas de un proyecto, tarea o problema, es necesario lo siguiente:

* Debe ser el administrador del sistema.

O debe tener todo lo siguiente:

* Debe tener una licencia de Plan con acceso administrativo a Hojas de horas y horas. Para obtener más información sobre la concesión de acceso administrativo a hojas de horas y horas, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).
* Debe tener al menos permisos de Contribute para el proyecto con acceso a Horario de registro. Para obtener más información sobre la concesión de permisos en proyectos, consulte [Uso compartido de un proyecto en Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
* Si desea registrar la hora directamente en un proyecto, su administrador de Workfront debe habilitar la opción Registrar la hora directamente en los proyectos, en la opción Hoja de horas y horas > Preferencias. Para obtener más información sobre cómo permitir que los usuarios registren horas directamente en los proyectos, consulte [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para iniciar sesión en un proyecto, tarea o problema:

1. Vaya a un proyecto, tarea o problema.
1. En el panel izquierdo, seleccione **Horas**.
1. Haga clic en **Tiempo de registro**.

   Aparece el cuadro de diálogo Horario de registro .

1. Especifique la siguiente información:

   * **Propietario:** Su nombre se muestra en este campo de forma predeterminada.\
      Si está registrando las horas para otro usuario, especifique su nombre.

   * **Horas**: Introduzca el número de horas para el proyecto, la tarea o el problema.
   * **Tipo de hora**: Seleccione un tipo de hora en el menú desplegable, si es diferente del que se muestra de forma predeterminada.

      Las opciones pueden variar en función de los tipos de hora configurados en el sistema. Para obtener más información sobre la configuración de tipos de hora, consulte [Definir tipos de hora y disponibilidad para hojas de hora](../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   * **Función del trabajo**: (Condicional) Si su administrador de Workfront o de grupo ha habilitado la variable **Asignar roles de trabajo a las entradas de hora manualmente** , seleccione un **Función del trabajo** en el menú desplegable. La Función especificada cuando se asigna al objeto se muestra de forma predeterminada. Si no se le asigna una función en el objeto, la función principal se mostrará como predeterminada. Para obtener más información sobre esta configuración, consulte el artículo [Configuración de las preferencias de horas y horas](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

      ![Screen_Shot_2017-05-03_at_10.16.52_AM.png](assets/screen-shot-2017-05-03-at-10.16.52-am-350x346.png)

1. Haga clic en **Horas de registro**.

### Panel de resumen

Puede registrar la hora de las tareas y los problemas en el panel Resumen.
Para obtener más información, consulte [Resumen](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

![](assets/summary-hour-log.png)

### Tableros {#boards}

>[!NOTE]
>
>Esta función solo está disponible a través de la opción de inclusión de las funciones iniciales para Workfront Board.

Puede iniciar sesión en tarjetas conectadas en un tablero de Workfront. Este es el mismo proceso que iniciar sesión en una tarea o problema, y las horas registradas en la tarjeta se guardan en la tarea o problema conectado.
Para obtener más información, consulte [Usar tarjetas conectadas en tableros](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

### Aplicación móvil {#mobile-app}

Puede registrar la hora desde la aplicación móvil de Workfront.
Para obtener más información, consulte [Adobe Workfront para Android](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md) o [Adobe Workfront para iOS](/help/quicksilver/workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md).
