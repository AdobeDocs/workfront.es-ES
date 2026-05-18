---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Uso del servidor MCP de Adobe Workfront
description: Utilice el servidor MCP de Adobe Workfront para buscar, crear, actualizar y administrar elementos de Workfront mediante una conversación en lenguaje natural en un asistente de IA.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 2%

---


# Uso del servidor MCP de Adobe Workfront

El servidor MCP [!DNL Adobe Workfront] le permite buscar, crear, actualizar y administrar elementos de Workfront preguntando a un asistente de IA en inglés sin formato. El asistente de IA decide qué acciones de Workfront llamar y gestiona la conversación con Workfront por usted.

[!DNL Claude] es actualmente el único asistente de IA compatible, pero los ejemplos y patrones de este artículo se aplican a cualquier asistente de IA que admita el servidor MCP de Workfront.

Este artículo supone que ya ha configurado la conexión. Para obtener información sobre la instalación, consulte [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Para obtener más información sobre el servidor MCP de Workfront, consulte [Descripción general del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).



## Acciones disponibles a través del servidor MCP de Workfront

El servidor MCP de Workfront cubre las acciones entre aprobaciones, planificación y flujo de trabajo.

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>Un asistente de IA actúa en Workfront con su cuenta y permisos de Workfront. Usted y su proveedor de asistente de IA son responsables de las acciones que realiza el asistente de IA en su nombre. Confirme lo que el asistente de IA está a punto de hacer antes de dejarlo continuar.


## Responsabilidad de las acciones del asistente de IA

Al conectar un asistente de IA a Workfront, el asistente de IA actúa en Workfront con la cuenta y los permisos de Workfront. Las acciones del asistente de IA tienen el mismo efecto que las acciones que realiza directamente en la interfaz de Workfront.

Usted y el proveedor del asistente de IA son responsables de las acciones que realiza el asistente de IA en Workfront. Adobe no se responsabiliza por los cambios que el asistente de IA realice en los datos de Workfront.

Antes de dejar que el asistente de IA continúe con una solicitud, confirme que comprende lo que pretende hacer, especialmente para las acciones que cambian o eliminan datos.

### Acciones principales

El servidor MCP de Workfront incluye las siguientes acciones principales:

| Acción | Qué hace |
|---|---|
| Crear | Crea nuevos elementos en Workfront. |
| Buscar | Busca y recupera elementos de Workfront. |
| Actualizar | Cambia los elementos existentes en Workfront. |
| Eliminar | Quita elementos de Workfront. |
| Resolver nombres de campo | Busca los nombres de campo de Workfront correctos para que el asistente de IA pueda crear solicitudes precisas con los datos. |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### Acciones de aprobaciones

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### Planificación de acciones

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### Acciones de flujo de trabajo

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## Ejemplos de qué preguntar

Una vez que esté conectado, escriba solicitudes en lenguaje natural en su asistente de IA. El asistente de IA decide qué acciones de Workfront llamar y devuelve los resultados.

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### Buscar y ver su trabajo

Solicite al asistente de IA que busque en Workfront elementos que coincidan con lo que está buscando. Por ejemplo:

* *Mostrarme todos los proyectos activos del equipo de marketing de marca.*
* *Asignarme todas las tareas asignadas a Joan Harris.*
* *Mostrarme todos los problemas en el proyecto &quot;Rediseño del sitio web&quot; en la categoría &quot;Técnico&quot;.*

### Crear nuevos elementos

Solicite al asistente de IA que cree proyectos, tareas u otros elementos de Workfront. Por ejemplo:

* *Cree un proyecto en blanco llamado &quot;Espacio aislado para innovación en el segundo trimestre&quot; a partir del 10 de marzo y hasta el 30 de abril. Definirme como propietario.*
* *Agregue una nueva tarea denominada &quot;Control de calidad de la página de aterrizaje&quot; al proyecto y programe su ejecución del 22 al 26 de abril.*
* *Cree un nuevo registro de campaña denominado &quot;Rebajas de verano de 2026&quot;.*

### Actualizar elementos existentes

Solicite al asistente de IA que realice cambios en los elementos que ya se encuentran en Workfront. Por ejemplo:

* *Actualice la tarea &quot;Revisión de diseño&quot; para que finalice el 18 de abril y asígnela al equipo creativo.*
* *Para el proyecto &quot;Lucent AI Launch - NA&quot;, finalice hasta mediados de abril y aumente el presupuesto a 150.000 dólares.*
* *Actualice el campo de presupuesto en el registro &quot;Campaña de verano&quot; a $75,000.*

### Eliminar elementos

Solicite al asistente de IA que elimine los elementos de Workfront. Por ejemplo:

* *Elimine el proyecto denominado &quot;Campaña de prueba del primer trimestre&quot;.*
* *Quite la tarea &quot;Imprimir producción de recursos&quot; del proyecto.*
* *Elimine el registro de campaña denominado &quot;Promoción antigua&quot;.*

>[!WARNING]
>
>Eliminar elementos en Workfront mediante un asistente de IA es lo mismo que eliminarlos en la interfaz de Workfront. Confirme lo que el asistente de IA está a punto de eliminar antes de dejarlo continuar.

### Trabajo con aprobaciones

Solicite al asistente de IA que administre las aprobaciones de documentos y recursos. Por ejemplo:

* *Agregue a Sarah Chen y Miguel Álvarez como aprobadores en el documento actual.*
* *Envíe un recordatorio a los aprobadores del recurso &quot;Vídeo de campaña de primavera&quot; que no hayan respondido.*
* *Aplique la plantilla de aprobación &quot;Lanzamiento de marketing&quot; al recurso &quot;Vídeo de campaña de primavera&quot;.*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### Trabajo con registros de Planning

Solicite al asistente de IA que administre los registros de planificación. Por ejemplo:

* *Cree un nuevo registro de planificación denominado &quot;Plan de marketing del segundo trimestre&quot; para el equipo de marketing de marca.*
* *Agregue una nueva tarea denominada &quot;Auditoría de medios sociales&quot; al registro de planificación.*
* *Actualice la tarea &quot;Auditoría de medios sociales&quot; para que finalice el 18 de abril y asígnela al equipo creativo.*

### Trabajo con flujo de trabajo

Solicite al asistente de IA que administre el flujo de trabajo. Por ejemplo:

* *Enrute el proyecto &quot;Espacio aislado para la innovación en el segundo trimestre&quot; al Consejo de revisión de la innovación.*
* *Actualice el registro &quot;Campaña de verano&quot; al estado &quot;Listo para el lanzamiento&quot;.*
* *Aprobar el registro &quot;Campaña de verano&quot;.*


### Encadenar solicitudes en una conversación

Puede encadenar solicitudes en una sola conversación. El asistente de IA mantiene el contexto, por lo que cada solicitud puede basarse en la anterior. Por ejemplo:

1. Pida al asistente de IA que busque un conjunto de elementos: *Buscar mis tareas vencidas.*
1. Una vez que el asistente de IA devuelva la lista, pídale que actúe en función de los resultados: *Actualice todos a viernes siguiente.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Consideraciones

Tenga en cuenta las siguientes consideraciones al utilizar el servidor MCP de Workfront.

### El asistente de IA puede utilizar información de una fase anterior de la conversación

Los asistentes de IA a veces reutilizan los datos de versiones anteriores de una conversación en lugar de solicitar a Workfront la última versión. Si algo ha cambiado en Workfront desde la última vez que el asistente de IA miró, es posible que vea información obsoleta.

Para obligar al asistente de IA a recuperar datos nuevos, pídale explícitamente. Por ejemplo:

* *Obtenga los datos más recientes de Workfront. No usar resultados en caché.*

### El servidor MCP de Workfront se actualiza automáticamente

Cuando Adobe publica una nueva versión del servidor MCP de Workfront, su asistente de IA utiliza la nueva versión automáticamente. No es necesario que vuelva a conectarse o cambie nada de su lado.

## Datos y seguridad

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Qué datos salen de Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Cómo administran los proveedores de asistentes de IA los datos de Workfront

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Diferencias entre asistentes de IA

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## Solución de problemas del uso diario

Para obtener más información acerca de los problemas de configuración y autenticación, consulte [Solucionar problemas de configuración y autenticación](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) en [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

| Problema | Causa probable | Corregir |
|---|---|---|
| El asistente de IA le está dando información obsoleta. | El asistente de IA está reutilizando datos de versiones anteriores de la conversación. | Solicite al asistente de IA que recupere datos nuevos de Workfront. |
| El asistente de IA devolvió datos de elementos de Workfront incorrectos. | El asistente de IA eligió los elementos equivocados basándose en una redacción ambigua. | Vuelva a preguntar con nombres, ID o filtros más específicos. |
| Una actualización o eliminación no surtió efecto en Workfront. | El asistente de IA aún no ha llamado a la acción o sus permisos no la permiten. | Confirme con el asistente de IA que la acción se ha ejecutado y, a continuación, compruebe sus permisos de Workfront. |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## Preguntas frecuentes

### ¿Con qué elementos de Workfront puedo trabajar mediante un asistente de IA?

Cualquier elemento al que tenga acceso en Workfront mediante niveles de acceso y permisos de objeto.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### ¿Mis datos de Workfront se envían al proveedor del asistente de IA o se almacenan en él?

Para obtener más información, consulte [Datos y seguridad](#data-and-security) en este artículo.

### ¿Qué sucede cuando se publica una nueva versión del servidor MCP de Workfront?

El servidor MCP se actualiza automáticamente. No es necesario que vuelva a conectarse o cambie nada.

### ¿Necesito saber la API de Workfront para utilizar el servidor MCP de Workfront?

No. El asistente de IA traduce las solicitudes en lenguaje natural a las acciones correctas de Workfront. Si ya está familiarizado con la API de Workfront, las acciones le resultarán familiares, pero no es un requisito.
