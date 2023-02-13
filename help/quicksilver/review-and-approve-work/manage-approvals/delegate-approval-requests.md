---
product-area: projects
navigation-topic: approvals
title: Delegar solicitud de aprobación
description: La delegación de solicitudes de aprobación le permite asignar a otro usuario para que apruebe sus solicitudes durante un período de tiempo, por ejemplo, si se encuentra fuera de la oficina durante las vacaciones.
author: Courtney
feature: Work Management
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: d04afc0cc55a71e48c357af2ed4446c22dab1ba4
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 0%

---

# Delegar solicitud de aprobación

Puede delegar temporalmente el trabajo al que está asignado mientras está fuera de la oficina. Puede delegar tareas y asignaciones de problemas o delegar solicitudes de aprobación. Este artículo describe cómo delegar solicitudes de aprobación. Para obtener información sobre la delegación de tareas y asignaciones de problemas, consulte [Administrar delegación de tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

>[!NOTE]
>
>Para garantizar que no se produzcan incoherencias en las fechas programadas para delegar las aprobaciones, recomendamos que la zona horaria de su perfil de usuario coincida con la de la programación. Para obtener más información, consulte los siguientes artículos:
>
>* [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>


## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>plan de Adobe Workfront*</p></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de Workfront.

## Comprender el acceso del usuario para aprobaciones delegadas

Durante el periodo de aprobación designado, el usuario al que delega una solicitud de aprobación tiene las siguientes capacidades:

* Pueden aprobar o rechazar solicitudes de aprobación existentes cuando no se haya tomado ninguna decisión
* Pueden aprobar y rechazar nuevas solicitudes de aprobación que se reciban durante un período de tiempo especificado
* Se concede acceso de vista a los objetos que están pendientes de aprobación

   >[!NOTE]
   >
   > El administrador de Adobe Workfront puede restringir el acceso de los usuarios a ciertos tipos de objetos. Cuando un usuario no tiene acceso a un tipo de objeto y se delega una aprobación de ese tipo al usuario, el usuario no tiene acceso de visualización al objeto. Sin embargo, el usuario aún puede aprobar o rechazar solicitudes de aprobación de la **Página principal** como se describe en [Aprobación del trabajo](../../review-and-approve-work/manage-approvals/approving-work.md).\
   Por ejemplo, el usuario A pertenece al grupo A. El administrador de Workfront ha restringido los derechos de acceso del Grupo A para que los usuarios de este grupo no puedan ver las tareas dentro de Workfront. Si se delega una solicitud de aprobación de tareas al usuario A, el usuario A no puede ver la tarea a la que está asociada la aprobación. Sin embargo, el usuario A puede aprobar o rechazar la solicitud de aprobación desde la página principal.

   Para obtener información sobre cómo el administrador de Workfront puede restringir el acceso a los tipos de objetos dentro de la configuración, consulte  [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

Una vez que la delegación de aprobación se detiene o se cancela, el usuario designado como aprobador:

* Ya no tiene acceso para aprobar el trabajo de elementos que requieren aprobación
* Continúa teniendo acceso de visualización a elementos de trabajo\
   Los usuarios a los que se haya concedido el acceso de visualización a los objetos mediante una delegación de aprobación conservan ese acceso de visualización incluso después de que la delegación de aprobación se detenga o se recupere. Para eliminar el acceso de vista a cualquier objeto al que el usuario tuviera acceso durante el tiempo en que se delegaban las aprobaciones, debe ir al objeto y eliminar los derechos de acceso directamente del objeto.

## Delegar solicitudes de aprobación en el área de inicio

* [Delegación de las aprobaciones en otro usuario](#delegate-your-approvals-to-another-user)
* [Actualizar o detener una delegación de aprobación](#update-or-stop-an-approval-delegation)
* [Ver aprobaciones delegadas](#view-delegated-approvals)

### Delegación de las aprobaciones en otro usuario {#delegate-your-approvals-to-another-user}

Puede delegar los siguientes tipos de aprobaciones, independientemente de cómo se le haya asignado la aprobación (ya se le haya asignado directamente, a un equipo del que sea miembro o a su función de trabajo):

* Aprobaciones del proyecto
* Aprobaciones de tareas
* Aprobaciones de problemas

No se pueden delegar aprobaciones de hojas de horas y documentos. 

Tenga en cuenta lo siguiente al delegar aprobaciones:

* Al delegar aprobaciones, se delegan todas las aprobaciones. No se pueden delegar solicitudes de aprobación individuales.
* Puede delegar aprobaciones a un solo usuario; no se pueden delegar aprobaciones a varios usuarios al mismo tiempo.\
   Todas las aprobaciones de todos los proyectos, tareas y problemas se delegan al usuario designado.
* Un máximo de 5 usuarios pueden delegar aprobaciones al mismo usuario al mismo tiempo. En otras palabras, un solo usuario no puede ser designado como aprobador temporal para más de 5 usuarios al mismo tiempo.
* La actividad relativa a las aprobaciones se muestra en la pestaña Actualizaciones . Debe tener activada la opción Mostrar actualizaciones del sistema. Tanto el usuario que delega la aprobación como el usuario en el que se delegan las aprobaciones reciben una notificación por correo electrónico con respecto a la actividad de aprobación.

Para delegar aprobaciones en otro usuario:

1. Haga clic en el **Página principal** icono ![](assets/home-icon-30x29.png) en la esquina superior izquierda de Adobe Workfront.

   >[!NOTE]
   El administrador de Workfront puede realizar los siguientes cambios en el icono Inicio de su entorno:
   * Sustitúyala por una imagen personalizada para ilustrar su organización. En este caso, el icono tendrá un aspecto diferente al que se muestra en este artículo.
   * Reemplace la página vinculada por una página diferente. En este caso, haga clic en el botón **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de la página, haga clic en **Página principal**.


   O

   Haga clic en el **Menú principal** icono > **su nombre** > **Tiempo desactivado** en el panel izquierdo.

1. (Opcional y condicional) En el área de inicio, haga clic en el **Filtro** menú desplegable y haga clic en **Aprobaciones**.

1. (Condicional) Haga clic en **Delegar mis aprobaciones**

   O

   Si el administrador del sistema o del grupo habilitó la delegación de tareas y problemas, haga clic en **Delegar** y haga clic en **Delegar aprobaciones**.

   ![](assets/delegate-approvals-nwe.png)

1. Especifique la siguiente información en la sección Delegar mis aprobaciones :

   * **Nombre**: Empiece a escribir el nombre del usuario al que desea delegar las aprobaciones y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.
   * **Fecha de inicio**: Seleccione la fecha en la que las aprobaciones empezarán a reenviarse. El reenvío comienza a las 12:00 a.m. de la fecha seleccionada.\
      La fecha de inicio debe ser la fecha actual o una fecha futura.
   * **Fecha final**: Realice una de las siguientes acciones:

      * Seleccione la fecha en la que las aprobaciones dejarán de reenviarse. El reenvío termina a las 23:59 en la fecha seleccionada.
      * Select **Sin fecha de finalización** para configurar Workfront para delegar aprobaciones indefinidamente.

1. Haga clic en **Guardar**.

### Actualizar o detener una delegación de aprobación {#update-or-stop-an-approval-delegation}

1. Haga clic en el **Página principal** icono ![](assets/home-icon-30x29.png) en la esquina superior izquierda de Adobe Workfront.

   >[!NOTE]
   El administrador de Workfront puede realizar los siguientes cambios en el icono Inicio de su entorno:
   * Sustitúyala por una imagen personalizada para ilustrar su organización. En este caso, el icono tendrá un aspecto diferente al que se muestra en este artículo.
   * Reemplace la página vinculada por una página diferente. En este caso, haga clic en el botón **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de la página, haga clic en **Página principal**.


1. Haga clic en el **Filtro** menú desplegable y haga clic en **Aprobaciones**.

1. (Condicional) Haga clic en **Editar delegación**

   O

   Si el administrador del sistema o del grupo habilitó la delegación de tareas y problemas, haga clic en **Editar delegación** y haga clic en **Delegar aprobaciones**.

1. (Condicional) Realice una de las siguientes acciones:

   * Para actualizar la delegación de aprobación existente: Cambie la información mostrada y haga clic en **Guardar**.

   * Para detener la delegación existente: Haga clic en **Detener delegación** y haga clic en **Detener delegación** para confirmar.

      ![](assets/stop-delegation-nwe.png)

### Ver aprobaciones delegadas {#view-delegated-approvals}

En la lista de trabajo solo puede ver los siguientes tipos de delegaciones de aprobación:

* Aprobaciones del proyecto
* Aprobaciones de tareas
* Aprobaciones de problemas

Para ver las aprobaciones delegadas:

1. Haga clic en el **Página principal** icono ![](assets/home-icon-30x29.png) en la esquina superior izquierda de Adobe Workfront.

   >[!NOTE]
   El administrador de Workfront puede realizar los siguientes cambios en el icono Inicio de su entorno:
   * Sustitúyala por una imagen personalizada para ilustrar su organización. En este caso, el icono tendrá un aspecto diferente al que se muestra en este artículo.
   * Reemplace la página vinculada por una página diferente. En este caso, haga clic en el botón **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de la página, haga clic en **Página principal**.


1. Haga clic en el **Filtro** menú desplegable y haga clic en **Aprobaciones**.\
   Todas las aprobaciones se muestran en la lista de forma predeterminada, incluidas las aprobaciones asignadas a usted y las aprobaciones delegadas a usted.

   ![](assets/delegated-to-me-nwe-350x93.png)
