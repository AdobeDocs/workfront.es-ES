---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configuración de las preferencias de horas y horas
description: Como [!DNL Adobe Workfront] administrador, puede especificar preferencias para hojas de horas y horas en [!DNL Workfront] para definir con qué elementos se pueden rellenar previamente las hojas de hora y con qué elementos pueden registrar los usuarios.
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 1%

---

# Configuración de las preferencias de horas y horas

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como [!DNL Adobe Workfront] administrador, puede especificar preferencias para hojas de horas y horas en [!DNL Workfront] para definir con qué elementos se pueden rellenar previamente las hojas de hora y con qué elementos pueden registrar los usuarios.

Los cambios que realice en las hojas de horas afectarán a todas las hojas de horas que se creen en el futuro.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador.</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Definir preferencias de horario y hora

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Hoja de horas y horas]** > **[!UICONTROL Preferencias]**.

1. En la página que se muestra, en la sección **[!UICONTROL Preferencias generales]** , configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Hora de registro para fechas futuras]</td> 
      <td> <p>Permite a los usuarios registrar la hora de las fechas futuras en todo el sistema en:</p> 
       <ul> 
        <li>Todos los proyectos, tareas y problemas en los que tengan acceso al tiempo de registro</li> 
        <li>Sus partes de horas como hora general</li> 
       </ul> <p>Esto resulta útil cuando los usuarios planean estar fuera de la oficina y desean hacerlo antes.</p> <p><b>NOTA</b>: No puede impedir que los usuarios inicien sesión en tareas o problemas que se hayan cerrado o cancelado. Solo puede evitar que los usuarios inicien sesión en proyectos completos o en ejecución. Se recomienda utilizar filtros en listas de tareas y problemas para excluir los que se han completado o cancelado de la visibilidad de los usuarios.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Asignar roles de trabajo a las entradas de hora manualmente]</td> 
      <td> <p>Permita a los usuarios seleccionar manualmente cualquier función de trabajo asignada en su perfil de usuario o asignada al objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Si deshabilita esta configuración después de asignar funciones de trabajo a entradas de hora, los usuarios deben ajustar las horas registradas en las distintas funciones en la ficha [!UICONTROL Hours] del proyecto, la tarea o el problema.</li> 
         <li>Si el usuario no tiene una función de trabajo asignada en su perfil y hay una tarea asignada como [!UICONTROL Task Owner] en el cuadro de diálogo [!UICONTROL Advanced Asscriptions], esa función de trabajo aparece cuando el usuario inicia sesión en la tarea.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir edición de parte de horas a propietarios y administradores]</td> 
      <td> <p>Restringir la edición a propietarios de hojas de horas y [!DNL Workfront] administradores. Cuando esta opción está deshabilitada, las hojas de horas también se pueden editar:</p> 
       <ul> 
        <li> <p>Usuarios con acceso administrativo a hojas de horas y horas en su nivel de acceso</p> </li> 
        <li> <p>Aprobadores de parte de horas si "Puede editar horas" está habilitado en el parte de horas</p> </li> 
        <li> <p>El administrador del propietario del parte de horas</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir la edición de horas a propietarios y administradores]</td> 
      <td>Restringir la edición al usuario que ha introducido las horas y [!DNL Workfront] administradores. Esta configuración se aplica a la ficha [!UICONTROL Hours] de un proyecto o a un informe de horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. En el **[!UICONTROL Tiempo de registro]** , configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Registrar el tiempo directamente en los proyectos]</td>
        <td>Permite a los usuarios iniciar sesión en el proyecto (tanto en la ficha [!UICONTROL Actualizaciones] como en el parte de horas). Si los usuarios no registran la hora a nivel de proyecto, estas opciones deben permanecer sin marcar.</td>
    </tr>
    <tr>
        <td>Registrar tiempo en proyectos completos</td>
        <td>Permite a los usuarios registrar la hora en un proyecto que se haya marcado como completado. Si esta opción está desactivada, los usuarios no pueden registrar la hora del trabajo que han completado en proyectos en el estado [!UICONTROL Complete].</td>
    </tr>
    <tr>
        <td>Registrar tiempo en proyectos inactivos</td>
        <td>Cuando esta opción está habilitada, los usuarios pueden iniciar sesión durante horas en los proyectos con el estado [!UICONTROL Dead].</td>
    </tr>
   </table>

1. En el **[!UICONTROL Rellenar partes de horas previamente con]**&#x200B; sección, configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Trabajo que se encuentra dentro de] &lt;number of="" weeks=""&gt; [!UICONTROL del rango de trabajo del parte de horas]</td> 
      <td> <p>Define el número de semanas antes y después del intervalo de fechas del parte de horas que contiene fechas de tareas y problemas asignados al usuario. El valor predeterminado es 1 semana y se puede ampliar este intervalo a 4 semanas. Esto significa que el parte de horas se rellena previamente con tareas y problemas que tienen fechas entre cuatro semanas antes del intervalo de fechas del parte de horas y hasta cuatro semanas después del intervalo de fechas del parte de horas, si selecciona 4 semanas para el intervalo. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tareas y problemas que se han completado]</td> 
      <td>Si se asignan varios recursos a una sola tarea, se recomienda esta configuración. Esto significa que cuando un recurso registra la hora en la tarea y la marca como completa, los demás recursos asignados a la tarea aún pueden encontrar la tarea o el problema en su parte de horas, para registrar sus horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tareas y problemas que tienen fechas planificadas en el intervalo de fechas del parte de horas]</td> 
      <td> <p>Cuando se selecciona, el parte de horas incluye tareas y problemas que tienen una Fecha de inicio planificada o una Fecha de finalización que se encuentra dentro del intervalo de fechas del parte de horas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tareas que tienen fechas proyectadas en el intervalo de fechas del parte de horas]</td> 
      <td> <p>Cuando se selecciona, el parte de horas incluye tareas que tienen una Fecha de inicio prevista o una Fecha de finalización comprendida dentro del lapso de tiempo del proyecto, incluso si la fecha planificada del problema o la tarea queda fuera del intervalo de fechas del parte de horas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **[!UICONTROL Preferencias de eliminación de proyectos, tareas o problemas]** especifique lo siguiente:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Better title would be Deleting projects, tasks, and issues</p>
   -->

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Al eliminar proyectos]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Mantener el tiempo registrado ya agregado a las hojas de horas como hora general]</strong>: Si este proyecto se restaura más adelante, la hora permanecerá en el parte de horas.</li> 
        <li><strong>[!UICONTROL Eliminar cualquier hora registrada]</strong>: Si posteriormente se restaura este proyecto, se restaurará el tiempo ya registrado en el proyecto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Al eliminar tareas o problemas]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Mover cualquier tiempo registrado al proyecto en el que reside la tarea o el problema]</strong>: Si esta tarea o problema se restaura más tarde, el tiempo permanece en el proyecto.<br></li> 
        <li> <p><strong>[!UICONTROL Eliminar cualquier hora registrada]</strong>: Si esta tarea o problema se restaura más tarde, el tiempo registrado se restaura a la tarea o problema.</p> <p>Para obtener información más detallada sobre estas opciones, consulte <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configurar efecto] en horas en que se elimina y se restaura un objeto</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Guardar]**.

## Desbloquear preferencias de horas y horas para grupos

Los grupos de su organización pueden necesitar un parte de horas o una preferencia de hora configurada de forma diferente para sus flujos de trabajo únicos. Puede desbloquear la preferencia de todos los grupos en toda la organización para que puedan configurarla por su cuenta.

Cuando una preferencia está desbloqueada y un administrador de grupo la modifica, afecta a los propietarios de hojas de horas si el grupo es su grupo principal.

Para obtener información sobre cómo un administrador de grupo configura las preferencias de horas y horas de un grupo, consulte [Configuración de las preferencias de horas y horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Después de un [!DNL Workfront] administrador desbloquea una preferencia a nivel de sistema, cualquier administrador de grupo puede configurarla y luego bloquearla para asegurarse de que todos los miembros de su grupo y los subgrupos siguientes usen la misma configuración. Esto es paralelo a la capacidad de que una [!DNL Workfront] El administrador debe configurar y bloquear una preferencia para todos los miembros del sistema. Para obtener más información, consulte [Bloquear o desbloquear un grupo de preferencias de horas y horas](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Para desbloquear una preferencia de proyecto para que los grupos puedan configurarla:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Hojas de hora y horas]** y haga clic en **[!UICONTROL Preferencias]**.

1. Realice una de las siguientes acciones:

   * Si desea que los administradores del grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos utilicen la configuración para una preferencia, asegúrese de que esté bloqueada (este es el valor predeterminado).

      >[!IMPORTANT]
      >
      >Le recomendamos que se comunique con los administradores y usuarios en grupos de todo el sistema para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando lo bloquea, la configuración para él la heredan todos los grupos del sistema. Y si la preferencia se ha desbloqueado durante cualquier periodo de tiempo, la configuración sustituye a las que pueden haber realizado los administradores del grupo.

1. Haga clic en **[!UICONTROL Guardar]**.
