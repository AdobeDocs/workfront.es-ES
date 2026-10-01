---
user-type: administrator
product-area: system-administration;setup
navigation-upperic: configure-locations
title: Configuración de colaboradores de IA
description: Como administrador de Adobe Workfront, puede configurar los colaboradores de IA y asignarlos a proyectos y tareas.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
source-git-commit: 3cf7495f827156fabac1214b38a104ed826d558c
workflow-type: tm+mt
source-wordcount: '1577'
ht-degree: 2%
---
# Configuración de colaboradores de IA

{{preview-fast-release-general}}

Los colaboradores de IA son una forma de incorporar agentes de IA en sus proyectos, tareas y problemas. Puede configurar un colaborador de IA y, a continuación, asignarlo como lo haría con un usuario.

Por ejemplo, puede configurar un colaborador de IA de tipo revisor con directrices de marca y, a continuación, asignar ese colaborador para que revise un documento.

Los tipos de AI Collaborator disponibles incluyen:

* Revisor de IA: cree un colaborador con marcas o Adobe Brand Intelligence y, a continuación, asígnelo como revisor en los recursos.

  Para obtener más información, consulte [Introducción al Revisor de IA de Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Agente de trabajo: cree un colaborador con una plataforma de IA estándar como Claude, OpenAI, Copilot o Writer y, a continuación, asigne al colaborador a una tarea o problema para completar los elementos de trabajo.

  Para obtener más información, vea [Usar agentes de trabajo](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

<!--
* <span class="preview">Project Coordinator: An out-of-the-box collaborator that monitors project status and follows up on overdue tasks automatically, without needing to configure an external agent.</span>

   <span class="preview">For more information, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).</span>
-->


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Seleccionar, Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema] <span class="preview">o Administrador del grupo</span></td> 
  </tr> 
  </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

* [Para revisores de IA](#for-ai-reviewers)
* [Para agentes de trabajo](#for-work-agents)

### Para revisores de IA:

* Su organización debe tener registrado un Contrato de IA de Adobe Gen firmado.

  Para obtener más información, consulte [Firmar el acuerdo de IA general de Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) en el artículo Asistente de IA en Workfront.
* Debe tener configurada una marca en Workfront para poder utilizarla para un revisor de IA.

  Para obtener instrucciones, consulte [Crear y administrar marcas para el revisor de IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Para utilizar Adobe Brand Intelligence como revisor de IA, su organización debe utilizar la experiencia de revisión y aprobación unificadas en Workfront.

  Para obtener más información, consulte [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

### Para agentes de trabajo

Debe configurar un agente en Claude, Copilot Studio, Writer, OpenAI o IBM antes de poder utilizarlo como agente de trabajo.

>[!NOTE]
>
>Nuestro objetivo es conectar con cualquier proveedor de agentes, de modo que si el proveedor que está utilizando no es compatible actualmente con los agentes de trabajo, póngase en contacto con el equipo de la cuenta para obtener ayuda.

## Crear nuevo revisor de IA

Los revisores de IA se pueden configurar para que utilicen marcas de Workfront o Adobe Brand Intelligence.

* **Marcas**: Las marcas se crean en Workfront. Puede crear marcas en Workfront cargando archivos de PDF que contengan las directrices de marca o introduciendo manualmente elementos de marca.
* **Adobe Brand Intelligence**: cuando un colaborador de IA revisa un recurso mediante Adobe Brand Intelligence, puede ver los comentarios realizados por el revisor de IA en Frame.io.


{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. Haga clic en **Nuevo colaborador** en la esquina superior derecha de la pantalla.
1. Haz clic en **Revisor** y luego haz clic en **Continuar**.
1. En el campo Nombre del colaborador, introduzca un nombre para el colaborador. Este es el nombre que aparece en la lista de usuarios asignados disponibles en una tarea.
1. Seleccione si el colaborador utilizará una marca o Adobe Brand Intelligence para sus críticas.
1. (Condicional) Si AI Collaborator va a utilizar una marca, seleccione la marca y las directrices de marca que utilizará.
1. Haga clic en **Guardar**.

## Configuración de un agente de trabajo

Los agentes de trabajo son agentes que se pueden asignar a tareas o problemas en Workfront. Configure el agente de trabajo con un nombre, un nivel de acceso y otros detalles, y asígnelo a una tarea como asignaría a un usuario.

Como los agentes de trabajo son agentes, sus acciones y capacidades se configuran donde se configuran los agentes. Actualmente, los agentes utilizados como agentes de trabajo se pueden crear en Copilot Studio, Claude o Writer, OpenAI y IBM.

Los agentes de trabajo se pueden asignar a tareas o problemas.

Para obtener una lista de prácticas recomendadas al crear un agente para trabajar como agente de trabajo, consulte [Prácticas recomendadas para crear un agente para un agente de trabajo](#best-practices-for-creating-an-agent-for-a-work-agent).

* [Configuración de un agente de trabajo en Workfront](#configure-a-work-agent-in-workfront)
* [Prácticas recomendadas para crear un agente para un agente de trabajo](#best-practices-for-creating-an-agent-for-a-work-agent)

### Configuración de un agente de trabajo en Workfront

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. Haga clic en **Nuevo colaborador** en la esquina superior derecha de la pantalla.
1. Seleccione **Agentes de trabajo** y haga clic en **Continuar**.
1. En el campo Nombre del colaborador de IA, introduzca un nombre para el colaborador. Este es el nombre que aparece en la lista de usuarios asignados disponibles en una tarea.
1. En el campo Descripción de AI Collaborator, introduzca una descripción del propósito del colaborador o de las acciones que realiza.
1. En el campo Nivel de acceso, seleccione un nivel de acceso para este colaborador. Este nivel de acceso controla lo que puede hacer el colaborador, del mismo modo que un nivel de acceso controla lo que un usuario puede hacer.
1. (Opcional) En el campo Grupos, seleccione los grupos a los que se asociará el agente de trabajo.

   >[!NOTE]
   >
   ><span class="preview">Si es administrador de un grupo, este campo solo muestra los grupos para los que es administrador. Los administradores de grupo deben seleccionar al menos un grupo.</span>

1. En el área **Elegir el origen del agente**, seleccione si desea conectar un agente creado en una plataforma común como Copilot o Writer, o utilizar un agente personalizado.
1. (Condicional) Si utiliza un agente de una plataforma común, introduzca los detalles de autenticación de la plataforma del agente:

   | Plataforma | Autenticación requerida |
   |---|---|
   | Copilot Studio | Secreto del canal web |
   | Agentes gestionados de Claude | Clave API antrópica<br>Id. de agente<br>Id. de entorno |
   | Agente de escritura | Clave de API <br>ID de aplicación |
   | <span class="preview">Agentes OpenAI</span> | <span class="preview">Clave de API <br>Id. de agente</span> |
   | <span class="preview">Orquestación Watsonx de IBM</span> | <span class="preview">URL de servicio<br>Clave de API<br> ID de agente</span> |

1. Haga clic en **Probar conexión**. Esto le permite saber si la conexión se ha configurado correctamente.
1. En el área **Después de que el colaborador finalice su trabajo, puede**, activar las acciones que desea que realice el colaborador.

   * <span class="preview">Enviar notificación: el agente hace un comentario en el flujo de actualización, etiquetando al usuario que solicitó el trabajo, asignó al agente o es propietario del proyecto. </span>
   * <span class="preview">Cargar un documento</span>
   * <span class="preview">Marcar tarea como completada</span>
   * Escribir campos de tarea: seleccione los formularios y campos en los que el agente puede escribir.

1. Haga clic en **Guardar**.

Para obtener más información sobre los agentes de trabajo, incluido cómo asignarlos a tareas, vea [Usar agentes de trabajo](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

### Prácticas recomendadas para crear un agente para un agente de trabajo

Puede encontrar útiles las siguientes prácticas recomendadas al crear un agente para utilizarlo como agente de trabajo en Workfront. Para ver las prácticas recomendadas, haga clic en la sección de la aplicación donde está creando el agente.

+++ Claude

1. Vaya a Claude Console en [platform.claude.com](https://platform.claude.com/).
1. Cree una clave de API.
   1. En Claves de API, haga clic en **Crear clave** en la esquina superior derecha.
   1. Proporcione un nombre y una fecha de caducidad.
   1. Copie la clave y guárdela en un lugar seguro. Necesitará esta clave para configurar el agente de trabajo en Workfront.

1. Cree un entorno.
   1. En **Agentes administrados** > **Entornos**, haga clic en **Crear entorno** en la esquina superior derecha.
   1. Proporcione un nombre y un tipo de alojamiento, según corresponda.
   1. Configure los paquetes compartidos y los metadatos según sea necesario. Los entornos se pueden reutilizar en varios agentes y permiten compartir paquetes y metadatos.
      El ID de entorno aparece debajo del nombre del entorno en la esquina superior izquierda.

1. Cree un agente.
   1. En Agentes administrados > Agentes, haga clic en **Crear agente** en la esquina superior derecha.
   1. Proporcione un nombre, modelo, mensaje del sistema, habilidades y herramientas según corresponda. Sea descriptivo, ya que los agentes de trabajo pasan el contexto de la tarea a este agente, que luego ejecuta el trabajo.
      El ID del agente aparece debajo del nombre del agente en la esquina superior izquierda.

1. Configure el agente de trabajo en Workfront.
   1. Introduzca su clave de API, ID de entorno e ID de agente
   1. Haga clic en **Probar conexión** para verificarla.

1. Asigne el agente de trabajo a una tarea de Workfront.
   1. El agente de trabajo se activa una vez completadas todas las tareas predecesoras.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Escritor

>[!NOTE]
>
> Puede utilizar un agente de Writer como agente de trabajo, pero los libros de reproducción de Writer no se pueden utilizar como agentes de trabajo.

Al crear un agente para utilizarlo como agente de trabajo en Writer, recomendamos el siguiente flujo de trabajo.

Encontrará información más detallada sobre la creación de agentes en la [documentación de Writer](https://dev.writer.com/no-code/introduction).

1. Cree una aplicación sin código en Writer AI Studio.
1. Añada un solo campo de entrada Text. Puede utilizar el nombre predeterminado &quot;Entrada de texto&quot;.
1. Agregue `@TextInput` al indicador. En la sección Indicadores de la configuración de la aplicación, asegúrese de que la plantilla de solicitud haga referencia a la variable de entrada. Sin esto, el modelo nunca ve los datos de tareas.
1. Ajuste el indicador para generar resultados inmediatamente. Elimine las instrucciones que pidan aclaraciones o contexto adicional al usuario antes de responder. Por ejemplo: &quot;Cuando reciba una entrada, trátela como una solicitud de generación de contenido y produzca la salida inmediatamente. No pidas una aclaración&quot;.
1. Copie la clave de API y el ID de aplicación. Los necesitará para configurar el agente de trabajo en Workfront.

   * Para obtener instrucciones sobre cómo configurar una clave de API en Writer, consulte [Quickstart](https://dev.writer.com/home/quickstart) en la documentación de Writer.
   * Para obtener instrucciones sobre cómo configurar un ID de aplicación en Writer, consulte [Invocar agentes sin código a través de la API](https://dev.writer.com/home/applications) en la documentación de Writer.

1. Configure el agente de trabajo en Workfront. Como parte de la configuración, ingresa tu clave de API y el identificador de la aplicación, luego haz clic en **Probar conexión** para verificarla.
1. Asigne el agente de trabajo a una tarea de Workfront. El agente de trabajo comienza a trabajar cuando se han completado todas las tareas predecesoras de la tarea.

+++

<div class="preview">

<!--
## Configure a Project Coordinator

The Project Coordinator is an out-of-the-box collaborator that monitors project status and helps keep work on track. Unlike Work Agents, the Project Coordinator does not require you to configure an external agent.

{{step-1-to-setup}}

1. In the left navigation, click **AI Collaborators**.
1. Click **New Collaborator** in the upper-right corner of the screen.
1. Select **Project Coordinator**.
1. In the **AI Collaborator name** field, enter a name for the Project Coordinator. This is the name that appears as the collaborator in your project.
1. In the **AI Collaborator description** field, enter a description of what the Project Coordinator does or its purpose.
1. In the **Access level** field, select an access level for the Project Coordinator. This access level controls what the collaborator can do on projects.
1. (Optional) In the **Send project updates** section, toggle **Allow** to enable project update notifications, then specify update details.
   * In the **Cadence** field, select whether the Coordinator sends updates daily or weekly.
   * If the Coordinator sends updates weekly, in the **Day of week** field, select the day of the week that updates are sent.
   * In the **Time (MST)** field, select the time to send updates.
   * In the **How to send** field, select whether the Coordinator sends updates as an update on the project, or as an email
   * In the **Who gets the update** field, select whether the update is sent only to the project owner, or to all project stakeholders.
   * (Optional) Check **Send additional update immediately when coordinator is assigned** to notify on assignment.
   * (Optional) Check **Send additional update when a date is missed** to send notifications when dates are missed.
1. (Optional) In the **Notify task assignees** section, toggle **Allow** to enable task notifications, then check the boxes for the situations that you want to notify assignees about.
1. (Optional) In the **Remind reviewers and approvers** section, toggle **Allow** to enable reminders for reviewers, then check the boxes for the situations that you want to remind reviewers and approvers about.
1. (Optional) In the **Update the content of project and task fields** section, toggle **Allow** to enable the coordinator to update project and task field values.
1. Click **Save**.

For more information on the Project Coordinator, including how to assign it to projects, see [Use the Project Coordinator collaborator](/help/quicksilver/manage-work/projects/manage-projects/use-project-coordinator.md).
-->

</div>

## Administrar colaboradores de IA

Puede editar, copiar y eliminar colaboradores de IA existentes.

>[!NOTE]
>
><span class="preview">Los administradores de grupo solo pueden ver e interactuar con los colaboradores de IA asociados con los grupos para los que son administradores. Si otros grupos también están asociados a un colaborador de IA determinado, un administrador de grupo puede verlo, pero no editarlo.</span>

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. (Condicional) Para editar un Collaborator, haga clic en el nombre del Collaborator que desee editar, realice las modificaciones que desee en la ventana Editar Collaborator y haga clic en **Guardar**.
1. (Condicional) Para eliminar un Collaborator, haga clic en el icono Eliminar ![Icono Eliminar](assets/delete-collaborator-icon.png) en la fila del AI Collaborator que desee eliminar y, a continuación, haga clic en **Eliminar**.
