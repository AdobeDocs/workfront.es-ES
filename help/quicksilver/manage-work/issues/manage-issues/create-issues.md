---
product-area: projects
navigation-topic: manage-issues
title: Crear problemas
description: Mientras trabaja en un proyecto, es posible que descubra que se producen eventos inesperados. Puede registrar esos eventos inesperados como problemas para un proyecto en particular o de una tarea. Los usuarios con el acceso adecuado pueden ver y supervisar el estado de los problemas a medida que el proyecto o la tarea progresa hasta su finalización, lo que elimina la necesidad de largas cadenas de correo electrónico o reuniones de estado. A diferencia de las tareas, que son eventos planificados, los problemas representan elementos de trabajo no planificados en Adobe Workfront.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: b6ea67f28b498cc0de4325a2350545c660574d4c
workflow-type: tm+mt
source-wordcount: '2024'
ht-degree: 0%

---

# Crear problemas

<!--remove Preview and Prod references when this comes to Prod-->

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes de o en el entorno de producción para los clientes que habilitaron versiones rápidas de. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

<span class="preview">Para obtener más información sobre la versión actual, consulte [Resumen de la versión del cuarto trimestre de 2023](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>



Mientras trabaja en un proyecto, es posible que descubra que se producen eventos inesperados. Puede registrar esos eventos inesperados como problemas para un proyecto en particular o de una tarea. Los usuarios con el acceso adecuado pueden ver y supervisar el estado de los problemas a medida que el proyecto o la tarea progresa hasta su finalización, lo que elimina la necesidad de largas cadenas de correo electrónico o reuniones de estado. A diferencia de las tareas, que son eventos planificados, los problemas representan elementos de trabajo no planificados en Adobe Workfront.

También puede agregar problemas a proyectos como solicitudes. Para obtener más información, consulte [Creación y envío de solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Los problemas y las solicitudes se utilizan de forma intercambiable en Workfront. Puede registrar los problemas tanto de los proyectos como de las tareas para indicar el trabajo imprevisto que debe solucionarse. También puede enviar solicitudes que se registren como problemas en un proyecto designado como Cola de solicitudes.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revise o superior para agregar problemas a un proyecto o tarea</p> <p>Solicitud o superior para agregar problemas como solicitudes mediante una cola de solicitudes.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Acceso de visualización o superior a Proyectos y tareas</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas del nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Conceder acceso a los problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de contribución o superiores con capacidad para agregar problemas a la tarea o proyecto donde crea el problema</p> <p> Para obtener información sobre la concesión de permisos a los problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre cómo solicitar permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Limitaciones en la creación de problemas

Cuando tenga los permisos y el acceso correctos, podrá crear problemas en un proyecto o tarea. Sin embargo, los siguientes son casos en los que es posible que no pueda crear problemas:

* El administrador de Workfront o de un grupo debe habilitar la adición de problemas a un proyecto que esté en estado completo o muerto en el área de Preferencias del proyecto. Para obtener información sobre cómo establecer las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* No puede agregar problemas a un proyecto que tenga Aprobación pendiente.

## Preparar el formulario Nuevo problema

Su organización debe tener un proceso bien definido para cuándo y cómo registrar un problema. Al configurar este proceso, el primer paso es crear el formulario necesario para enviar un problema. Tanto si permite que los problemas se agreguen directamente a tareas y proyectos, como si tiene colas de solicitudes en las que se envían problemas, puede definir qué campos de Workfront, así como qué campos personalizados están disponibles para los usuarios cuando envían nuevos problemas y deben completarse. El formulario Nuevo problema puede contener información importante que resulta útil para resolver el problema rápidamente.

Los campos para los nuevos problemas de un proyecto se definen en la sección Detalles de cola del proyecto, donde se registrarán los problemas. Para obtener información sobre cómo configurar la sección Detalles de cola del proyecto, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Para obtener información sobre cómo crear problemas enviándolos a una cola de solicitudes, consulte la [Crear problemas al introducir una nueva solicitud](#create-issues-by-entering-a-new-request) de este artículo.

## Crear problemas en una tarea o proyecto mediante el botón Nuevo problema

Después de definir los campos de un formulario de nuevo problema en el proyecto, puede empezar a crear problemas.

La creación de problemas difiere según el entorno en el que decida crear el problema.

### Cree problemas en una tarea o proyecto con el botón Nuevo problema del entorno de producción

Para crear un problema en una tarea o un proyecto:

1. Vaya a un proyecto en el que desee crear el problema.
1. (Opcional) Si desea registrar el problema de una tarea, vaya a **Tareas** y, a continuación, haga clic en el nombre de una tarea.
1. Haga clic en **Problemas** sección.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Clic **Nuevo problema**.

   ![](assets/qs-issue-list-on-project-with-new-issue-button-highlighted-350x270.png)

1. (Condicional) Si el creador del proyecto creó temas de la cola o grupos de temas en el proyecto, se agregarán al formulario de nuevo problema. Especifique el **Grupo de temas** o el **Tema de cola** de su nuevo problema. Los grupos de temas y los temas de colas tienen nombres personalizados según su entorno.\
   Para obtener más información sobre la creación de grupos de temas, consulte [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obtener más información sobre la creación de temas de colas, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * Si solo hay un tema de la cola definido en el proyecto, se muestra automáticamente.
   * Si el grupo de temas no tiene ningún tema de cola o grupo de temas debajo, no hay nada disponible en la lista desplegable Grupo de temas.

1. (Condicional) Si el creador del proyecto permite el **Tipo de solicitud** para mostrar en el formulario Nuevo problema, seleccione el tipo de problema de entre las siguientes opciones:

   * Informe de errores
   * Solicitud de cambio
   * Problema
   * Solicitud\
     Según la configuración dada por el administrador de Workfront a sus Preferencias del proyecto, los nombres de los tipos de problemas podrían ser diferentes para usted.

   >[!TIP]
   >
   >Los tipos de solicitud deben habilitarse en Detalles de cola y al crear el tema de cola para que se muestre como una selección en el formulario Nuevo problema. Para obtener más información, consulte los siguientes artículos:
   >* [Crear una cola de solicitudes](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Crear temas de cola](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Añada un nombre para el nuevo problema en la **Nombre de problema** field.
1. Siga especificando los campos disponibles en la **Nuevo problema** formulario. Para obtener más información sobre los campos disponibles al introducir un problema nuevo, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >No todos los campos relacionados con el problema están disponibles en el formulario Nuevo problema. El creador del proyecto habilita los campos disponibles al crear un problema cuando definen el área Detalles de cola del proyecto. Para obtener más información, consulte [Crear una cola de solicitudes](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Condicional) Si los temas de la cola están asociados a un formulario personalizado, ese formulario personalizado se mostrará en la **Nuevo problema** formulario.\
   O\
   Si el proyecto está asociado con un formulario personalizado de problema mediante el área Detalles de la cola, el formulario se muestra en la variable **Nuevo problema** , después de los campos predeterminados de Workfront.

   Para obtener más información, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Haga clic en **Guardar nuevo problema.**

Los problemas se pueden asignar a varios usuarios, funciones del puesto o a un equipo. Para obtener más información sobre la asignación y administración de solicitudes, consulte [Administrar solicitudes de trabajo y equipo](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content: -->

<div class="preview">

### Crear problemas en una tarea o proyecto mediante el botón Nuevo problema del entorno de vista previa

Para crear un problema en una tarea o un proyecto:

1. Vaya a un proyecto en el que desee crear el problema.
1. (Opcional) Si desea registrar el problema de una tarea, vaya a **Tareas** y, a continuación, haga clic en el nombre de una tarea.
1. Haga clic en **Problemas** sección.

   ![](assets/qs-issues-icon-highlighted-on-project-350x216.png)

1. Clic **Nuevo problema**.
Se muestra el cuadro Nuevo problema.

   ![](assets/new-issue-box-matches-new-request-ui.png)

1. (Condicional) Si el creador del proyecto creó temas de la cola o grupos de temas en el proyecto, se agregarán al formulario de nuevo problema. Especifique el **Grupo de temas** o el **Tema de cola** de su nuevo problema. Los grupos de temas y los temas de colas tienen nombres personalizados según su entorno.\
   Para obtener más información sobre la creación de grupos de temas, consulte [Crear grupos de temas](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Para obtener más información sobre la creación de temas de colas, consulte [Crear temas de cola](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Si solo hay un tema de la cola definido en el proyecto, se muestra automáticamente.
   * Si el grupo de temas no tiene ningún tema de cola o grupo de temas debajo, no hay nada disponible en la lista desplegable Grupo de temas.

1. Añada el nombre del problema en la **Asunto** y, a continuación, añada un **Descripción**.

1. (Condicional) Si el creador del proyecto permite el **Tipo de solicitud** para mostrar en el formulario Nuevo problema, seleccione el tipo de problema de entre las siguientes opciones:

   * Informe de errores
   * Solicitud de cambio
   * Problema
   * Solicitud\
     Según la configuración dada por el administrador de Workfront a sus Preferencias del proyecto, los nombres de los tipos de problemas podrían ser diferentes para usted.

   >[!TIP]
   >
   >Los tipos de solicitud deben habilitarse en Detalles de cola y al crear el tema de cola para que se muestre como una selección en el formulario Nuevo problema. Para obtener más información, consulte los siguientes artículos:
   >* [Crear una cola de solicitudes](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Crear temas de cola](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Siga especificando los campos disponibles en la **Nuevo problema** formulario. Para obtener más información sobre los campos disponibles al introducir un problema nuevo, consulte [Editar problemas](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >No todos los campos relacionados con el problema están disponibles en el formulario Nuevo problema. El creador del proyecto habilita los campos disponibles al crear un problema cuando definen el área Detalles de cola del proyecto. Para obtener más información, consulte [Crear una cola de solicitudes](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Condicional) Si los temas de la cola están asociados a un formulario personalizado, ese formulario personalizado se mostrará en la **Nuevo problema** formulario.\
   O\
   Si el proyecto está asociado con un formulario personalizado de problema mediante el área Detalles de la cola, el formulario se muestra en la variable **Nuevo problema** , después de los campos predeterminados de Workfront.

   Para obtener más información, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Clic **Enviar**.

   Los problemas se pueden asignar a varios usuarios, funciones del puesto o a un equipo. Para obtener más información sobre la asignación y administración de solicitudes, consulte [Administrar solicitudes de trabajo y equipo](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

</div>

## Crear problemas en línea de una tarea o proyecto

>[!IMPORTANT]
>
>El propietario del proyecto debe habilitar **Permitir que los usuarios agreguen problemas en línea** al definir la configuración de problemas del proyecto, antes de agregar problemas en línea al proyecto o a las tareas. Para obtener información sobre cómo configurar los problemas de un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Si desea agregar varios problemas rápidamente, puede crear problemas para una tarea o un proyecto en línea agregándolos a una lista de problemas.

>[!NOTE]
>
>Cuando agrega problemas en línea, Workfront no aplica el formulario Nuevo problema a los nuevos problemas. No se recomienda agregar problemas en línea si desea que los usuarios proporcionen determinada información al introducir problemas. Esto puede tener un impacto negativo en la creación de informes de problemas y, posteriormente, en la capacidad del usuario asignado al problema para tener toda la información necesaria para resolverlo.

Para crear problemas en línea:

1. Vaya a un proyecto en el que desee crear el problema.
1. (Opcional) Si desea registrar el problema de una tarea, vaya a **Tareas** y, a continuación, haga clic en el nombre de una tarea.
1. Haga clic en **Problemas** sección.
1. Clic **Agregar más problemas**.

   Se crea una nueva línea en la lista de problemas de la sección Problemas.

   >[!TIP]
   >
   >Esta opción aparece atenuada si la opción Permitir que los usuarios agreguen problemas en línea no está seleccionada en el cuadro Editar proyecto. Para obtener más información, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Empiece a escribir el nombre del problema en el campo Nombre y, a continuación, continúe añadiendo más información sobre el problema en línea.

   >[!TIP]
   >
   >Los campos que están disponibles para editar en línea los proporciona la vista que aplique a la lista de problemas. Es posible que no pueda editar en línea el siguiente tipo de campos:
   >   
   >* Campos que pertenecen a otro objeto
   >* Campos que no tiene acceso para editar
   >* Campos que son cálculos y que Workfront actualiza automáticamente

1. Haga clic en Entrar para finalizar la edición en línea y añada el problema al proyecto o tarea.

## Crear problemas al introducir una nueva solicitud {#create-issues-by-entering-a-new-request}

Puede designar proyectos para que sean receptáculos para la recepción de problemas. Este tipo de proyectos se denominan Colas de solicitudes en Workfront. Puede acceder a las colas de solicitudes a través del área de solicitudes del menú principal.

>[!TIP]
>
>Los términos &quot;problema&quot; y &quot;solicitud&quot; son intercambiables en Workfront.

Para obtener más información sobre cómo configurar proyectos como colas de solicitudes para recibir problemas, consulte [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Para obtener información sobre el envío de solicitudes, consulte [Creación y envío de solicitudes de Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
