---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Configurar preferencias de horas y hojas de horas
description: Como un [!DNL Adobe Workfront] administrador, puede especificar preferencias para plantillas de horas y horas en [!DNL Workfront] para definir con qué elementos pueden rellenarse previamente las plantillas de horas y con qué elementos pueden registrar los usuarios el tiempo.
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 62c600a13f61f7f5e889a92b446252e5ca0777f9
workflow-type: tm+mt
source-wordcount: '1352'
ht-degree: 1%

---

# Configurar preferencias de horas y hojas de horas

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como un [!DNL Adobe Workfront] administrador, puede especificar preferencias para plantillas de horas y horas en [!DNL Workfront] para definir con qué elementos pueden rellenarse previamente las plantillas de horas y con qué elementos pueden registrar los usuarios el tiempo.

>[!NOTE]
>
>Los elementos para los que ha registrado tiempo durante el marco de tiempo de la plantilla de horas se muestran en la plantilla de horas de forma predeterminada, aunque es posible que no cumplan las condiciones descritas en este artículo para rellenar previamente la plantilla de horas.
>
>Para obtener información sobre el registro del tiempo, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).


Cualquier cambio que realice en las hojas de horas afectará a todas las que se creen en el futuro.

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
   <td> <p>Debe ser un [!DNL Workfront] administrador.</p> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Establecer preferencias de horas y hojas de horas

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Hoja de horas y horas]** > **[!UICONTROL Preferencias]**.

1. En la página que se muestra, en la variable **[!UICONTROL Preferencias generales]** , configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Registrar tiempo para fechas futuras]</td> 
      <td> <p>Permite a los usuarios registrar tiempo para fechas futuras en todo el sistema en:</p> 
       <ul> 
        <li>Cualquier proyecto, tarea o problema en el que tenga acceso para registrar el tiempo</li> 
        <li>Sus hojas de horas como Hora general</li> 
       </ul> <p>Esto resulta útil cuando los usuarios planean estar fuera de la oficina y desean registrar esa hora de antemano.</p> <p><b>NOTA</b>:</p> 
       <p>No puede impedir que los usuarios registren la hora en tareas o problemas que se hayan cerrado o cancelado. Solo puede evitar que los usuarios registren el tiempo en proyectos completos o inactivos. Le recomendamos que utilice filtros en listas de tareas y problemas para excluir de la visibilidad a los usuarios los que se hayan completado o cancelado.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Asignar roles a entradas de hora manualmente]</td> 
      <td> <p>Permite que los usuarios seleccionen manualmente cualquier rol asignado en su perfil de usuario o asignado al objeto.</p> <p><b>IMPORTANTE</b>:  
        <ul> 
         <li>Si deshabilita esta configuración después de asignar los roles a las entradas de horas, los usuarios deben ajustar las horas registradas en los distintos roles de la ficha [!UICONTROL Horas] del proyecto, tarea o problema.</li> 
         <li>Si el usuario no tiene un rol asignado en su perfil y hay una tarea asignada como [!UICONTROL Propietario de tarea] en el cuadro de diálogo [!UICONTROL Asignaciones avanzadas], ese rol aparece cuando el usuario registra tiempo en la tarea.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir la edición de hojas de horas a propietarios y administradores]</td> 
      <td> <p>Restringir la edición a propietarios de hojas de horas y [!DNL Workfront] administradores. Si se deshabilita esta opción, las plantillas de horas también se pueden editar:</p> 
       <ul> 
        <li> <p>Usuarios con acceso administrativo a hojas de horas y horas en su nivel de acceso</p> </li> 
        <li> <p>Aprobadores de hojas de horas si "Puede editar horas" está habilitado en la hoja de horas</p> </li> 
        <li> <p>El administrador del propietario de la plantilla de horas</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Restringir la edición de horas a propietarios y administradores]</td> 
      <td>Restringir la edición al usuario que introduce las horas y [!DNL Workfront] administradores. Esta opción se aplica a la ficha [!UICONTROL Horas] de un proyecto o de un informe de horas.</td> 
     </tr> 
    </tbody> 
   </table>

1. En el **[!UICONTROL Donde los usuarios pueden registrar el tiempo]** , configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Registrar tiempo directamente en proyectos]</td>
        <td>Permite a los usuarios registrar tiempo en el proyecto (tanto en la ficha [!UICONTROL Actualizaciones] como en la hoja de horas). Si los usuarios no registran el tiempo en el nivel de proyecto, estas opciones deben permanecer desmarcadas.</td>
    </tr>
    <tr>
        <td>Registrar tiempo en proyectos completos</td>
        <td>Permite a los usuarios registrar el tiempo de un proyecto que se ha marcado como completado. Si esta opción está deshabilitada, los usuarios no podrán registrar el tiempo de trabajo que hayan completado en los proyectos en el estado [!UICONTROL Completado].</td>
    </tr>
    <tr>
        <td>Registrar tiempo en proyectos inactivos</td>
        <td>Cuando esta opción está habilitada, los usuarios pueden registrar horas en los proyectos con un estado [!UICONTROL Inactivo].</td>
    </tr>
   </table>

1. En el **[!UICONTROL Rellenar de forma previa las hojas de horas]** , configure cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Trabajo que se encuentra dentro] &lt;number of="" weeks=""&gt; [!UICONTROL del intervalo de trabajo de la hoja de horas]</td> 
      <td> <p>Define el número de semanas antes y después del intervalo de fechas de la hoja de horas que contiene las fechas de las tareas y problemas asignados al usuario. La configuración predeterminada es 1 semana y puede ampliar este intervalo a 4 semanas. Esto significa que la hoja de horas se rellena previamente con tareas y problemas que tienen fechas entre cuatro semanas antes del intervalo de fechas de la hoja de horas y hasta cuatro semanas después del intervalo de fechas de la hoja de horas, si selecciona 4 semanas para el intervalo de fechas. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tareas y problemas que se han completado]</td> 
      <td>Si se suelen asignar varios recursos a una sola tarea, se recomienda esta configuración. Esto significa que cuando un recurso registra la hora con la tarea y la marca como completada, los demás recursos asignados a la tarea pueden encontrar la tarea o el problema en su hoja de horas para registrar sus horas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tareas y problemas con fechas planificadas que se encuentren en el rango de fechas de la hoja de horas]</td> 
      <td> <p>Una vez seleccionada, la hoja de horas incluye tareas y problemas con una fecha planificada de inicio o una fecha de finalización que se encuentran dentro del intervalo de fechas de la hoja de horas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Tareas que tienen Fechas proyectadas en el intervalo de fechas de la hoja de horas]</td> 
      <td> <p>Cuando se selecciona, la hoja de horas incluye tareas que tienen una Fecha proyectada de inicio o Fecha de finalización que se encuentra dentro del marco de tiempo del proyecto, incluso si la fecha planificada del problema o la tarea está fuera del intervalo de fechas de la hoja de horas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **[!UICONTROL Proyectos, tareas y problemas eliminados]** , especifique lo siguiente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Al eliminar proyectos]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Mantener el tiempo registrado ya añadido a las hojas de horas como tiempo general]</strong>: Si este proyecto se restaura más adelante, el tiempo permanece en la plantilla de horas.</li> 
        <li><strong>[!UICONTROL Eliminar cualquier hora registrada]</strong>: si se restaura este proyecto posteriormente, el tiempo ya registrado se restaura en el proyecto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Al eliminar tareas o problemas]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Mover el tiempo registrado al proyecto donde reside la tarea o el problema]</strong>: si esta tarea o este problema se restaura posteriormente, el tiempo permanece en el proyecto.<br></li> 
        <li> <p><strong>[!UICONTROL Eliminar cualquier hora registrada]</strong>: si esta tarea o este problema se restaura posteriormente, el tiempo registrado se restaura en la tarea o el problema.</p> <p>Para obtener información más detallada sobre estas opciones, consulte <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Configurar efecto] en horas en que se elimina y restaura un objeto</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Guardar]**.

## Desbloquear hoja de horas y preferencias de horas para grupos

Es posible que los grupos de su organización necesiten una plantilla de horas o una preferencia de hora configuradas de forma diferente para sus flujos de trabajo únicos. Puede desbloquear la preferencia de todos los grupos de la organización para que puedan configurarla ellos mismos.

Cuando una preferencia está desbloqueada y un administrador de grupo la modifica, afecta a los propietarios de plantillas de horas si el grupo es su grupo de inicio.

Para obtener información sobre cómo un administrador de grupo configura las preferencias de horas y hojas de horas de un grupo, consulte [Configurar las preferencias de horas y hojas de horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Después de un [!DNL Workfront] Un administrador desbloquea una preferencia en el sistema. Cualquier administrador de grupo puede configurarla y, a continuación, bloquearla para garantizar que todos los miembros de su grupo y de los subgrupos siguientes utilicen la misma configuración. Esto es paralelo a la capacidad de que un [!DNL Workfront] El administrador de debe configurar y bloquear una preferencia para todos los usuarios del sistema. Para obtener más información, consulte [Bloquear o desbloquear una plantilla de horas de grupo y sus preferencias horarias](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

Para desbloquear una preferencia de proyecto de modo que los grupos puedan configurarla:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **[!UICONTROL Hojas de horas y horas]**, luego haga clic en **[!UICONTROL Preferencias]**.

1. Realice una de las siguientes acciones:

   * Si desea que los administradores de grupo puedan configurar una preferencia para sus grupos, desbloquéela ![](assets/unlock-toggle-button.png).
   * Si desea que todos los grupos utilicen su configuración para una preferencia, asegúrese de que esté bloqueada (este es el valor predeterminado).

     >[!IMPORTANT]
     >
     >Le recomendamos que se comunique con los administradores y usuarios de los grupos de todo el sistema para asegurarse de que todas las necesidades se tienen en cuenta de la forma en que configura una preferencia bloqueada. Cuando lo bloquea, la configuración para él la heredan todos los grupos del sistema. Y si la preferencia se ha desbloqueado durante cualquier período de tiempo, la configuración reemplaza las que los administradores del grupo puedan haber realizado.

1. Haga clic en **[!UICONTROL Guardar]**.
