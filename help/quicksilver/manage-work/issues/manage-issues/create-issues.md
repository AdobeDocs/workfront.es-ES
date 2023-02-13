---
product-area: projects
navigation-topic: manage-issues
title: Crear problemas
description: Mientras trabaja en un proyecto, es posible que descubra que se producen eventos inesperados. Puede registrar estos eventos inesperados como problemas para un proyecto en particular o para una tarea. Los usuarios con el acceso adecuado pueden ver y supervisar el estado de los problemas a medida que el proyecto o la tarea avanza hasta su finalización, lo que elimina la necesidad de largas cadenas de correo electrónico o reuniones de estado. A diferencia de las tareas, que son eventos planificados, los problemas representan elementos de trabajo no planificados en Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# Crear problemas

Mientras trabaja en un proyecto, es posible que descubra que se producen eventos inesperados. Puede registrar estos eventos inesperados como problemas para un proyecto en particular o para una tarea. Los usuarios con el acceso adecuado pueden ver y supervisar el estado de los problemas a medida que el proyecto o la tarea avanza hasta su finalización, lo que elimina la necesidad de largas cadenas de correo electrónico o reuniones de estado. A diferencia de las tareas, que son eventos planificados, los problemas representan elementos de trabajo no planificados en Adobe Workfront.

También puede agregar problemas a los proyectos como solicitudes. Para obtener más información, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Los problemas y las solicitudes se utilizan de forma intercambiable en Workfront. Puede registrar problemas tanto en proyectos como en tareas para indicar el trabajo imprevisto que debe solucionarse. También puede enviar solicitudes que se registren como problemas en un proyecto designado como cola de solicitud.

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
   <td> <p>Revisar o posterior para agregar problemas a un proyecto o tarea</p> <p>Solicite o superior que agregue problemas como solicitudes, utilizando una cola de solicitud.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Ver o acceder más a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas en el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concesión de acceso a problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Contribute o permisos superiores con capacidad para Añadir problemas a la tarea o proyecto en el que cree el problema</p> <p> Para obtener información sobre la concesión de permisos a problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre la solicitud de permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitaciones en la creación de problemas

Cuando tenga el acceso y los permisos correctos, puede crear problemas en un proyecto o tarea. Sin embargo, los siguientes son casos en los que es posible que no pueda crear problemas:

* El administrador de Workfront o un administrador de grupo deben habilitar la adición de problemas a un proyecto que esté en estado Finalizado o Muerto en el área Preferencias del proyecto . Para obtener información sobre cómo definir las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* No se pueden agregar problemas a un proyecto que esté en Pendiente de aprobación.

## Preparar el formulario Nuevo problema

Su organización debe tener un proceso bien definido para cuándo y cómo registrar un problema. Al configurar este proceso, el primer paso es crear el formulario necesario para enviar un problema. Tanto si permite que se agreguen problemas a tareas y proyectos directamente como si tiene colas de solicitud en las que se envían problemas, puede definir qué campos de Workfront y qué campos personalizados están disponibles para los usuarios cuando envían nuevos problemas y deben completarse. El formulario Nuevo problema puede contener información importante que será útil para resolver el problema rápidamente.

Los campos de los nuevos problemas de un proyecto se definen en la sección Detalles de cola del proyecto donde se registrarán los problemas. Para obtener información sobre la configuración de la sección Detalles de cola del proyecto, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Para obtener información sobre la creación de problemas al enviarlos a una cola de solicitudes, consulte la [Crear problemas introduciendo una nueva solicitud](#create-issues-by-entering-a-new-request) en este artículo.

## Creación de problemas en una tarea o proyecto mediante el botón Nuevo problema

Una vez definidos los campos de un nuevo formulario de problemas en el proyecto, puede empezar a crear problemas.

Para crear un problema en una tarea o un proyecto:

1. Vaya a un proyecto en el que desee crear el problema.
1. (Opcional) Si desea registrar el problema para una tarea, vaya a la **Tareas** y, a continuación, haga clic en el nombre de una tarea.
1. Haga clic en el **Problemas** para obtener más información.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Haga clic en **Nuevo problema**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (Condicional) Si el creador del proyecto ha creado Temas de cola o Grupos de temas en el proyecto, estos se añaden al nuevo formulario de problemas. Especifique la variable **Grupo de temas** o **Tema de cola** de su nuevo número. Deben tener nombres personalizados para su entorno.\
   Para obtener más información sobre la creación de grupos de temas, consulte [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obtener más información sobre la creación de temas de cola, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * Si solo hay un tema de cola definido en el proyecto, se muestra automáticamente.
   * Si el grupo de temas no tiene ningún tema de cola o grupo de temas debajo de él, no hay nada disponible en la lista desplegable del grupo de temas.

1. (Condicional) Si el creador del proyecto puede usar la variable **Tipo de problema** para mostrarlo en el formulario Nuevo problema, seleccione el tipo de problema entre las siguientes opciones:

   * Informe de errores
   * Solicitud de cambio
   * Problema
   * Solicitud\
      Dependiendo de cómo haya configurado el administrador de Workfront sus preferencias de proyecto, los nombres de los tipos de problemas pueden ser diferentes para usted.

1. Especifique cualquiera de los campos disponibles en la variable **Nuevo problema** formulario. Para obtener más información sobre la definición de campos al introducir un nuevo problema, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).
1. (Condicional) Si los temas de cola están asociados a un formulario personalizado, ese formulario personalizado se mostrará en la **Nuevo problema** formulario.\
   O\
   Si el proyecto está asociado con un formulario personalizado de problemas a través del área Detalles de la cola , el formulario se muestra en la **Nuevo problema** en los campos predeterminados de Workfront.

   Para obtener más información, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Haga clic en **Guardar nuevo problema.**

Los problemas se pueden asignar a varios usuarios, funciones de trabajo o a un equipo. Para obtener más información sobre la asignación y administración de solicitudes, consulte [Administrar solicitudes de trabajo y equipo](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

## Crear problemas en una tarea o proyecto en línea

>[!IMPORTANT]
>
>El propietario del proyecto debe habilitar **Permitir que los usuarios agreguen problemas en línea** al definir la configuración de problemas del proyecto, antes de poder agregar problemas en línea al proyecto o las tareas. Para obtener información sobre la configuración de problemas en un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

Cuando desee agregar varios problemas rápidamente, puede crear problemas para una tarea o un proyecto en línea, agregándolos a una lista de problemas.

>[!NOTE]
>
>Cuando se agregan problemas en línea, Workfront no aplica el formulario Nuevo problema a los nuevos problemas. No se recomienda añadir problemas en línea si desea que los usuarios proporcionen cierta información al introducir problemas. Esto puede tener un impacto negativo en los informes de problemas y más tarde en la capacidad del usuario asignado al problema de tener toda la información necesaria para resolver el problema.

Para crear problemas en línea:

1. Vaya a un proyecto en el que desee crear el problema.
1. (Opcional) Si desea registrar el problema para una tarea, vaya a la **Tareas** y, a continuación, haga clic en el nombre de una tarea.
1. Haga clic en el **Problemas** para obtener más información.
1. Haga clic en **Agregar más problemas**.

   Se crea una nueva línea en la lista de problemas de la sección Problemas .

   >[!TIP]
   >
   >Esta opción aparece atenuada si se anula la selección de Permitir a los usuarios agregar problemas en línea en el cuadro Editar proyecto . Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Empiece a escribir el nombre del problema en el campo Nombre y, a continuación, siga agregando más información sobre el problema en línea.

   >[!TIP]
   >
   >Los campos disponibles para editar en línea están disponibles en la vista que aplique a la lista de problemas. Es posible que no pueda editar en línea los siguientes tipos de campos:
   >   
   >* Campos que pertenecen a otro objeto
   >* Campos a los que no tiene acceso para editar
   >* Campos que son cálculos y que Workfront actualiza automáticamente


1. Haga clic en Entrar para finalizar la edición en línea y agregue el problema al proyecto o la tarea.

## Crear problemas introduciendo una nueva solicitud {#create-issues-by-entering-a-new-request}

Puede designar proyectos para que sean receptáculos para recibir problemas. Este tipo de proyectos se llaman Solicitar colas en Workfront. Puede acceder a Solicitar colas a través del área Solicitudes del menú principal.

>[!TIP]
>
>Los términos &quot;problema&quot; y &quot;solicitud&quot; se pueden intercambiar en Workfront.

Para obtener más información sobre cómo configurar proyectos como colas de solicitud para recibir problemas, consulte [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Para obtener información sobre el envío de solicitudes, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
