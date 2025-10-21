---
product-area: projects
navigation-topic: manage-issues
title: Crear problemas
description: Mientras trabaja en un proyecto, es posible que descubra que surgen eventos inesperados. Puede registrar esos eventos inesperados como problemas de un proyecto concreto o de una tarea. Los usuarios con el acceso adecuado pueden ver y supervisar el estado de los problemas a medida que el proyecto o la tarea progresa hasta su finalización, lo que elimina la necesidad de largas cadenas de correo electrónico o reuniones de estado. A diferencia de las tareas, que son eventos planificados, los problemas representan elementos de trabajo no planificados en Adobe Workfront.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 89%

---

# Crear problemas

<!--Audited: 08/2025-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

Mientras trabaja en un proyecto, es posible que descubra que surgen eventos inesperados. Puede registrar esos eventos inesperados como problemas de un proyecto concreto o de una tarea. Los usuarios con el acceso adecuado pueden ver y supervisar el estado de los problemas a medida que el proyecto o la tarea progresa hasta su finalización, lo que elimina la necesidad de largas cadenas de correo electrónico o reuniones de estado. A diferencia de las tareas, que son eventos planificados, los problemas representan elementos de trabajo no planificados en Adobe Workfront.

También puede añadir problemas a proyectos como solicitudes. Para obtener más información, consulte [Crear y enviar solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Los problemas y las solicitudes se utilizan de forma intercambiable en Workfront. Puede registrar los problemas tanto de los proyectos como de las tareas para indicar el trabajo imprevisto que debe resolverse. También puede enviar solicitudes que se registren como problemas en un proyecto designado como una cola de solicitudes.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <ul><li>Colaborador o superior</li>
   <li>Ligero o superior para editar problemas en la sección Problemas de una tarea o proyecto</li></ul>
   O
   <ul><li>Solicitud o superior</li> <li>Revise o superior para editar problemas en la sección Problemas de una tarea o proyecto</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Acceso de visualización o superior a proyectos y tareas</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de aportación o superiores con capacidad para añadir problemas a la tarea o el proyecto donde crea el problema</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license:</p>
   <ul><li>Contributor or higher</li>
   <li>Light or higher to edit issues in the Issues section of a task or project</li></ul>
   <p>Current license:</p>
  <ul><li>Request or higher</li> <li>Review or higher to edit issues in the Issues section of a task or a project</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions with ability to Add Issues to the task or project where you create the issue</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitaciones en la creación de problemas

Cuando disponga de los permisos y el acceso correctos, podrá crear problemas en un proyecto o tarea. Sin embargo, en los siguientes casos es posible que no pueda crear problemas:

* El administrador de Workfront o de un grupo debe habilitar la adición de problemas a un proyecto que esté en estado completado o inactivo en el área de Preferencias del proyecto. Para obtener información sobre cómo establecer las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* No puede añadir problemas a un proyecto que esté pendiente de aprobación.

## Preparar el formulario Nuevo problema

Su organización debe contar con un proceso bien definido sobre cuándo y cómo registrar un problema. Al configurar este proceso, el primer paso es crear el formulario necesario para enviar un problema.

Los usuarios pueden agregar problemas a un proyecto de las siguientes maneras:

* Añádalos directamente a tareas y proyectos.
* Enviarlos a una cola de solicitudes.

El formulario Nuevo problema puede contener información importante que resulta útil para resolver el problema rápidamente.

Puede configurar el formulario Nuevo problema para que incluya la siguiente información cuando los usuarios agreguen problemas al proyecto o a sus tareas:

* Campos personalizados
* Rutas de aprobación
* Asignaciones (Reglas de enrutamiento)

Los campos para nuevos problemas o solicitudes se definen en la sección Detalles de cola del proyecto, donde se registrarán los problemas.

Para obtener información acerca de cómo configurar la sección Detalles de la cola de un proyecto, vea [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Para obtener información sobre cómo crear problemas enviándolos a una cola de solicitudes, consulte la sección [Crear problemas al introducir una nueva solicitud](#create-issues-by-entering-a-new-request) en este artículo.

## Crear problemas en una tarea o proyecto mediante el botón Nuevo problema

Después de definir los campos del formulario de un nuevo problema en el proyecto, puede empezar a crear problemas.

Para crear un problema en una tarea o un proyecto, siga estos pasos:

1. Vaya a un proyecto en el que desee crear el problema.
1. (Opcional) Si desea registrar el problema de una tarea, vaya al área **Tareas** y luego haga clic en el nombre de una tarea.
1. Haga clic en la sección **Problemas**.

   Se muestra la lista de problemas del proyecto

1. Haga clic en **Nuevo problema** en la parte superior de la lista de problemas.
Se muestra el cuadro Nuevo problema.

   ![Nuevo cuadro de problemas](assets/new-issue-box-matches-new-request-ui.png)

1. (Condicional) Si el creador del proyecto creó temas de la cola o grupos de temas en el proyecto, se añadirán al formulario de nuevo problema. Especifique el **Grupo de temas** o el **Tema de la cola** del nuevo problema. Los grupos de temas y los temas de la cola tienen nombres personalizados según su entorno.\
   Para obtener más información sobre cómo crear grupos de temas, vea [Creación de grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obtener más información acerca de cómo crear temas de la cola, vea [Creación de temas de la cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Si solo hay un tema de la cola definido en el proyecto, se muestra de forma automática.
   * Si el grupo de temas no tiene ningún tema de la cola o grupo de temas debajo, no hay nada disponible en la lista desplegable Grupo de temas.

1. Ponga el nombre del problema en el campo **Asunto** y después añada una **Descripción**.

1. (Condicional) Si el creador del proyecto permitió que el campo **Tipo de solicitud** se mostrara en el formulario Nuevo problema, seleccione el tipo de problema en las siguientes opciones:

   * Informe de errores
   * Solicitud de cambio
   * Problema
   * Solicitud\
     Según la configuración dada por el administrador de Workfront a sus Preferencias del proyecto, los nombres de los tipos de problemas podrían ser diferentes para usted.

   >[!TIP]
   >
   >Los tipos de solicitud deben habilitarse en Detalles de la cola y al crear el tema de la cola para que se muestre como una selección en el formulario Nuevo problema. Para obtener más información, consulte los siguientes artículos:
   >
   >* [Creación de una cola de solicitudes](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >* [Creación de temas de cola](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Continúe especificando los campos disponibles en el formulario **Nuevo problema**. Para obtener más información acerca de los campos disponibles al introducir un problema nuevo, consulte [Edición de problemas](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >No todos los campos relacionados con el problema están disponibles en el formulario Nuevo problema. El creador del proyecto habilita los campos disponibles al crear un problema cuando definen el área Detalles de la cola del proyecto. Para obtener más información, vea [Creación de una cola de solicitudes](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Condicional) Si los temas de la cola están asociados a un formulario personalizado, este se mostrará en el formulario **Nuevo problema**.\
   O\
   Si el proyecto está asociado con un formulario personalizado de problema mediante el área Detalles de la cola, el formulario se mostrará en el formulario **Nuevo problema**, después de los campos predeterminados de Workfront.

   Para obtener más información, vea [Creación de una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Haga clic en **Enviar**.

   Los problemas se pueden asignar a varios usuarios, funciones del puesto o a un equipo. Para obtener más información sobre cómo asignar y administrar solicitudes, vea [Administración de solicitudes de trabajo y equipo](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).


## Creación de problemas en línea de una tarea o proyecto

>[!IMPORTANT]
>
>El propietario del proyecto debe habilitar **Permitir que los usuarios añadan problemas en línea** al definir la configuración de problemas del proyecto para que pueda añadir problemas en línea al proyecto o a las tareas. Para obtener información acerca de cómo configurar los problemas de un proyecto, vea [Edición de proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Si desea añadir varios problemas rápido, puede crearlos para una tarea o un proyecto en línea añadiéndolos a una lista de problemas.

>[!NOTE]
>
>Cuando añade problemas en línea, Workfront no aplica el formulario Nuevo problema a los nuevos problemas. No se recomienda añadir problemas en línea si desea que los usuarios proporcionen cierta información al introducir problemas. Esto puede tener un impacto negativo en la creación de informes de problemas y, después, en la capacidad del usuario asignado al problema para tener toda la información necesaria para resolverlo.

Para crear problemas en línea, siga estos pasos:

1. Vaya a un proyecto en el que desee crear el problema.
1. (Opcional) Si desea registrar el problema para una tarea, vaya a la sección **Tareas** y, a continuación, haga clic en el nombre de una tarea.
1. Haga clic en **Problemas** en el panel izquierdo.
1. Haga clic en **Añadir más problemas** en la parte inferior de la lista de problemas.

   Se crea una nueva línea en la lista de problemas de la sección Problemas.

   >[!TIP]
   >
   >Esta opción aparece atenuada si la opción Permitir que los usuarios añadan problemas en línea no está seleccionada en el cuadro Editar proyecto. Para obtener más información, consulte [Edición de proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![Botón Agregar más problemas](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Empiece a escribir el nombre del problema en el campo Nombre y, a continuación, continúe añadiendo más información sobre el problema en línea.

   >[!TIP]
   >
   >Los campos que están disponibles para editar en línea los proporciona la vista que aplique a la lista de problemas. Es posible que no pueda editar en línea el siguiente tipo de campos:
   >   
   >* Campos que pertenecen a otro objeto
   >* Campos en los que no tiene acceso para editar
   >* Campos que son cálculos y que Workfront actualiza de forma automática

1. Haga clic en Intro para finalizar la edición en línea y añada el problema al proyecto o tarea.

## Creación de problemas al introducir una nueva solicitud {#create-issues-by-entering-a-new-request}

Puede designar proyectos para que sean receptáculos de recepción de problemas. Este tipo de proyectos se denominan Colas de solicitudes en Workfront. Puede acceder a Colas de solicitudes desde el área Solicitudes del menú principal.

>[!TIP]
>
>Los términos “problema” y “solicitud” son intercambiables en Workfront.

Para obtener más información acerca de cómo configurar proyectos como colas de solicitudes para recibir problemas, vea [Creación de una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Para obtener información sobre cómo enviar solicitudes, consulte [Creación y envío de solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
