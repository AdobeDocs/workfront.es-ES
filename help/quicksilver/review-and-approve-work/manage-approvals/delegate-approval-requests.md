---
product-area: projects
navigation-topic: approvals
title: Delegar solicitud de aprobación
description: La delegación de solicitudes de aprobación le permite asignar a otro usuario para que apruebe sus solicitudes durante un período de tiempo, por ejemplo, si va a estar fuera de la oficina en vacaciones.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: c6e3e3d8d4fd6b6916c8fd49983bc3572949acaa
workflow-type: tm+mt
source-wordcount: '1262'
ht-degree: 0%

---

# Delegar solicitud de aprobación

Puede delegar temporalmente el trabajo al que esté asignado mientras esté fuera de la oficina. Puede delegar asignaciones de tareas y problemas o delegar solicitudes de aprobación. Este artículo describe cómo delegar solicitudes de aprobación. Para obtener información sobre la delegación de asignaciones de tareas y problemas, consulte [Administrar delegación de tareas y problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

Puede delegar los siguientes tipos de aprobaciones, independientemente de cómo se le haya asignado la aprobación (ya sea directamente a usted, a un equipo del que sea miembro o a su función):

* Aprobaciones de proyecto
* Aprobaciones de tareas
* Aprobaciones de problema

No puede delegar aprobaciones de hojas de horas, documentos o pruebas.

>[!NOTE]
>
>Para garantizar que no se produzcan incoherencias con las fechas programadas para delegar sus aprobaciones, recomendamos que la zona horaria del perfil de usuario coincida con la de su programación. Para obtener más información, consulte los siguientes artículos:
>
>* [Crear una programación](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Editar el perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>plan Adobe Workfront*</p></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan o tipo de licencia tiene, póngase en contacto con su administrador de Workfront.

+++

## Comprender el acceso de los usuarios para aprobaciones delegadas

Durante el período de aprobación designado, el usuario al que delega una solicitud de aprobación tiene las siguientes capacidades:

* Puede aprobar o rechazar solicitudes de aprobación existentes cuando no se haya tomado ninguna decisión
* Pueden aprobar y rechazar nuevas solicitudes de aprobación recibidas durante un período de tiempo especificado
* Se concede acceso de visualización a los objetos que esperan aprobación

  >[!NOTE]
  >
  > El administrador de Adobe Workfront puede restringir el acceso de los usuarios a ciertos tipos de objetos. Cuando un usuario no tiene acceso a un tipo de objeto y se le delega una aprobación de ese tipo, el usuario no tiene acceso de visualización al objeto. Sin embargo, el usuario puede aprobar o rechazar solicitudes de aprobación desde la página **Inicio**, tal como se describe en [Aprobación del trabajo](../../review-and-approve-work/manage-approvals/approving-work.md).\
  >Por ejemplo, el usuario A pertenece al grupo A. El administrador de Workfront ha restringido los derechos de acceso del grupo A, de modo que los usuarios de este grupo no pueden ver las tareas dentro de Workfront. Si se delega una solicitud de aprobación de tarea al usuario A, este no podrá ver la tarea a la que está asociada la aprobación. Sin embargo, el usuario A puede aprobar o rechazar la solicitud de aprobación desde la página de inicio.

  Para obtener información acerca de cómo el administrador de Workfront puede restringir el acceso a los tipos de objeto en la instalación, consulte  [Crear o modificar niveles de acceso personalizados](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

Una vez cancelada o detenida la delegación de aprobación, el usuario designado como aprobador:

* Ya no tiene acceso para aprobar el trabajo de los elementos que requieren aprobación
* Sigue teniendo acceso de visualización de los elementos de trabajo\
  Los usuarios a los que se les ha concedido el acceso de Vista a objetos a través de una delegación de aprobación conservan ese acceso de Vista incluso después de que la delegación de aprobación se detenga o se recupere. Para eliminar el acceso de visualización a cualquier objeto al que el usuario tuviera acceso durante el tiempo en que se delegaban las aprobaciones, debe ir al objeto y eliminar los derechos de acceso directamente del objeto.

## Delegar solicitudes de aprobación en el área de Inicio

Puede delegar solicitudes de aprobación desde el área de Inicio.

### Delegar sus aprobaciones a otro usuario {#delegate-your-approvals-to-another-user}

Puede delegar los siguientes tipos de aprobaciones, independientemente de cómo se le haya asignado la aprobación (ya sea directamente a usted, a un equipo del que sea miembro o a su función):

* Aprobaciones de proyecto
* Aprobaciones de tareas
* Aprobaciones de problema

No puede delegar aprobaciones de hojas de horas, documentos o pruebas.

Tenga en cuenta lo siguiente al delegar aprobaciones:

* Al delegar aprobaciones, se delegan todas las aprobaciones. No puede delegar solicitudes de aprobación individuales.
* Puede delegar aprobaciones a un solo usuario; no puede delegarlas a varios usuarios al mismo tiempo.\
  Todas las aprobaciones de todos los proyectos, tareas y problemas se delegan al usuario que designe.
* Un máximo de 5 usuarios puede delegar aprobaciones al mismo usuario al mismo tiempo. En otras palabras, un solo usuario no puede designarse como aprobador temporal para más de 5 usuarios al mismo tiempo.
* La actividad relativa a las aprobaciones se muestra en la pestaña Actualizaciones. Debe tener activada la opción Mostrar actualizaciones del sistema. Tanto el usuario que delega la aprobación como el usuario al que se delegan las aprobaciones reciben una notificación por correo electrónico en relación con la actividad de aprobación.

Para delegar aprobaciones a otro usuario:

1. Haga clic en el icono **Inicio** ![](assets/home-icon-30x29.png) en la esquina superior izquierda de Adobe Workfront.

   >[!NOTE]
   >
   >El administrador de Workfront puede realizar los siguientes cambios en el icono Inicio de su entorno:
   >
   >* Sustitúyala por una imagen personalizada para ilustrar su organización. En este caso, el icono tendrá un aspecto diferente al que se muestra en este artículo.
   >* Reemplace la página vinculada a ella por una página diferente. En este caso, haga clic en **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de la página y, a continuación, haga clic en **Inicio**.

   O

   Haga clic en el icono **Menú principal** > **su nombre** > **Tiempo libre** en el panel izquierdo.

1. (Opcional y condicional) En el área de Inicio, haga clic en el menú desplegable **Filtro** y luego haga clic en **Aprobaciones**.

1. (Condicional) Haga Clic En **Delegar Mis Aprobaciones**

   O

   Si el administrador del sistema o del grupo habilitó la delegación de tareas y problemas, haga clic en **Delegar** y luego en **Delegar aprobaciones**.

   ![](assets/delegate-approvals-nwe.png)

1. Especifique la siguiente información en la sección Delegar mis aprobaciones:

   * **Nombre**: empiece a escribir el nombre del usuario al que desea delegar las aprobaciones y, a continuación, haga clic en el nombre cuando aparezca en el menú desplegable.
   * **Fecha de inicio**: seleccione la fecha para que las aprobaciones comiencen a reenviarse. El reenvío comienza a las 12:00 a.m. en la fecha que seleccione.\
     La fecha de inicio debe ser la fecha actual o una fecha futura.
   * **Fecha de finalización**:Realice una de las siguientes acciones:

      * Seleccione la fecha para que las aprobaciones dejen de reenviarse. El reenvío finaliza a las 23:59 en la fecha que seleccione.
      * Seleccione **Sin fecha de finalización** para configurar Workfront para delegar aprobaciones indefinidamente.

1. Haga clic en **Guardar**.

### Actualización o detención de una delegación de aprobación {#update-or-stop-an-approval-delegation}

1. Haga clic en el icono **Inicio** ![](assets/home-icon-30x29.png) en la esquina superior izquierda de Adobe Workfront.

   >[!NOTE]
   >
   >El administrador de Workfront puede realizar los siguientes cambios en el icono Inicio de su entorno:
   >
   >* Sustitúyala por una imagen personalizada para ilustrar su organización. En este caso, el icono tendrá un aspecto diferente al que se muestra en este artículo.
   >* Reemplace la página vinculada a ella por una página diferente. En este caso, haga clic en **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de la página y, a continuación, haga clic en **Inicio**.

1. Haga clic en el menú desplegable **Filtro** y luego haga clic en **Aprobaciones**.

1. (Condicional) Haga clic en **Editar delegación**

   O

   Si el administrador del sistema o del grupo habilitó la delegación de tareas y problemas, haga clic en **Editar delegación** y luego haga clic en **Delegar aprobaciones**.

1. (Condicional) Realice una de las acciones siguientes:

   * Para actualizar la delegación de aprobación existente: cambie la información mostrada y haga clic en **Guardar**.

   * Para detener la delegación existente: haga clic en **Detener delegación** y luego haga clic en **Detener delegación** para confirmar.

     ![](assets/stop-delegation-nwe.png)

### Ver aprobaciones delegadas {#view-delegated-approvals}

En la Lista de trabajos se pueden ver únicamente los siguientes tipos de delegaciones de aprobación:

* Aprobaciones de proyecto
* Aprobaciones de tareas
* Aprobaciones de problema

Para ver aprobaciones delegadas:

1. Haga clic en el icono **Inicio** ![](assets/home-icon-30x29.png) en la esquina superior izquierda de Adobe Workfront.

   >[!NOTE]
   >
   >El administrador de Workfront puede realizar los siguientes cambios en el icono Inicio de su entorno:
   >
   >* Sustitúyala por una imagen personalizada para ilustrar su organización. En este caso, el icono tendrá un aspecto diferente al que se muestra en este artículo.
   >* Reemplace la página vinculada a ella por una página diferente. En este caso, haga clic en **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de la página y, a continuación, haga clic en **Inicio**.

1. Haga clic en el menú desplegable **Filtro** y luego haga clic en **Aprobaciones**.\
   Todas las aprobaciones se muestran en la lista de forma predeterminada, incluidas las aprobaciones que se le han asignado y las que le han delegado.

   ![](assets/delegated-to-me-nwe-350x93.png)
