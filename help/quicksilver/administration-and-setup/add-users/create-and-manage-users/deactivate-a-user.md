---
title: Desactivar o reactivar un usuario
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Los administradores de Workfront pueden desactivar o reactivar un usuario.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: 1a81c1becfc0866b92dbd1358af23671e5302266
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 9%

---

# Desactivar o reactivar un usuario {#deactivate-or-reactivate-a-user}

>[!CONTEXTUALHELP]
>id="wf_users_deactivate_user"
>title="Desactivar un usuario"
>abstract="Al desactivar un usuario, se elimina de Workfront y Frame.io. Los usuarios desactivados se pueden reactivar más adelante."

<!--Audited 5/2025-->

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on deactivating a user in the Adobe Admin Console, see the section "Remove users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Si un usuario abandona la organización, se recomienda desactivarlo en el sistema para evitar crear confusión a otros usuarios al añadirlos a las actualizaciones o asignarles trabajo. Cuando desactiva un usuario, los demás usuarios ya no ven su nombre cuando buscan personas en el sistema.

Los administradores pueden ver los usuarios inactivos en el área de Configuración.

Puede reactivar un usuario en cualquier momento.

>[!IMPORTANT]
>
>* Se recomienda desactivar usuarios que hayan abandonado la organización en lugar de eliminarlos. Si se elimina un usuario, se perderá todo el historial en Workfront asociado con ese usuario. Esto incluye sus asignaciones de trabajo, su asociación con notas, horas, documentos y todos los demás objetos que hayan creado una vez.
>
>* Al desactivar un usuario en Workfront, se eliminan sus licencias tanto de Workfront como de revisión digital. Además, ya no se puede asignar trabajo al usuario. Cuando se desactiva un usuario, su licencia de Workfront y su licencia de revisión quedan disponibles para que las utilice otro usuario. El resto de la información del perfil del usuario desactivado permanece sin cambios.
>
>* Al desactivar un usuario en Workfront, no se elimina del Perfil de productos de Workfront en Adobe Admin Console. Para obtener más información, consulte [Eliminar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p><p>O</p><p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. </li> 
     <li> <p>Usuarios configurados en su nivel de acceso configurado para Editar acceso, con Crear y al menos una de las dos opciones de Administración de usuarios habilitada en Ajustar la configuración <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si Administración de usuarios (usuarios del grupo) está habilitada, debe ser administrador de un grupo al que pertenezca el usuario.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de desactivar un administrador de Workfront o un usuario con licencia estándar o de planificación, debe asociar sus objetos y actividades a otro usuario.

Para obtener más información, consulte [Acerca de la desactivación de administradores de Workfront y usuarios con licencias Standard o Plan](#about-deactivating-workfront-administrators-and-plan-license-users) en este artículo.

## Desactivar un usuario

Tenga en cuenta lo siguiente al desactivar un usuario:

* El usuario no podrá acceder al sistema.
<!--* The user will be removed from Frame.io review links, assets, projects, and accounts.
   * Reactivating the user does not automatically add them back to the Frame.io items. You must reassign the user manually to Workfront projects, tasks, and assets that require Frame.io collaboration.-->
* Se conservarán todos los datos asociados con el usuario.
* Puede asignar una licencia de usuario desactivado a otro usuario.

Para desactivar un usuario:

{{step-1-to-users}}

1. Seleccione un usuario en la lista de usuarios.
1. Haga clic en el icono **Más** ![Más iconos](assets/more-icon.png) y, a continuación, haga clic en **Desactivar**.

1. En el cuadro de diálogo **Desactivar usuario**, haga clic en **Desactivar**.

## Programar usuarios para su desactivación

Como administrador, es posible que desee marcar a los usuarios para su desactivación antes de que abandonen realmente la organización. Por ejemplo, si está trabajando con un usuario que está vinculado por contrato, estará en su sistema durante un período de tiempo limitado y sabrá su fecha de finalización. Puede programarlos para que se desactiven en esa fecha.

Los administradores de Workfront y los usuarios de licencias de planificación pueden ver la fecha de desactivación en su perfil de usuario.

Para programar la desactivación de un usuario:

{{step-1-to-users}}

1. Seleccione el usuario en la lista usuarios.

   O

   (Opcional) Seleccione varios usuarios para programarlos y desactivarlos de forma masiva.

1. Haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).
1. En el panel izquierdo del cuadro **Editar usuario**, haga clic en **Planificación de recursos**.
1. Haga clic en **Establecer fecha de desactivación**.

1. Seleccione la fecha y la hora de la **fecha de desactivación**.

   >[!NOTE]
   >
   >* En el cuadro Tiempo, solo puede seleccionar incrementos de hora completas, no minutos.
   >* Si selecciona una hora para el día actual que ha pasado, Workfront programará la desactivación para el día siguiente a las 12:00 a. m.
   >* La hora seleccionada coincide con la zona horaria del equipo del usuario que está programando la desactivación.

1. Haga clic en **Guardar**.

El usuario se desactiva en el día seleccionado en algún momento después de la hora seleccionada. Si ha seleccionado varios usuarios para desactivarlos de forma masiva, todos los usuarios seleccionados se desactivarán el día seleccionado en algún momento después de la hora seleccionada.

Le recomendamos que genere un informe para los usuarios que ha programado para su desactivación a fin de mantenerse informados sobre los usuarios que se aproximan a la desactivación. No hay confirmación de que la desactivación se haya producido después de desactivar los usuarios.

## Reactivar un usuario

{{step-1-to-users}}

1. Seleccione un usuario, haga clic en el icono **Más** ![Más iconos](assets/more-icon.png) y, a continuación, haga clic en **Activar**.

1. En el cuadro de diálogo **Reactivar usuario**, seleccione un nuevo **nivel de acceso** en el menú desplegable y luego haga clic en **Reactivar**.
<!--
### Asset review and approval impact when you reactivate a user

Deactivated users lose access to their assigned Frame.io accounts as well as assigned projects, assets, and review links. If you choose to reactivate the user, you must manually reassign them to projects, tasks, and assets that require Frame.io collaboration. -->

### Impacto de la corrección al reactivar un usuario

Los usuarios desactivados pierden la función de corrección predeterminada que se les ha asignado y la licencia de revisión (si cuenta con un plan heredado de Workfront Premium). Si decide reactivar el usuario, deberá:

* Reasigne la licencia (si cuenta con un plan heredado de Workfront Premium). Para obtener más información sobre los planes de revisión de Workfront, consulte [Acceso a la funcionalidad de revisión en Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Compruebe que tienen la función de prueba correcta. A los usuarios de prueba reactivados se les asigna la función que se especifique como predeterminada para los nuevos usuarios. Consulte [Configurar funciones de revisión predeterminadas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) para obtener más información.

## Acerca de la desactivación de administradores de Workfront y usuarios con licencias Standard o Plan

Antes de desactivar un administrador de Workfront o un usuario con una licencia de planificación, es importante comprobar si hay objetos y actividades de Workfront que impliquen a esa persona y luego asociarlos a otro administrador de Workfront o usuario con licencia de planificación según sea necesario.

Estos objetos y actividades pueden incluir lo siguiente:

* Tareas o problemas asignados al usuario.
* Proyectos propiedad del usuario.
* Informes configurados para ejecutarse con los derechos de acceso del usuario.
* Plantillas propiedad del usuario.
* Proyectos y plantillas en los que el usuario se ha establecido como administrador de recursos.
* Reglas de enrutamiento de cola de solicitudes el administrador de Workfront o el usuario con licencia de planificación es el usuario asignado predeterminado.
* Procesos de aprobación que tienen una fase que incluye al usuario (especialmente si es el único aprobador de la fase).
* Plantillas de horas que enumeran al usuario como aprobador.
* Perfiles de hojas de horas que enumeran al usuario como aprobador.
* Revisión de flujos de trabajo automatizados que incluyen al usuario.

## Influencia de la planificación de recursos al programar la desactivación de un usuario

Cuando se programa la desactivación de un usuario, ya no aparece en el Planificador de recursos como disponible para las horas presupuestadas. Si siguen formando parte de los conjuntos de recursos, aparecen en el Planificador de recursos, pero su disponibilidad se establecerá en cero horas a partir de la fecha de su desactivación programada.

El Planificador de recursos tiene en cuenta todos los roles de los usuarios y las Fechas planificadas de finalización de las tareas y calcula los recursos en consecuencia.

Para obtener más información sobre el Planificador de recursos, consulte [Información general del Planificador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

