---
title: 'Creación de Bridge: Conexión de la intención estratégica a los proyectos'
description: Aprenda a crear un "hilo estratégico" entre sus planes de alto nivel en Adobe Workfront Planning y su ejecución diaria de flujos de trabajo en Adobe Workfront.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 567ab223-b282-4b98-9655-7b9766fba869
source-git-commit: 699add479d958b9f3fc01ae30513ddf6689620f1
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---


# Construya el puente: conectando la intención estratégica con los proyectos

{{planning-important-intro}}

Aprenda a crear un hilo estratégico entre sus planes de alto nivel en Adobe Workfront Planning y su ejecución diaria en Workfront. Puede crear un puente entre la estrategia y la ejecución mediante conexiones.

Esta guía está dirigida a los administradores de Workfront y de Workspace que implementan Workfront Planning.

## Información general sobre la alineación de la estrategia con la ejecución

Al conectar tu estrategia con tu trabajo diario, la visión se convierte en realidad. Cuando los planes de alto nivel están sincronizados con la ejecución, se crea un subproceso estratégico que garantiza que todos los proyectos y tareas hagan avanzar la empresa.

Para lograr esta alineación, es necesario establecer un conjunto de vínculos técnicos y protecciones de procesos que conecten los esfuerzos de Workfront con los registros estratégicos de Workfront Planning.

Al reducir la brecha entre la planificación y la acción, se asegura de que la energía de su equipo siempre se centre en sus objetivos de mayor prioridad.

## Establezca la base creando una conexión

Antes de poder vincular la planificación y la ejecución, como administrador de espacio de trabajo debe definir qué tipos de registro son aptos para una conexión.

### Información general del campo de conexión

El puente comienza con la creación de un campo de conexión.

Un campo de conexión sirve como protocolo de enlace técnico entre tipos de registro.

Este tipo de campo es el motor de todas las relaciones de Workfront Planning. Es una expresión de intención, ya que establece que un tipo de registro específico (como una Táctica de canal) puede vincularse a otros tipos de objetos, ya residan en Planning o Workfront.

Para obtener más información, vea [Información general sobre los tipos de registros conectados](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

### Defina cuándo crear una conexión

Lo ideal es que decida si necesita crear conexiones antes de que se cree cualquier trabajo.

Al agregar un campo de conexión, está creando el entorno para admitir un subproceso estratégico, independientemente de cómo se creen finalmente los registros individuales.

## Establecer estrategia y ejecución sincronizadas

Para mantener la capa estratégica centrada, recomendamos enfocar los registros de planificación en la intención de alto nivel mientras se utiliza Workfront para la ejecución táctica.

Este enfoque utiliza las fortalezas únicas de ambos módulos de las siguientes maneras:

* **Planificación de Workfront (la capa estratégica):** Permanece de alto nivel. Rastrea la campaña, la táctica del canal y el presupuesto. No hace ruido y está preparado para ejecutivos.

* **Workfront (el nivel de ejecución):** administra los detalles tácticos. Puede administrar experiencias o actividades individuales como proyectos, tareas y problemas. Puede asignarlas para su propiedad y compilarlas en aprobaciones para su ejecución.

## Pasar de la intención a la acción activando el puente

Una vez configurada la conexión, debe decidir cómo activar el vínculo entre un registro estratégico específico y un proyecto de ejecución.

### Usar una ruta guiada por tabla

Los estrategas y los usuarios avanzados suelen utilizar la vista de tabla como su área de trabajo para refinar los planes a lo largo del tiempo.

La creación de un registro en una tabla no establece un vínculo a Workfront de forma predeterminada.

La conexión a un proyecto de ejecución se establece cuando un usuario decide activar el vínculo.

Esto se puede hacer de las siguientes maneras:

* Cree manualmente un proyecto conectado descendente directamente desde el campo de conexión de Workfront Planning o desde una página Conexiones opcional en la vista de detalles del registro.

  La creación manual genera un proyecto en blanco sin formularios personalizados específicos.

  Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Automáticamente, mediante automatizaciones de Workfront Planning, para necesidades más complejas.

  Estas automatizaciones están disponibles como botones en la barra de acciones al seleccionar una fila de una tabla.

  Esto permite la supervisión humana o la creación de marcadores de posición, lo que garantiza que los proyectos solo se generen en el entorno de flujo de trabajo cuando realmente se necesitan.

  Para obtener más información, vea [Crear objetos mediante automatizaciones de registros de Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md)


### Creación de activaciones automatizadas

Para organizaciones con solicitudes de gran volumen o necesidades de automatización avanzadas, el puente se puede activar automáticamente en función de eventos específicos o de valores de campo configurados en un formulario de solicitud.

Necesitará una licencia para Adobe Workfront Fusion para este enfoque.

Para obtener más información, consulte [Configurar y administrar Workfront Fusion: índice de artículos](https://experienceleague.adobe.com/es/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-workfront-fusion-toc).

* **Usar déclencheur de envío:** Debido a que los formularios proporcionan un único evento de envío limpio, se pueden usar como déclencheur para las automatizaciones de Fusion. Un escenario de Fusion puede detectar un envío de formulario y generar inmediatamente un proyecto vinculado en Workfront.

* **Usar déclencheur de valor de campo:** Para una automatización más profunda, puede configurar Fusion para que supervise campos específicos. Por ejemplo, una casilla de verificación simple denominada &quot;Listo para la ejecución&quot; puede servir como catalizador y establecer el puente automáticamente en el momento en que se selecciona.

## Agregar campos de búsqueda para ver la superficie

Una vez vinculado un proyecto, puede mostrar datos en tiempo real de Workfront directamente en el registro de Planning agregando campos de búsqueda del proyecto.

Como administrador del espacio de trabajo, puede configurar campos de búsqueda para extraer cualquier sistema o campo personalizado del proyecto vinculado (como Fecha real de finalización o Creative Lead) en el tipo de registro de Planning. Una vez capturados, estos datos se pueden resumir en varios niveles de la jerarquía estratégica, hasta el nivel de campaña. Esto proporciona potentes informes agregados para las partes interesadas en todo el ciclo de vida del marketing, lo que les mantiene informados sin necesidad de abandonar el entorno de planificación.

## Consiga visibilidad conectando estrategia con acción

El valor final del puente es la visibilidad en tiempo real.

Al conectar la intención con la acción, puede responder preguntas comerciales críticas de un vistazo. A continuación se muestran ejemplos de estas preguntas:

* ¿Está nuestra campaña &quot;Conocimiento de la marca del año fiscal 2026&quot; dando resultados de forma activa en este momento?

* ¿Dónde necesitan nuestras tácticas estratégicas más apoyo creativo para mantenerse a tiempo?

* ¿Cómo estamos alineando nuestros recursos con nuestros pilares estratégicos de máxima prioridad?

## Prácticas recomendadas y sugerencias

### Dos:

* **Utilice la metáfora de &quot;hilo estratégico&quot;:** Recuerde a los equipos que cada proyecto debe ser un &quot;hilo&quot; en una cadena estratégica.

* **Automatice el traspaso:** Use automatizaciones para crear proyectos en déclencheur a fin de ahorrar tiempo y esfuerzo, a la vez que mejore la conectividad y el control de los datos.

* **Vínculo, no duplicar:** Use campos de búsqueda para que aparezcan datos de ejecución en tiempo real (como fechas de estado o finalización) en sus registros estratégicos. Esto garantiza que sus vistas estratégicas sean siempre precisas sin necesidad de actualizaciones manuales por parte de su equipo.

### No lo haga:

* **No trate los registros de planificación como listas de tareas:** El puente está diseñado para conectar la intención estratégica con los proyectos de ejecución. Mantenga los registros de planificación centrados en el &quot;qué&quot; y el &quot;por qué&quot;, y permita que el módulo de flujo de trabajo gestione el &quot;cómo&quot; granular a través de las tareas y los problemas.

* **No sincronizar en exceso:** No es necesario que sincronice todos los detalles de nivel de proyecto con Planning. Mantenga la capa estratégica de alto nivel y libre de ruido.

* **No salte el puente:** Si el trabajo comienza en el módulo Flujo de trabajo sin un vínculo a Planning, ha creado un &quot;Plan en la sombra&quot; que es invisible para el liderazgo.

<!--original content:

# The Bridge: Connecting Strategic Intent to Projects 

 

## Goal 

Learn how to create a "strategic thread" between your high-level plans in Workfront Planning and your daily execution in the Workflow module. 

 

## Overview 

Connecting your strategy to your daily work turns vision into reality. When high-level plans are in sync with execution, you create a **strategic thread** that ensures every project and task moves the business forward. 

 

Achieving this alignment requires a set of technical links and process guardrails that connect efforts in the **Workflow module** with strategic records in **Workfront Planning (WFP)**. By bridging the gap between planning and action, you ensure that your team's energy is always focused on your highest-priority goals. 

 

## The foundation: Establishing the connection 

Before you can bridge planning and execution, a workspace manager must define which record types are eligible for a connection. 

 

### The connection field: The technical handshake 

The bridge begins with a **connection field**. This field type is the engine behind all relationships in WFP. It is an expression of intent, in that it establishes that a specific record type (like a *channel tactic*) is allowed to be linked to other objects, whether they live in the workflow module or within planning itself. 

 

### Deciding to connect 

Establishing this allowance is a configuration-level decision that typically happens before any work is created. By adding a connection field, you are architecting your environment to support a "strategic thread," regardless of how the individual records are eventually created. 

 

## Strategy and execution in sync 

To keep your strategic layer focused, we recommend focusing your planning records on high-level intent while using the Workflow module for tactical execution. This approach uses the unique strengths of both modules: 

 

*   **Workfront Planning (The strategic layer):** Stays high-level. It tracks the *Campaign*, the *Channel Tactic*, and the *Budget*. It is noise-free and executive-ready. 

*   **Workflow module (The execution layer):** Manages the tactical details. Individual "Experiences" or "Activities" are managed here as **projects, tasks, and issues**. 

 

## Activating the bridge: From intent to action 

Once the connection is configured, you must decide how to activate the link between a specific strategic record and an execution project. 

 

### Professional triage: The table-led path 

Strategists and power users often use the **table view** as their "workbench" to refine plans over time.  

*   **Deliberate handoff:** By default, creating a record in a table does not establish a link to the Workflow module. The connection to an execution project is established when a user decides to activate the link. This can be done by manually creating a downstream connected project directly from the connection field in WFP or an optional **connection view page** in the record's detail view. Note that manual creation results in a blank project without specific custom forms; for more complex needs, you can use a **native WFP automation**. These automations are available when you select a row in a table, appearing as buttons in the blue action bar at the bottom of your screen. This allows for human oversight or placeholder creation, ensuring that projects are only generated in your workflow environment when they are truly needed. 

 

### Automated activation 

For organizations with high-volume requests or advanced automation needs, the bridge can be activated automatically based on specific events or field values. 

*   **Submission triggers:** Because forms provide a single, clean "submission event," they can be used as triggers for **Fusion automations**. A scenario can detect a form submission and immediately generate a linked project in the workflow module. 

*   **Field-value triggers:** For deeper automation, you can configure **Fusion** to monitor specific fields. For example, a simple checkbox labeled "ready for execution" can serve as the catalyst, establishing the bridge automatically the moment it is checked. 

 

## Surfacing visibility: Lookup fields 

Once a project is linked, you can surface real-time data from the Workflow module directly within the WFP record. 

 

A workspace manager can set up **lookup fields** to pull any native or custom field from the linked project (such as *actual completion date* or *creative lead*) into the WFP record type. Once captured, this data can be rolled up through multiple levels of your strategic hierarchy—even all the way to the campaign level. This provides powerful aggregate reporting for stakeholders across the entire marketing lifecycle, keeping them informed without needing to leave the planning environment. 

 

## Strategy-to-action visibility 

The ultimate value of the bridge is **real-time visibility**. By connecting intent to action, you can answer critical business questions at a glance: 

 

*   "Is our 'FY26 Brand Awareness' campaign actively delivering results right now?" 

*   "Where do our strategic tactics need more creative support to stay on schedule?" 

*   "How are we aligning our resources with our highest-priority strategic pillars?" 

 

## Best practices & tips 

 

### Do: 

*   **Use the "strategic thread" metaphor.** Remind teams that every project should be a "bead" on a strategic string. 

*   **Automate the handoff.** Use automations to trigger project creation to save time and effort while also improving data connectivity and governance. 

*   **Link, don't duplicate.** Use lookup fields to surface real-time execution data (like status or completion dates) in your strategic records. This ensures your strategic views are always accurate without requiring manual updates from your team. 

 

### Don't: 

*   **Don't treat planning records as task lists.** The bridge is designed to connect strategic intent to execution projects. Keep your planning records focused on the "what" and "why," and let the workflow module handle the granular "how" through tasks and issues. 

*   **Don't over-sync.** You don't need to sync every project-level detail back to Planning. Keep the strategic layer high-level and noise-free. 

*   **Don't bypass the bridge.** If work starts in the Workflow module without a link to Planning, you've created a "Shadow Plan" that is invisible to leadership. 

-->



