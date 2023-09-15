---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Delegar tareas y problemas
description: Puede delegar temporalmente el trabajo al que esté asignado mientras esté fuera de la oficina. Este artículo describe cómo delegar asignaciones de tareas y problemas.
author: Alina
feature: Work Management
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1485'
ht-degree: 1%

---

# Administrar delegación de tareas y problemas

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Puede delegar temporalmente el trabajo al que esté asignado mientras esté fuera de la oficina.

Puede delegar tareas y asignaciones de problemas o puede delegar aprobaciones. Este artículo describe cómo delegar asignaciones de tareas y problemas.

Para obtener información general sobre la delegación de trabajo, consulte [Resumen del trabajo delegado](../../manage-work/delegate-work/delegate-work-overview.md).

## Requisitos de acceso

>[!IMPORTANT]
>
>* Los usuarios que seleccione como delegados reciben los mismos permisos que sus permisos en las tareas y problemas que delegue en ellos.
>* Los permisos deben funcionar dentro de sus niveles de acceso y, a veces, sus niveles de acceso pueden ser inferiores a los suyos.
>
>   
>   Por ejemplo, si un usuario solo tiene acceso de Vista a las tareas de su nivel de acceso y tiene permisos de Administración en las tareas que delega en él, recibirá permisos de Administración en las tareas que delega en él. Sin embargo, no podrán realizar las mismas acciones que usted en las tareas delegadas. Deben solicitar al administrador del sistema acceso de edición de tareas para poder actualizar las tareas en su ausencia.
>
>   
>   Para obtener información sobre cómo un usuario puede modificar su nivel de acceso, consulte [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* Para los elementos que se asignan después de que la delegación ya haya comenzado, puede tardar hasta una hora después de que se haya asignado el elemento [!DNL Workfront] para compartir los elementos recién asignados con el delegado.


Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>Revisar o superior</p>

>[!NOTE]
>
>Aunque se le puede asignar un trabajo cuando tiene una licencia de solicitud, no puede delegar su trabajo a otros. [!DNL Workfront] no recomienda asignar trabajo a los usuarios de revisión o solicitud.

</tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Tareas y Problemas Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver los permisos o niveles superiores de las tareas o problemas que tiene asignados</p> 
    <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Requisitos previos

Antes de poder realizar las actividades descritas en este artículo, debe asegurarse de lo siguiente:

* Su [!DNL Workfront] o el administrador del grupo habilitó el [!UICONTROL Permitir que los usuarios eliminen tareas y problemas con las horas registradas] configuración en la [!UICONTROL Configurar] área de su [!DNL Workfront] ejemplo.

  Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de todo el sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Delegar tareas y problemas a otro usuario

Antes de delegar el trabajo a otros, le recomendamos que se ponga en contacto con ellos y les informe de que serán designados como delegados en sus elementos de trabajo. Pida su aprobación verbal antes de delegar el trabajo para asegurarse de que tengan el tiempo necesario para completar el trabajo mientras está fuera de la oficina.

Para obtener información general sobre la delegación de tareas y problemas, consulte [Información general sobre tareas y problemas delegados](delegate-work.md).

Para delegar sus tareas y problemas a otros:

1. Vaya a la [!UICONTROL **Inicio**] y haga clic en [!UICONTROL **Delegar**] en la parte superior del [!UICONTROL **Lista de trabajos**].

   ![](assets/delegate-button-in-home.png)

1. En el [!UICONTROL **Delegar tareas y problemas**] pestaña, actualice lo siguiente:

   * [!UICONTROL **Delegar sus tareas y problemas a**]: Empiece a escribir el nombre del usuario al que desea delegar sus tareas y problemas y, a continuación, selecciónelo cuando se muestre en la lista. Solo puede seleccionar un usuario.\

     El usuario que seleccione como delegado recibe los mismos permisos que sus permisos en las tareas y problemas que delegue en ellos. Para obtener más información, consulte [Delegar tarea y descripción general del problema](delegate-work-overview.md).

   * [!UICONTROL **Fecha de inicio**]: seleccione en el calendario la fecha en la que debe comenzar la delegación de los elementos de trabajo.

     >[!TIP]
     >
     >La fecha de inicio no puede ser una fecha pasada.

   * [!UICONTROL **Sin fecha de finalización**]: seleccione esta opción si no desea especificar la fecha de finalización de la delegación.

   * [!UICONTROL **Fecha de finalización**]: seleccione en el calendario una fecha en la que la delegación deba detenerse.

     >[!TIP]
     >
     >Al no seleccionar una Fecha de finalización, la delegación solo se puede delegar para el día actual.

     ![](assets/delegate-box-expanded-in-home.png)

1. Haga clic en [!UICONTROL **Guardar**].

   Suceden las siguientes cosas:

   * El trabajo se ha delegado al usuario especificado. Se delegarán todas las tareas o problemas incompletos que tengan fechas dentro del lapso de tiempo seleccionado (incluidos los recién asignados, después de habilitar la delegación).

   >[!TIP]
   >
   >   Los elementos de trabajo completados que tienen fechas dentro del lapso de tiempo de la delegación no se delegan.


   * Recibirá un mensaje en la esquina superior derecha de la pantalla para confirmar que ha habilitado la delegación de su trabajo a otro usuario. El nombre del usuario delegado se muestra en el mensaje de confirmación.

   * Se muestra una indicación de que las tareas y los problemas se han delegado a otros usuarios en la mayoría de las áreas donde puede ver asignaciones en [!DNL Workfront]. Para obtener más información sobre las áreas que no incluyen los nombres de los delegados, consulte [Delegar tarea y descripción general del problema](delegate-work-overview.md).

   * El [!UICONTROL **Delegar**] botón en el [!UICONTROL Inicio] cambios de área en [!UICONTROL **Editar delegación**] para indicar que hay una delegación en el lugar.
   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Si las notificaciones de eventos y las notificaciones personales están habilitadas, también recibirá una confirmación de su delegación por correo electrónico.

   * El usuario que ha seleccionado como delegado recibe un correo electrónico sobre la delegación si las notificaciones de eventos están habilitadas.

     Para obtener información sobre cómo activar las notificaciones personales por correo electrónico, consulte [Modificar sus propias notificaciones por correo electrónico](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).




## Editar o detener delegación

Puede permitir que una delegación caduque si ha seleccionado una fecha de finalización o puede detenerla manualmente. También puede modificar el lapso de tiempo de la delegación si las fechas de la delegación han cambiado.

1. Vaya a la [!UICONTROL Inicio] y haga clic en [!UICONTROL Editar delegación] en la esquina superior derecha de la Lista de trabajos.
1. En el [!UICONTROL Delegar tareas y problemas] pestaña, realice una de las siguientes acciones:
   * Modifique la [!UICONTROL **Fecha de inicio**] o el [!UICONTROL **Fecha de finalización**]
   * Clic [!UICONTROL **Detener delegación**]

   >[!TIP]
   >
   >    Solo puede editar la fecha de finalización de una delegación si esta ya ha comenzado.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Condicional) haga clic en [!UICONTROL **Guardar**] para guardar las nuevas fechas de delegación

   O

   Clic [!UICONTROL **Detener delegación**] en el cuadro de confirmación para confirmar la detención de la delegación.

   La delegación ha actualizado las fechas o se ha detenido y los usuarios delegados se han eliminado de sus tareas y problemas. Sus permisos para las tareas y problemas siguen vigentes.


## Localizar trabajo delegado e información de delegado

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

Cuando se delegan tareas y problemas, existen varias áreas en [!DNL Workfront] donde puede ver el trabajo delegado o quiénes son los delegados.

* [Busque delegados en la casilla Asignaciones](#locate-delegates-in-the-assignments-box)
* [Localizar trabajo delegado en [!UICONTROL Inicio]](#locate-delegated-work-in-home)


### Busque delegados en la [!UICONTROL Asignaciones] caja

Cuando el administrador del sistema o del grupo habilita la delegación de trabajo en el sistema, la variable [!UICONTROL Asignaciones] El cuadro muestra las siguientes fichas en todas las partes a las que se puede acceder:

* [!UICONTROL **Asignaciones**]: los usuarios asignados a la tarea o al problema se muestran aquí.
* [!UICONTROL **Delegaciones**]: aquí se muestran los usuarios designados como delegados por los usuarios asignados a la tarea o al problema.

Puede acceder a las [!UICONTROL Asignaciones] en las áreas siguientes:

* El encabezado de la tarea o del problema

  ![](assets/assignments-and-delegates-panel-in-task-header.png)

  El [!UICONTROL Asignaciones] del encabezado de tarea o problema cambia a [!UICONTROL Asignaciones y delegaciones].

* El [!UICONTROL Distribuidor de cargas de trabajo] al asignar manualmente tareas o problemas

  ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> No puede ver delegados en [!UICONTROL Asignaciones] de una tarea o problema Cuadro de edición.

Si se delega una tarea o un problema y la variable [!UICONTROL Delegaciones] subpestaña está vacía, puede darse una de las siguientes situaciones:

* No se le ha asignado la tarea o el problema.
* Las fechas de la tarea o del problema están fuera del lapso de tiempo de delegación.

>[!TIP]
>
>Las horas planificadas o reales para tareas y problemas delegados no se tienen en cuenta en las herramientas de administración de recursos, como la variable [!UICONTROL Distribuidor de cargas de trabajo] o el [!DNL Resource Planner] para los usuarios delegados. Las horas permanecen asociadas únicamente al usuario asignado.

### Localizar trabajo delegado en [!UICONTROL Inicio]

1. Vaya a la [!UICONTROL **Inicio**] , luego haga clic en el menú desplegable filter y seleccione una o más de las siguientes opciones:
   * [!UICONTROL **Delegado**]: para ver las tareas y los problemas delegados por usted o por usted.
   * [!UICONTROL **Se me ha delegado**]: para ver las tareas y los problemas delegados por otro usuario.
   * [!UICONTROL **Delegado por mí**]: para ver las tareas y los problemas delegados por usted a otros usuarios.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Haga clic en [!UICONTROL clasificación] menú desplegable para ordenar la lista según los siguientes criterios:
   * [!UICONTROL Finalización planificada]. Esta es la opción de ordenación predeterminada.
   * [!UICONTROL Inicio planificado]
   * [!UICONTROL Fecha de confirmación]
   * [!UICONTROL Proyecto]
   * [!UICONTROL Mi prioridad]
1. Expanda las agrupaciones en la [!UICONTROL **Lista de trabajos**] para ver los elementos de trabajo delegados. Existen los siguientes escenarios:
   * Para los elementos que ha delegado en otros, el nombre del delegado se muestra en el [!UICONTROL **Lista de trabajos**] así como el [!UICONTROL **Asignaciones y delegaciones**] a la derecha.

   * Para los elementos delegados en usted, el nombre del usuario asignado aparece en la [!UICONTROL **Lista de trabajos**] así como el **[!UICONTROL Asignaciones y delegaciones]** a la derecha.

   >[!TIP]
   >
   >    Si la delegación está configurada para comenzar en una fecha posterior a la fecha actual, la fecha de inicio de la delegación también se muestra en la [!UICONTROL Lista de trabajos]. Los elementos delegados se muestran en la agrupación seleccionada para el [!UICONTROL Lista de trabajos], según el tipo de agrupación. Por ejemplo, si agrupa por [!UICONTROL Fecha planificada de finalización], los elementos delegados se muestran en la agrupación que coincide con las fechas de finalización planificadas.
