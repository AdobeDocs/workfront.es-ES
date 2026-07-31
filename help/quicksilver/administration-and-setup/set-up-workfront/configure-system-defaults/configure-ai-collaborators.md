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
source-git-commit: dc6bfcd7d3431532c1227f6cd31f22445882143f
workflow-type: tm+mt
source-wordcount: '1344'
ht-degree: 4%

---

# Configuración de colaboradores de IA


<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>


Los colaboradores de IA son una forma de incorporar agentes de IA en sus proyectos y tareas. Puede configurar un colaborador de IA y, a continuación, asignarlo como lo haría con un usuario.

Por ejemplo, puede configurar un colaborador de IA de tipo revisor con directrices de marca y, a continuación, asignar ese colaborador para que revise un documento.

Los tipos de AI Collaborator disponibles incluyen:

* Revisor: cree un colaborador con marcas o Adobe Brand Intelligence y, a continuación, asígnelo como revisor en los recursos.

  Para obtener más información, consulte [Introducción al Revisor de contenido de Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Colaborador de tareas: cree un colaborador con Copilot o Writer y, a continuación, asigne el colaborador a una tarea para completar el trabajo de nivel de tarea.

  Para obtener más información, consulte [Usar colaboradores de tareas](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Standard, Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

### Para revisores de IA:

* Su organización debe tener registrado un Contrato de IA de Adobe Gen firmado.

  Para obtener más información, consulte [Firmar el acuerdo de IA general de Adobe](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) en el artículo Asistente de IA en Workfront.
* Debe tener configurada una marca en Workfront para poder utilizarla en un colaborador de IA de tipo revisor.

  Para obtener instrucciones, consulte [Crear y administrar marcas para el revisor de contenido](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Para utilizar Adobe Brand Intelligence for a Reviewer AI Collaborator, su organización debe utilizar la experiencia unificada de revisión y aprobación en Workfront. </span>

  Para obtener más información, vea [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md). </span>

<div class="preview">

### Para colaboradores de tareas

Debe configurar un agente en Claude, Copilot Studio o Writer antes de poder utilizarlo como colaborador de tareas.

</div>

## Crear un nuevo colaborador de IA de tipo revisor

Los colaboradores de IA del revisor se pueden configurar para que utilicen marcas de Workfront o Adobe Brand Intelligence.

* **Marcas**: Las marcas se crean en Workfront. Puede crear marcas en Workfront cargando archivos de PDF que contengan las directrices de marca o introduciendo manualmente elementos de marca.
* **Adobe Brand Intelligence**: cuando un colaborador de IA revisa un recurso mediante Adobe Brand Intelligence, puede ver los comentarios realizados por el revisor en Frame.io.  </span>


{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. Haga clic en **Nuevo colaborador** en la esquina superior derecha de la pantalla.
1. Haz clic en **Revisor** y luego haz clic en **Continuar**.
1. En el campo Nombre del colaborador, introduzca un nombre para el colaborador. Este es el nombre que aparece en la lista de usuarios asignados disponibles en una tarea.
1. Seleccione si el colaborador utilizará una marca o Adobe Brand Intelligence para sus revisiones.
1. (Condicional) Si AI Collaborator va a utilizar una marca, seleccione la marca y las directrices de marca que utilizará.
1. Haga clic en **Guardar**.

<div class="preview">

## Configurar un colaborador de tareas

Los colaboradores de tareas son agentes de MCP que puede asignar a tareas en Workfront. Puede configurar el colaborador de tareas con un nombre, un nivel de acceso y otros detalles, y asignarlo de la misma manera que asignaría a un usuario.

Debido a que los colaboradores de tareas son agentes de MCP, sus acciones y capacidades se configuran allí donde configure los agentes. Actualmente, los agentes utilizados como colaboradores de tareas pueden crearse en Copilot Studio, Claude o Writer.

Para obtener una lista de prácticas recomendadas al crear un agente para que funcione como colaborador de tareas, consulte [Prácticas recomendadas para crear un agente para un colaborador de tareas](#best-practices-for-creating-an-agent-for-a-task-collaborator).

### Configuración de un colaborador de tareas en Workfront

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. Haga clic en **Nuevo colaborador** en la esquina superior derecha de la pantalla.
1. Seleccione **Agentes de tareas** y haga clic en **Continuar**.
1. En el campo Nombre del colaborador de IA, introduzca un nombre para el colaborador. Este es el nombre que aparece en la lista de usuarios asignados disponibles en una tarea.
1. En el campo Descripción de AI Collaborator, introduzca una descripción del propósito del colaborador o de las acciones que realiza.
1. En el campo Nivel de acceso, seleccione un nivel de acceso para este colaborador. Este nivel de acceso controla lo que puede hacer el colaborador, del mismo modo que un nivel de acceso controla lo que un usuario puede hacer.
1. En el área **Elegir el origen del agente**, seleccione si desea conectar un agente creado en una plataforma común como Copilot o Writer, o utilizar un agente personalizado.
1. (Condicional) Si utiliza un agente de una plataforma común, introduzca los detalles de autenticación de la plataforma del agente:

   | Plataforma | Autenticación requerida |
   |---|---|
   | Copilot Studio | Secreto del canal web |
   | Claude Managed Agents | Clave API antrópica<br>Id. de agente<br>Id. de entorno |
   | Escritor | Clave de API <br>ID de aplicación |

1. Haga clic en **Probar conexión**. Esto le permite saber si la conexión se ha configurado correctamente.
1. En el área **Después de que el colaborador finalice su trabajo, puede**, activar las acciones que desea que realice el colaborador.
1. Haga clic en **Guardar**.

Para obtener más información sobre los colaboradores de tareas, incluido cómo asignarlos a tareas, consulte [Usar colaboradores de tareas](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


### Prácticas recomendadas para crear un agente para un colaborador de tareas

Puede encontrar útiles las siguientes prácticas recomendadas al crear un agente para utilizarlo como colaborador de tareas en Workfront. Para ver las prácticas recomendadas, haga clic en la sección de la aplicación donde está creando el agente.

+++ Claude

1. Vaya a Claude Console en [platform.claude.com](https://platform.claude.com/).
1. Cree una clave de API.
   1. En Claves de API, haga clic en **Crear clave** en la esquina superior derecha.
   1. Proporcione un nombre y una fecha de caducidad.
   1. Copie la clave y guárdela en un lugar seguro. Necesitará esta clave para configurar Task Collaborator en Workfront.

1. Cree un entorno.
   1. En **Agentes administrados** > **Entornos**, haga clic en **Crear entorno** en la esquina superior derecha.
   1. Proporcione un nombre y un tipo de alojamiento, según corresponda.
   1. Configure los paquetes compartidos y los metadatos según sea necesario. Los entornos se pueden reutilizar en varios agentes y permiten compartir paquetes y metadatos.
      El ID de entorno aparece debajo del nombre del entorno en la esquina superior izquierda.

1. Cree un agente.
   1. En Agentes administrados > Agentes, haga clic en **Crear agente** en la esquina superior derecha.
   1. Proporcione un nombre, modelo, mensaje del sistema, habilidades y herramientas según corresponda. Sea descriptivo, ya que los colaboradores de tareas pasan el contexto de las tareas a este agente, que luego ejecuta el trabajo.
      El ID del agente aparece debajo del nombre del agente en la esquina superior izquierda.

1. Configure Task Collaborator en Workfront.
   1. Introduzca su clave de API, ID de entorno e ID de agente
   1. Haga clic en **Probar conexión** para verificarla.

1. Asigne el Task Collaborator a una tarea de Workfront.
   1. Task Collaborator se activa una vez completadas todas las tareas predecesoras.

+++
<!--
+++ Copilot Studio



+++
-->
+++ Escritor

Al crear un agente para utilizarlo como colaborador de tareas en Writer, recomendamos el siguiente flujo de trabajo.

Encontrará información más detallada sobre la creación de agentes en la [documentación de Writer](https://dev.writer.com/no-code/introduction).

1. Cree una aplicación sin código en Writer AI Studio.
1. Añada un solo campo de entrada Text. Puede utilizar el nombre predeterminado &quot;Entrada de texto&quot;.
1. Agregue `@TextInput` al indicador. En la sección Indicadores de la configuración de la aplicación, asegúrese de que la plantilla de solicitud haga referencia a la variable de entrada. Sin esto, el modelo nunca ve los datos de tareas.
1. Ajuste el indicador para generar resultados inmediatamente. Elimine las instrucciones que pidan aclaraciones o contexto adicional al usuario antes de responder. Por ejemplo: &quot;Cuando reciba una entrada, trátela como una solicitud de generación de contenido y produzca la salida inmediatamente. No pidas una aclaración&quot;.
1. Copie la clave de API y el ID de aplicación. Necesitará Task Collaborator para configurar Task Collaborator en Workfront.

   * Para obtener instrucciones sobre cómo configurar una clave de API en Writer, consulte [Quickstart](https://dev.writer.com/home/quickstart) en la documentación de Writer.
   * Para obtener instrucciones sobre cómo configurar un ID de aplicación en Writer, consulte [Invocar agentes sin código a través de la API](https://dev.writer.com/home/applications) en la documentación de Writer.

1. Configure Task Collaborator en Workfront. Como parte de la configuración, ingresa tu clave de API y el identificador de la aplicación, luego haz clic en **Probar conexión** para verificarla.
1. Asigne el Task Collaborator a una tarea de Workfront. El colaborador comienza a trabajar cuando se han completado todas las tareas predecesoras de la tarea.

+++

</div>

## Administrar colaboradores de IA

Puede editar, copiar y eliminar colaboradores de IA existentes.

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. (Condicional) Para editar un Collaborator, haga clic en el nombre del Collaborator que desee editar, realice las modificaciones que desee en la ventana Editar Collaborator y haga clic en **Guardar**.
1. (Condicional) Para copiar un Collaborator, haga clic en el icono Copiar ![Icono Copiar](assets/copy-ai-collaborator.png) en la fila del AI Collaborator que desee copiar, haga clic en el nombre de la copia, realice las modificaciones que desee en la ventana Editar Collaborator y haga clic en **Guardar**.
1. (Condicional) Para eliminar un Collaborator, haga clic en el icono Eliminar ![Icono Eliminar](assets/delete-collaborator-icon.png) en la fila del AI Collaborator que desee eliminar y, a continuación, haga clic en **Eliminar**.
