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
source-git-commit: 331746b2e3f0a5ce6cd0bb01e020d787d6ad951b
workflow-type: tm+mt
source-wordcount: '1564'
ht-degree: 4%
---
# Configuración de colaboradores de IA

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes.</span>

Los colaboradores de IA son una forma de incorporar agentes de IA en sus proyectos, tareas y problemas. Puede configurar un colaborador de IA y, a continuación, asignarlo como lo haría con un usuario.

Por ejemplo, puede configurar un colaborador de IA de tipo revisor con directrices de marca y, a continuación, asignar ese colaborador para que revise un documento.

Los tipos de AI Collaborator disponibles incluyen:

* Revisor de IA: cree un colaborador con marcas o Adobe Brand Intelligence y, a continuación, asígnelo como revisor en los recursos.

  Para obtener más información, consulte [Introducción al Revisor de IA de Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Agente de trabajo: cree un colaborador <span class="preview">con tecnología de Adobe CX Coworker,</span> o conecte un agente desde una plataforma externa admitida y, a continuación, asigne al colaborador a una tarea o problema para completar los elementos de trabajo.

  Para obtener más información, vea [Usar agentes de trabajo](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).

  Para obtener más información sobre Adobe CX Enterprise Coworker, consulte [Información general sobre CX Enterprise Coworker en Workfront](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md).

<!-- BECKY CHECK ME: Why this changed: we updated the Work Agent description to include Adobe Native and need product confirmation on any additional package, license, agreement, credit, or administrator restrictions before publishing. -->

Las licencias utilizadas por los colaboradores de IA no se facturan. Si su organización tiene 200 licencias de Workfront y crea un colaborador de IA, se utilizan 201 licencias, pero solo se facturan 200.

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
   <td>[!UICONTROL Administrador del sistema] o Administrador de grupo</span></td> 
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

<span class="preview">Los requisitos previos dependen del origen del agente:</span>

* <span class="preview">Adobe nativo: su organización debe tener Adobe CX Coworker habilitado. No es necesario configurar un agente en una plataforma externa ni proporcionar credenciales de plataforma externa.</span>
* Plataforma externa o agente personalizado: configure el agente en la plataforma a la que planea conectarse antes de crear el agente de trabajo en Workfront.

>[!NOTE]
>
>Nuestro objetivo es conectar con cualquier proveedor de agentes, de modo que si el proveedor que está utilizando no es compatible actualmente con los agentes de trabajo, póngase en contacto con el equipo de la cuenta para obtener ayuda.

<!-- BECKY CHECK ME: Why this changed: we separated Native and external-agent prerequisites to match the draft, and we still need product confirmation on the final setup and entitlement requirements before removing the qualifiers. -->

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

<span class="preview">Las siguientes instrucciones de configuración reflejan la compatibilidad nativa de Adobe y el modelo de configuración basado en el origen que aún se encuentra en la vista previa.</span>

Los agentes de trabajo son agentes que se pueden asignar a tareas o problemas en Workfront. Configure el agente de trabajo con un nombre, un nivel de acceso y otros detalles, y asígnelo a una tarea como asignaría a un usuario.

Como los agentes de trabajo son agentes, sus acciones y capacidades se configuran donde se configuran los agentes. Los agentes de trabajo pueden ser <span class="preview">agentes de trabajo nativos que usen Coworker</span> o pueden provenir de una plataforma externa compatible, como Copilot Studio, Claude, OpenAI y IBM.

>Los agentes de trabajo se pueden asignar a tareas o problemas.

<!-- BECKY CHECK ME: Why this changed: we broadened the origin language to include Adobe Native and want product confirmation on whether the release should describe it as a ready-to-use origin and whether the external-agent setup language still matches production. -->

Las licencias utilizadas por los agentes de trabajo no se facturan. Si su organización tiene 200 licencias de Workfront y crea un agente de trabajo, se utilizan 201 licencias, pero solo se facturan 200.

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
   >Si es administrador de un grupo, este campo sólo muestra los grupos para los que es administrador. Los administradores de grupo deben seleccionar al menos un grupo.

1. En el área **Elegir el origen del agente**, seleccione si desea <span class="preview">usar Adobe Native</span>, conectar un agente creado en una plataforma común como Copilot o usar un agente personalizado.
1. <span class="preview">(Condicional) Si selecciona Adobe Native, confirme que Adobe CX Coworker está habilitado para su organización y que desea utilizar el agente nativo de Adobe listo para usar.</span>
1. (Condicional) Si utiliza un agente de una plataforma común, introduzca los detalles de autenticación de la plataforma del agente:

   | Plataforma | Autenticación requerida |
   |---|---|
   | Copilot Studio | Secreto del canal web |
   | Agentes gestionados de Claude | Clave API antrópica<br>Id. de agente<br>Id. de entorno |
   | Agentes OpenAI | Clave de API <br>ID de agente |
   | IBM watsonx Orchestrate | URL del servicio<br>Clave de API<br> ID del agente |

1. Haga clic en **Probar conexión**. Esto le permite saber si la conexión se ha configurado correctamente.
1. En el área **Después de que el colaborador finalice su trabajo, puede**, activar las acciones que desea que realice el colaborador.

   * Enviar notificación: el agente realiza un comentario en el flujo de actualización, etiquetando al usuario que solicitó el trabajo, asignó al agente o es propietario del proyecto.
   * Cargar documentos basados en texto
   * Marcar tarea como completada
   * Escribir campos de tarea: seleccione los formularios y campos en los que el agente puede escribir.
   * Escribir campos de proyecto: seleccione los formularios y campos en los que el agente puede escribir.

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



>[!IMPORTANT]
>
>El escritor ha desaprobado el uso de agentes. Los agentes de trabajo configurados con agentes de Writer ya no funcionan después del 9 de octubre. 2026.
>
>Para obtener más información sobre la obsolescencia, consulte [Migración y obsolescencia de la biblioteca del agente](https://support.writer.com/articles/8335689949-migrating-no-code-agents) en la documentación de Writer.


<!--

>[!NOTE]
>
> You can use a Writer agent as a Work Agent, but Writer playbooks cannot be used as Work Agents.

When creating an agent for use as a Work Agent in Writer, we recommend the following workflow.

More detailed information about creating agents can be found in the [Writer documentation](https://dev.writer.com/no-code/introduction).

1. Create a no-code app in Writer AI Studio. 
1. Add a single Text input field. You can use the default name "Text input."
1. Add `@TextInput` to your Prompt. In the Prompts section of your app configuration, make sure your prompt template references the input variable. Without this, the model never sees the task data.
1. Adjust your Prompt to generate output immediately. Remove any instructions that ask the user for clarification or additional context before responding. For example: "When you receive input, treat it as a content generation request and produce the output immediately. Do not ask for clarification."
1. Copy your API key and Application ID. You will need them to configure the Work Agent in Workfront.

   * For instructions on setting up an API key in Writer, see [Quickstart](https://dev.writer.com/home/quickstart) in the Writer documentation.
   * For instructions on setting up an application ID in Writer, see [Invoke no-code agents via the API](https://dev.writer.com/home/applications) in the Writer documentation.
 
1. Configure the Work Agent in Workfront. As part of the configuration, enter your API key and Application ID, then click **Test connection** to verify.
1. Assign the Work Agent to a Workfront task. The Work Agent begins work when all of the task's predecessor tasks are complete.

-->

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
>Los administradores de grupos solo pueden ver e interactuar con los colaboradores de IA asociados con los grupos para los que son administradores. Si otros grupos también están asociados a un colaborador de IA determinado, un administrador de grupo puede verlo, pero no editarlo.

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. (Condicional) Para editar un Collaborator, haga clic en el nombre del Collaborator que desee editar, realice las modificaciones que desee en la ventana Editar Collaborator y haga clic en **Guardar**.
1. (Condicional) Para eliminar un Collaborator, haga clic en el icono Eliminar ![Icono Eliminar](assets/delete-collaborator-icon.png) en la fila del AI Collaborator que desee eliminar y, a continuación, haga clic en **Eliminar**.
