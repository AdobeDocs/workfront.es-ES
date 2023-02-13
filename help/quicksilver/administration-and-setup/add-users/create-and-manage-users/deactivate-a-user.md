---
title: Desactivar o reactivar un usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador de Workfront, puede desactivar o reactivar un usuario.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Desactivar o reactivar un usuario

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre cómo desactivar un usuario en Adobe Admin Console, consulte la sección &quot;Eliminar usuarios&quot; en el artículo [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) o póngase en contacto con su administrador de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Es posible que los usuarios abandonen la organización y que tenga que eliminarlos de Adobe Workfront. No deben permanecer activos en el sistema porque esto crearía confusión para otros usuarios al agregarlos a actualizaciones o al asignarles trabajo. Cuando desactiva un usuario, otros usuarios ya no ven su nombre cuando buscan personas en el sistema.

Los administradores pueden ver usuarios inactivos en el área de configuración.

Puede reactivar un usuario en cualquier momento.

>[!IMPORTANT]
>
>Se recomienda desactivar los usuarios que hayan abandonado la organización en lugar de eliminarlos. Si se elimina un usuario, se perderá todo el historial de Workfront asociado a él. Esto incluye sus asignaciones de trabajo, su asociación con notas, horas, documentos y todos los demás objetos que una vez han creado.
>
>Al desactivar un usuario en Workfront, se eliminan las licencias del usuario para las pruebas digitales y Workfront. Además, ya no se puede asignar trabajo al usuario. Cuando se desactiva un usuario, la licencia de Workfront y la licencia de prueba de ese usuario quedan disponibles para que la utilice otro usuario; el resto de la información del perfil del usuario desactivado permanece tal cual.
>
>Para obtener más información sobre el impacto de la eliminación y el de la desactivación de usuarios, consulte [Eliminar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Plan </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener una de las siguientes opciones:</p> 
    <ul> 
     <li> <p>Nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p><b>Usuarios</b> en el nivel de acceso configurado para <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos <b>Administrador de usuarios</b> opciones activadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si es Usuario <b>Administración (usuarios del grupo)</b> está activada, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> <p>Para obtener más información sobre la variable <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Desactivar un usuario

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Seleccione un usuario, haga clic en el icono Más ![](assets/more-icon.png)y haga clic en **Desactivar**.

1. Haga clic en **Desactivar** en el cuadro que aparece.

## Programar usuarios para su desactivación

Como administrador, es posible que desee marcar a los usuarios para su desactivación antes de que abandonen su organización. Por ejemplo, si está trabajando con un usuario que está enlazado contractualmente, estará en su sistema durante un período de tiempo limitado y sabe su fecha de finalización. Puede programarlos para desactivarlos en esa fecha.

Los administradores de Workfront y los usuarios de licencias de Plan pueden ver la fecha de desactivación en su perfil de usuario.

Para programar la desactivación de un usuario:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Seleccione el nombre del usuario.

   O

   (Opcional) Seleccione varios usuarios para programarlos para su desactivación de forma masiva.

1. Haga clic en el icono Editar ![](assets/edit-icon.png).
1. En el cuadro Editar usuario que aparece, haga clic en **Planificación de recursos** para ir a esa zona.
1. Active la variable **Desactivación de programación** .

1. En el calendario que se muestra, especifique la fecha y la hora del **Fecha de desactivación programada**.

   >[!NOTE]
   >
   >* En el cuadro de tiempo, solo puede seleccionar incrementos de hora completos, no minutos.
   >* Si selecciona una hora para el día actual que ha pasado, Workfront programará la desactivación para el día siguiente a las 12:00. La hora seleccionada coincide con la zona horaria del equipo del usuario que está programando la desactivación.


1. Haga clic en **Guardar cambios**.

   El usuario se desactiva el día seleccionado, a veces después de la hora seleccionada. Si ha seleccionado varios usuarios para desactivarlos de forma masiva, todos los usuarios seleccionados se desactivarán el día seleccionado, a veces después de la hora seleccionada.

Le recomendamos que cree un informe para los usuarios que ha programado para su desactivación, para mantenerse informados sobre los usuarios que se van a desactivar. No hay confirmación de que la desactivación se haya producido una vez que los usuarios se desactivan.

## Reactivar un usuario

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Seleccione un usuario, haga clic en el icono Más ![](assets/more-icon.png)y haga clic en **Activar**.

1. Asignar un nuevo **Nivel de acceso** en el menú desplegable.

### Impacto de la prueba al reactivar un usuario

Los usuarios desactivados pierden la función de prueba predeterminada asignada y su licencia de prueba (si está en un plan heredado de Workfront Premium). Si decide reactivar el usuario, debe:

* Vuelva a asignar la licencia (si está en un plan heredado de Workfront Premium). Para obtener más información sobre los planes de pruebas de Workfront, consulte [Acceso a la funcionalidad de pruebas en Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Compruebe que tienen la función de prueba correcta. A los usuarios de prueba reactivados se les asigna la función de prueba predeterminada que se especifique para los nuevos usuarios. Consulte [Configuración de las funciones de prueba predeterminadas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) para obtener más información.

## Acerca de la desactivación de administradores de Workfront y usuarios de licencias de Plan

Antes de desactivar un administrador de Workfront o un usuario con una licencia de Plan, es importante comprobar los objetos y actividades de Workfront que involucren a esa persona y luego asociarlos a otro administrador de Workfront o a otro usuario de licencia de Plan según sea necesario.

Estos objetos y actividades pueden incluir lo siguiente:

* Tareas o problemas asignados al usuario
* Proyectos propiedad del usuario
* Informes configurados para ejecutarse con los derechos de acceso del usuario
* Plantillas que son propiedad del usuario
* Proyectos y plantillas en los que se configuró el usuario como gestor de recursos
* Solicitar reglas de enrutamiento de cola en las que el administrador de Workfront o el usuario de licencia de Plan sea el Usuario asignado predeterminado
* Procesos de aprobación que tienen una fase que incluye al usuario (especialmente si son el único aprobador del escenario)
* Hojas de tiempo que enumeran al usuario como aprobador
* Perfiles de hoja de horas que enumeran al usuario como aprobador
* Revisión de los flujos de trabajo automatizados que incluyen al usuario

## Impacto en la planificación de recursos al programar la desactivación de un usuario

Cuando programa un usuario para su desactivación, ya no aparece en el Planificador de recursos como disponible para el horario de presupuestación. Si siguen formando parte de los grupos de recursos, aparecerán en el Planificador de recursos, pero su disponibilidad se establecerá en cero horas a partir de la fecha de su desactivación programada.

El planificador de recursos tiene en cuenta todas las funciones de trabajo de los usuarios y las fechas de finalización planificadas de las tareas y calcula los recursos en consecuencia.

Para obtener más información acerca del planificador de recursos, consulte [Información general del planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
