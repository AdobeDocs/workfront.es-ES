---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Uso del servidor MCP de Adobe Workfront
description: Utilice el servidor MCP de Adobe Workfront para buscar, crear, actualizar y administrar elementos de Workfront a través de una conversación en lenguaje natural en una plataforma agéntica de IA.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 0%

---


# Uso del servidor MCP de Adobe Workfront

El servidor MCP [!DNL Adobe Workfront] le permite buscar, crear, actualizar y administrar elementos de Workfront solicitando una plataforma auténtica de IA en inglés sin formato. La plataforma decide qué acciones de Workfront llamar y gestiona la conversación con Workfront por usted.

[!DNL Claude] es actualmente la única plataforma agéntica de IA compatible, pero los ejemplos y patrones de este artículo se aplican a cualquier plataforma agéntica de IA que admita el servidor MCP de Workfront.

Este artículo supone que ya ha configurado la conexión. Para obtener información sobre la instalación, consulte [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Para obtener más información sobre el servidor MCP de Workfront, consulte [Descripción general del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Herramientas disponibles

El servidor MCP de Workfront expone un conjunto de herramientas que la plataforma agéntica de IA llama en su nombre, por ejemplo, herramientas para buscar Workfront, crear elementos, actualizar campos y administrar aprobaciones. Para obtener la lista de referencia completa, agrupada por área de Workfront, consulte [Herramientas de servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Cuando conecta una plataforma independiente de IA a Workfront, esta actúa en Workfront con su cuenta y permisos de Workfront. Las acciones de la plataforma tienen el mismo efecto que las acciones que realiza directamente en la interfaz de Workfront.
>
>Usted y su proveedor de plataformas agénticas de IA son responsables de las acciones que realiza la plataforma en Workfront. Adobe no se responsabiliza por los cambios que realice la plataforma agéntica de IA en sus datos de Workfront.
>
>Antes de dejar que la plataforma agéntica de IA continúe con una solicitud, confirme que comprende lo que pretende hacer, especialmente para las acciones que cambian o eliminan datos.


## Ejemplos de qué preguntar

Una vez que esté conectado, escriba solicitudes en lenguaje natural en la plataforma agéntica de IA. La plataforma agéntica de IA decide qué acciones de Workfront llamar y devuelve los resultados.

### Buscar y ver su trabajo

Para buscar en Workfront elementos que coincidan con lo que está buscando, pregunte:

* *Mostrarme todos los proyectos activos del equipo de marketing de marca.*
* *Asignarme todas las tareas asignadas a Joan Harris.*
* *Mostrarme todos los problemas en el proyecto &quot;Rediseño del sitio web&quot; en la categoría &quot;Técnico&quot;.*

### Crear nuevos elementos

Para crear proyectos, tareas u otros elementos de Workfront, haga lo siguiente:

* *Cree un proyecto en blanco llamado &quot;Espacio aislado para innovación en el segundo trimestre&quot; a partir del 10 de marzo y hasta el 30 de abril. Definirme como propietario.*
* *Agregue una nueva tarea denominada &quot;Control de calidad de la página de aterrizaje&quot; al proyecto y programe su ejecución del 22 al 26 de abril.*
* *Cree un nuevo registro de campaña denominado &quot;Rebajas de verano de 2026&quot;.*

### Actualizar elementos existentes

Para realizar cambios en elementos que ya están en Workfront, haga lo siguiente:

* *Actualice la tarea &quot;Revisión de diseño&quot; para que finalice el 18 de abril y asígnela al equipo creativo.*
* *Para el proyecto &quot;Lucent AI Launch - NA&quot;, finalice hasta mediados de abril y aumente el presupuesto a 150.000 dólares.*
* *Actualice el campo de presupuesto en el registro &quot;Campaña de verano&quot; a $75,000.*

### Eliminar elementos

Para eliminar elementos de Workfront, haga lo siguiente:

* *Elimine el proyecto denominado &quot;Campaña de prueba del primer trimestre&quot;.*
* *Quite la tarea &quot;Imprimir producción de recursos&quot; del proyecto.*
* *Elimine el registro de campaña denominado &quot;Promoción antigua&quot;.*

>[!WARNING]
>
>Eliminar elementos en Workfront a través de una plataforma agéntica de IA es lo mismo que eliminarlos en la interfaz de Workfront. Confirme qué está a punto de eliminar la plataforma agéntica de IA antes de dejarlo continuar.

### Trabajo con aprobaciones

Para administrar las aprobaciones de documentos y recursos, haga lo siguiente:

* *Agregue a Sarah Chen y Miguel Álvarez como aprobadores en el documento actual.*
* *Envíe un recordatorio a los aprobadores del recurso &quot;Vídeo de campaña de primavera&quot; que no hayan respondido.*
* *Aplique la plantilla de aprobación &quot;Lanzamiento de marketing&quot; al recurso &quot;Vídeo de campaña de primavera&quot;.*


### Trabajo con registros de Planning

Para administrar los registros de planificación, haga lo siguiente:

* *Cree un nuevo registro de planificación denominado &quot;Plan de marketing del segundo trimestre&quot; para el equipo de marketing de marca.*
* *Agregue una nueva tarea denominada &quot;Auditoría de medios sociales&quot; al registro de planificación.*
* *Actualice la tarea &quot;Auditoría de medios sociales&quot; para que finalice el 18 de abril y asígnela al equipo creativo.*

### Trabajo con flujo de trabajo

Para administrar el flujo de trabajo, haga lo siguiente:

* *Enrute el proyecto &quot;Espacio aislado para la innovación en el segundo trimestre&quot; al Consejo de revisión de la innovación.*
* *Actualice el registro &quot;Campaña de verano&quot; al estado &quot;Listo para el lanzamiento&quot;.*
* *Aprobar el registro &quot;Campaña de verano&quot;.*


### Encadenar solicitudes en una conversación

Puede encadenar solicitudes en una sola conversación. La plataforma agéntica de IA mantiene el contexto, por lo que cada solicitud puede basarse en la anterior. Por ejemplo:

1. Pedir un conjunto de elementos: *Buscar mis tareas vencidas.*
1. Una vez que haya obtenido la lista, pida una acción sobre los resultados: *Actualice todos a viernes siguiente.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Consideraciones

Tenga en cuenta las siguientes consideraciones al utilizar el servidor MCP de Workfront.

### La plataforma agéntica de IA puede utilizar información de versiones anteriores de la conversación

Las plataformas agénticas de IA a veces reutilizan los datos de versiones anteriores en lugar de solicitar a Workfront la última versión. Si algo ha cambiado en Workfront desde la última vez que se buscó la plataforma agéntica de IA, es posible que vea información obsoleta.

Para obligar a la plataforma agéntica de IA a recuperar datos nuevos, pídala explícitamente. Por ejemplo:

* *Obtenga los datos más recientes de Workfront. No usar resultados en caché.*

### El servidor MCP de Workfront se actualiza automáticamente

Cuando Adobe lanza una nueva versión del servidor MCP de Workfront, su plataforma principal de IA utiliza la nueva versión automáticamente. No es necesario que vuelva a conectarse o cambie nada de su lado.

## Datos y seguridad

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Qué datos salen de Workfront

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Cómo gestionan los proveedores de plataformas agénticas de IA los datos de Workfront

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Diferencias entre plataformas agénticas de IA

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## Solución de problemas del uso diario

+++ Amplíe para ver sugerencias de solución de problemas para el uso diario del servidor MCP de Workfront.

| Problema | Causa probable | Corregir |
|---|---|---|
| La plataforma agéntica de IA le proporciona información obsoleta. | La plataforma agéntica de IA está reutilizando datos de versiones anteriores de la conversación. | Solicite datos nuevos a Workfront. |
| La plataforma agéntica de IA devolvió datos de elementos de Workfront incorrectos. | La plataforma de inteligencia artificial eligió los elementos equivocados basándose en términos ambiguos. | Vuelva a preguntar con nombres, ID o filtros más específicos. |
| Una actualización o eliminación no surtió efecto en Workfront. | La plataforma agéntica de IA aún no ha llamado a la acción o sus permisos no la permiten. | Confirme con la plataforma agéntica de IA que se ejecutó la acción y, a continuación, compruebe sus permisos de Workfront. |

Para obtener más información acerca de los problemas de configuración y autenticación, consulte [Solucionar problemas de configuración y autenticación](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) en [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Preguntas frecuentes

+++ Amplíe para ver las preguntas más frecuentes sobre el uso del servidor MCP de Workfront.

### ¿Con qué elementos de Workfront puedo trabajar a través de una plataforma agéntica de IA?

Cualquier elemento al que tenga acceso en Workfront mediante niveles de acceso y permisos de objeto.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### ¿Mis datos de Workfront se envían al proveedor de la plataforma agéntica de IA o se almacenan en él?

Para obtener más información, consulte [Datos y seguridad](#data-and-security) en este artículo.

### ¿Qué sucede cuando se publica una nueva versión del servidor MCP de Workfront?

El servidor MCP se actualiza automáticamente. No es necesario que vuelva a conectarse o cambie nada.

### ¿Necesito saber la API de Workfront para utilizar el servidor MCP de Workfront?

No. La plataforma agéntica de IA traduce sus solicitudes en lenguaje natural a las acciones correctas de Workfront. Si ya está familiarizado con la API de Workfront, las acciones le resultarán familiares, pero no es un requisito.

+++
