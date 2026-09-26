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
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 3%
---
# Configuración de colaboradores de IA

Los colaboradores de IA son una forma de incorporar agentes de IA en sus proyectos y tareas. Puede configurar un colaborador de IA y, a continuación, asignarlo como lo haría con un usuario.

Por ejemplo, puede configurar un colaborador de IA de tipo revisor con directrices de marca y, a continuación, asignar ese colaborador para que revise un documento.

Los tipos de AI Collaborator disponibles incluyen:

* Revisor de IA: cree un colaborador con marcas o Adobe Brand Intelligence y, a continuación, asígnelo como revisor en los recursos.

  Para obtener más información, consulte [Introducción al Revisor de IA de Workfront](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

* Agente de trabajo: cree un colaborador mediante Copiloto o Escritor y, a continuación, asigne el colaborador a una tarea para completar el trabajo de nivel de tarea.

  Para obtener más información, vea [Usar agentes de trabajo](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md).


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
* Debe tener configurada una marca en Workfront para poder utilizarla para un revisor de IA.

  Para obtener instrucciones, consulte [Crear y administrar marcas para el revisor de IA](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).
* Para utilizar Adobe Brand Intelligence como revisor de IA, su organización debe utilizar la experiencia de revisión y aprobación unificadas en Workfront.

  Para obtener más información, consulte [Introducción a la revisión y aprobación unificadas](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

### Para agentes de trabajo

Debe configurar un agente en Claude, Copilot Studio o Writer antes de poder utilizarlo como agente de trabajo.

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

Los agentes de trabajo son agentes que puede asignar a tareas en Workfront. Configure el agente de trabajo con un nombre, un nivel de acceso y otros detalles, y asígnelo a una tarea como asignaría a un usuario.

Como los agentes de trabajo son agentes, sus acciones y capacidades se configuran donde se configuran los agentes. Actualmente, los agentes utilizados como agentes de trabajo pueden crearse en Copilot Studio, Claude o Writer.

Los agentes de trabajo solo se pueden asignar a tareas y, actualmente, no se pueden asignar a problemas.

Para obtener una lista de prácticas recomendadas al crear un agente para trabajar como agente de trabajo, consulte [Prácticas recomendadas para crear un agente para un agente de trabajo](#best-practices-for-creating-an-agent-for-a-work-agent).

### Configuración de un agente de trabajo en Workfront

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. Haga clic en **Nuevo colaborador** en la esquina superior derecha de la pantalla.
1. Seleccione **Agentes de trabajo** y haga clic en **Continuar**.
1. En el campo Nombre del colaborador de IA, introduzca un nombre para el colaborador. Este es el nombre que aparece en la lista de usuarios asignados disponibles en una tarea.
1. En el campo Descripción de AI Collaborator, introduzca una descripción del propósito del colaborador o de las acciones que realiza.
1. En el campo Nivel de acceso, seleccione un nivel de acceso para este colaborador. Este nivel de acceso controla lo que puede hacer el colaborador, del mismo modo que un nivel de acceso controla lo que un usuario puede hacer.
1. En el área **Elegir el origen del agente**, seleccione si desea conectar un agente creado en una plataforma común como Copilot o Writer, o utilizar un agente personalizado.
1. (Condicional) Si utiliza un agente de una plataforma común, introduzca los detalles de autenticación de la plataforma del agente:

   | Plataforma | Autenticación requerida |
   |---|---|
   | Copilot Studio | Secreto del canal web |
   | Agentes gestionados de Claude | Clave API antrópica<br>Id. de agente<br>Id. de entorno |
   | Escritor | Clave de API <br>ID de aplicación |

1. Haga clic en **Probar conexión**. Esto le permite saber si la conexión se ha configurado correctamente.
1. En el área **Después de que el colaborador finalice su trabajo, puede**, activar las acciones que desea que realice el colaborador.
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

## Administrar colaboradores de IA

Puede editar, copiar y eliminar colaboradores de IA existentes.

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Colaboradores de IA**.
1. (Condicional) Para editar un Collaborator, haga clic en el nombre del Collaborator que desee editar, realice las modificaciones que desee en la ventana Editar Collaborator y haga clic en **Guardar**.
1. (Condicional) Para eliminar un Collaborator, haga clic en el icono Eliminar ![Icono Eliminar](assets/delete-collaborator-icon.png) en la fila del AI Collaborator que desee eliminar y, a continuación, haga clic en **Eliminar**.
