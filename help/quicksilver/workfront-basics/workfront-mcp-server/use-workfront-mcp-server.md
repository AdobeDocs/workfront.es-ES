---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Uso del servidor MCP de Adobe Workfront
description: Utilice el servidor MCP de Adobe Workfront para buscar, crear, actualizar y administrar elementos de Workfront a través de una conversación en lenguaje natural en una plataforma agéntica de IA.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 648342f0002046febba1b8e751bc1cffec2c1346
workflow-type: tm+mt
source-wordcount: '1793'
ht-degree: 0%

---


# Uso del servidor MCP de Adobe Workfront

{{highlighted-preview-article-level}}

El servidor MCP [!DNL Adobe Workfront] le permite buscar, crear, actualizar y administrar elementos de Workfront solicitando una plataforma auténtica de IA en lenguaje natural. La plataforma decide qué acciones de Workfront llamar y gestiona la conversación con Workfront por usted.

>[!IMPORTANT]
>
>Actualmente, el servidor MCP de Workfront solo está disponible para clientes de la región de EE. UU. que utilizan AWS.

## Requisitos previos

* Debe configurar la conexión entre su plataforma agéntica de IA y el servidor MCP de Workfront. Para obtener instrucciones de instalación, consulte [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).
* La instancia de Workfront debe estar habilitada en Adobe Identity Management System (IMS).
* Debe tener una cuenta de Workfront con el nivel de acceso y los permisos de objeto necesarios para los elementos con los que desea trabajar.
* Para utilizar MCP con Workfront Planning, su organización debe estar en un paquete de Workfront que incluya Adobe Workfront Planning.

Este artículo supone que ya ha configurado la conexión. Para obtener información sobre la instalación, consulte [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Herramientas disponibles

El servidor MCP de Workfront expone un conjunto de herramientas que la plataforma agéntica de IA llama en su nombre. Por ejemplo, herramientas para buscar en Workfront, crear elementos, actualizar campos y administrar aprobaciones. Para obtener la lista de referencia completa, consulte [Herramientas de servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Cuando conecta una plataforma independiente de IA a Workfront, esta actúa en Workfront con su cuenta y permisos de Workfront. Las acciones de la plataforma tienen el mismo efecto que las acciones que realiza directamente en la interfaz de Workfront.<br>
>
>Usted y su proveedor de plataformas agénticas de IA son responsables de las acciones que realiza la plataforma en Workfront. Adobe no se responsabiliza de los cambios que la plataforma agéntica de IA realice en los datos de Workfront.<br>
>
>Antes de dejar que la plataforma agéntica de IA continúe con una solicitud, confirme que comprende lo que pretende hacer, especialmente para las acciones que cambian o eliminan datos.


## Ejemplos de qué preguntar

Una vez que esté conectado, escriba solicitudes en lenguaje natural en la plataforma agéntica de IA. La plataforma agéntica de IA decide qué acciones de Workfront llamar y devuelve los resultados.

>[!NOTE]
>
>Es posible que algunas acciones no estén disponibles debido a los controles de administración del área Configuración de Workfront. Por ejemplo, es posible que no pueda crear elementos si el administrador de Workfront ha deshabilitado las acciones de escritura para el servidor MCP.


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

>[!IMPORTANT]
>
>* Para utilizar MCP con Workfront Planning, su organización debe estar en un paquete de Workfront que incluya Adobe Workfront Planning.

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


## Consideraciones

Tenga en cuenta las siguientes consideraciones al utilizar el servidor MCP de Workfront:

### La plataforma agéntica de IA puede utilizar información de versiones anteriores de la conversación

Las plataformas agénticas de IA a veces reutilizan los datos de versiones anteriores en lugar de solicitar a Workfront la última versión. Si algo ha cambiado en Workfront desde la última vez que se buscó la plataforma agéntica de IA, es posible que vea información obsoleta.

Para obligar a la plataforma agéntica de IA a recuperar datos nuevos, pídala explícitamente. Por ejemplo:

* *Obtenga los datos más recientes de Workfront. No usar resultados en caché.*

### Buscar actualizaciones en el servidor MCP de Workfront

Es posible que desee actualizar periódicamente la conexión con el servidor MCP de Workfront para asegurarse de que dispone de las herramientas y funciones más recientes.

La mayoría de las actualizaciones deben realizarse automáticamente. Sin embargo, recomendamos consultar las notas de la versión de Workfront periódicamente.


## Datos y seguridad

Las herramientas del servidor MCP de Workfront son coherentes con el funcionamiento de las llamadas de API. Workfront no almacena preguntas, respuestas ni ningún otro tipo de datos. Sea cual sea la información de Workfront que solicite, es accesible desde la plataforma Workfront.

Los permisos de objeto y nivel de acceso determinan lo que se puede consultar o escribir en Workfront. El administrador de Workfront controla las acciones de lectura y escritura de MCP en el área Configuración de Workfront.

### Qué datos salen de Workfront

El proveedor de la plataforma agéntica de IA tiene acceso a los datos de Workfront con los que interactúa a través del servidor MCP de Workfront. Consulte con su proveedor de plataforma agéntica de IA para obtener más información.


### Cómo gestionan los proveedores de plataformas agénticas de IA los datos de Workfront

Workfront no controla cómo el proveedor de la plataforma agéntica de IA gestiona los datos de Workfront. Consulte con su proveedor de plataforma agéntica de IA para obtener más información.

## Solución de problemas del uso diario

+++ Amplíe para ver sugerencias de solución de problemas para el uso diario del servidor MCP de Workfront.

| Problema | Causa probable | Corregir |
| --- | --- | --- |
| La plataforma agéntica de IA le proporciona información obsoleta. | La plataforma agéntica de IA está reutilizando datos de versiones anteriores de la conversación. | Solicite datos nuevos a Workfront. |
| La plataforma agéntica de IA devolvió datos de elementos de Workfront incorrectos. | La plataforma de inteligencia artificial eligió los elementos equivocados basándose en términos ambiguos. | Vuelva a preguntar con nombres, ID o filtros más específicos. |
| Una actualización o eliminación no surtió efecto en Workfront. | El administrador de Workfront ha deshabilitado las acciones de escritura para el servidor MCP de Workfront o no tiene permiso para realizar la acción en el elemento específico. | Confirme con la plataforma agéntica de IA que se ejecutó la acción. A continuación, compruebe que las acciones de escritura estén habilitadas para el servidor MCP de Workfront y que tiene permiso para cambiar el elemento. |

Para obtener más información acerca de los problemas de configuración y autenticación, consulte [Solucionar problemas de configuración y autenticación](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) en [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Preguntas frecuentes

+++ Amplíe para ver las preguntas más frecuentes sobre el uso del servidor MCP de Workfront.

### ¿Qué es una plataforma agéntica de IA?

Una plataforma agéntica de IA es una herramienta de IA que puede realizar acciones en su nombre en
otros sistemas, no solo responder preguntas. Al conectar uno a Workfront
a través del servidor MCP, puede encontrar, crear, actualizar y eliminar Workfront
elementos basados en lo que se le pide en lenguaje natural. Algunos ejemplos son Claude
Escritorio, ChatGPT y otros clientes de IA compatibles con MCP.


### ¿Debo ser administrador de Workfront para utilizar el servidor MCP de Workfront?

No. Cualquier usuario de Workfront puede utilizar el servidor MCP de Workfront a través de un
Plataforma agéntica de IA. La plataforma independiente actúa con su Workfront
cuenta, nivel de acceso y permisos de objeto, para que solo pueda hacer lo que desee
ya se podía hacer directamente en Workfront.

### ¿Por qué la plataforma agéntica de IA no puede crear, actualizar o eliminar elementos por mí?

El administrador de Workfront controla qué acciones de MCP están permitidas en la variable
Área de configuración de Workfront. Si las acciones de escritura están desactivadas, la plataforma agéntica de IA
Todavía puede encontrar y leer elementos de Workfront, pero no puede realizar cambios. Usted también
necesita el nivel de acceso y los permisos de objeto adecuados para los elementos específicos
está trabajando con.

### ¿La plataforma agéntica de IA me preguntará antes de cambiar o eliminar datos de Workfront?

Eso depende de la plataforma de IA agéntica, no de Workfront. La mayoría de las plataformas
le pedirá que confirme antes de ejecutar una acción, especialmente en el caso de eliminaciones.
Antes de aprobar una solicitud, lea lo que la plataforma dice que está a punto de hacer:
los cambios se producen en Workfront del mismo modo que si se hicieran
usted mismo en la interfaz.

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### ¿Por qué la plataforma agéntica de IA devolvió los elementos incorrectos de Workfront?

La plataforma agéntica de IA selecciona elementos en función de las palabras utilizadas. Si su
La solicitud es ambigua (por ejemplo, dos proyectos tienen nombres similares)
podría elegir el equivocado. Vuelva a preguntar con nombres, ID, fechas más específicos,
o filtros para reducir los resultados.


### ¿Con qué elementos de Workfront puedo trabajar a través de una plataforma agéntica de IA?

Cualquier elemento al que tenga acceso en Workfront a través de su nivel de acceso y
permisos de objeto. Esto incluye proyectos, tareas, problemas, documentos,
aprobaciones, registros de Planning y mucho más.

### ¿Pueden otras personas ver mis conversaciones con la plataforma agéntica de IA?

Workfront no almacena sus mensajes ni las respuestas de la plataforma agéntica de IA.
Quienquiera que proporcione su plataforma agéntica de IA controla cómo sus conversaciones
se almacenan o comparten. Consulte con su proveedor de plataforma agéntica de IA para
detalles.

### ¿Necesito saber la API de Workfront o qué herramienta MCP utilizar?

No. La plataforma agéntica de IA traduce su solicitud en lenguaje natural a
Seleccione las acciones y las herramientas de Workfront que más le convengan. Si usted es
ya familiarizadas con la API de Workfront, las acciones le resultarán familiares,
pero no es un requisito.

### ¿Mis datos de Workfront se envían al proveedor de la plataforma agéntica de IA o se almacenan en él?

Para obtener más información, consulte [Datos y seguridad](#data-and-security) en esta
artículo.

### ¿Qué sucede cuando se publica una nueva versión del servidor MCP de Workfront?

Por lo general, el servidor MCP se actualiza automáticamente, pero es posible que tenga que actualizar la conexión con el servidor MCP a veces para ver las herramientas y capacidades más recientes.

### ¿Puedo usar el servidor MCP de Workfront si mi instancia de Workfront no está habilitada en Adobe Identity Management System (IMS)?

No. La instancia de Workfront debe estar habilitada en Adobe Identity Management System (IMS) para utilizar el servidor MCP de Workfront. Si no está seguro de si la instancia está habilitada en IMS, póngase en contacto con el administrador de Workfront.


+++
