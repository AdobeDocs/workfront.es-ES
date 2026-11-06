---
product-area: betas
title: Introducción a la funcionalidad Organizaciones conectadas
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 1eaa497ba7e446f7fdf978f369205f309bbe231f
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 0%
---
# Introducción a la capacidad Organizaciones conectadas

>[!IMPORTANT]
>
>La capacidad Organizaciones conectadas se encuentra actualmente en una fase beta cerrada y abierta a un pequeño número de clientes.
>
>La versión beta abarca hasta finales de 2026.
>
>Si tiene alguna pregunta, póngase en contacto con el administrador del programa beta de Adobe.

La capacidad Organizaciones conectadas permite que una empresa y sus socios colaboren en el trabajo cuando ambas organizaciones han adquirido Adobe Workfront.

Por ejemplo, una empresa cliente puede enviar una solicitud a la empresa de su proveedor para que realice el trabajo.

Cada empresa puede seguir trabajando en su propia instancia de Workfront, con sus propios usuarios, permisos y flujos de trabajo.

Los objetos de trabajo se reflejan entre las dos instancias y solo se sincronizan los datos que ambas partes acuerdan compartir.

El resultado es una vista compartida de solicitudes, estados y decisiones sin inicios de sesión de invitado adicionales, licencias duplicadas o subprocesos de correo electrónico largos.

## Descripción general del flujo de trabajo actual de varias organizaciones

Cuando dos empresas invirtieron en Workfront, deberían poder trabajar juntas sin que una pagara dos veces o pasara al sistema de la otra.

En la actualidad, cuando las dos empresas trabajan en dos sistemas separados, su colaboración puede incluir algunos de los siguientes flujos de trabajo:

* Las solicitudes y los informes viajan a través de hilos de correo electrónico que son difíciles de seguir.

* Las entregas son manuales, con poca auditabilidad.

* Trabajar dentro del sistema de otra compañía significa inicios de sesión como invitado, licencias adicionales o ambas cosas.

* Circulan múltiples copias de archivos, y nadie está seguro de cuál es la fuente de la verdad.

* El estado es difícil de seguir, por lo que los administradores de cuentas invierten tiempo en crear mazos y programar reuniones de actualización.

## Descripción general de la solución Organización conectada

Al utilizar la capacidad Organización conectada, las dos empresas siguen trabajando en dos sistemas independientes y su colaboración incluirá algunos de los siguientes flujos de trabajo:

* Ninguna organización tiene acceso a un objeto en la instancia de la otra.
* Un objeto, como una solicitud de la organización cliente, se duplica y publica en la instancia del proveedor.
* Solo los metadatos configurados para la sincronización se mantienen actualizados entre las dos copias.
* Cada compañía administra sus propios usuarios, permisos y flujos de trabajo más allá de ese objeto.

El principio rector es compartir lo mínimo necesario para realizar el trabajo y mantener todo lo demás confidencial.

<table>
<tbody>
<tr class="odd">
<td><strong>Qué se comparte</strong></td>
<td><strong>Lo que permanece privado</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Breves y detalles de solicitud</p></li>
<li><p>Plazos e hitos acordados</p></li>
<li><p>Revisar comentarios</p></li>
<li><p>Decisiones de aprobación</p></li>
<li><p>Activos aprobados finales</p></li>
</ul></td>
<td><ul>
<li><p>Relaciones con otros clientes u otras agencias</p></li>
<li><p>Financieros, tasas y lo que se cobra al cliente</p></li>
<li><p>Planificación de recursos y capacidad</p></li>
<li><p>Estructura interna del proyecto, tareas y cualquier campo no seleccionado para compartir</p></li>
</ul></td>
</tr>
</tbody>
</table>

## Funciones disponibles en la versión beta

La primera fase del programa beta le permite conectar las dos instancias y comenzar el trabajo.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Característica** | **Qué hace** |
| **Organizaciones conectadas** | Vincula las dos instancias de Workfront entre las dos organizaciones. Durante la versión beta, Adobe configura la conexión. Actualmente se está desarrollando una configuración de autoservicio. |
| **Formularios de solicitud** | La empresa cliente crea un formulario de solicitud, lo publica y lo comparte con una empresa proveedora desde la configuración de uso compartido del formulario. |
| **admisión de solicitudes asistidas por IA** | El solicitante del cliente puede utilizar la capacidad de rellenado de formularios de IA para escribir un mensaje y adjuntar archivos en lugar de rellenar un formulario largo. El sistema asigna ese contenido a los campos del formulario y muestra la asignación para su revisión. El solicitante acepta el resultado y envía el formulario. |
| **Solicitudes reflejadas** | La solicitud enviada aparece en el área de Solicitudes de la empresa del proveedor como una copia de solo lectura, incluidos los valores de los campos personalizados. |
| **Conversión de solicitud a proyecto** | El proveedor convierte la solicitud en un proyecto y selecciona el portafolio, el programa y la plantilla para poner en marcha el trabajo. El nuevo objeto de la instancia del proveedor se vincula de nuevo a la solicitud original del cliente. La empresa solicitante no puede ver los detalles del trabajo real del lado del proveedor. |
| **Comentarios bidireccionales** | Los comentarios sobre la solicitud son visibles en ambos lados y llegan casi inmediatamente, por lo que ambas partes pueden trabajar para llegar a un acuerdo en un solo lugar. |
| **Solicitar aceptación** | Una vez que ambas partes están de acuerdo, el proveedor acepta la solicitud y el cliente puede ver que se ha aceptado. |
| **Actualizaciones de estado redactadas por IA** | Cuando un solicitante solicita el estado en un comentario, el proveedor puede utilizar comandos de IA para generar de forma rápida y coherente un borrador de respuesta. <br> El borrador incluye información de los objetos conectados a la solicitud, como la fecha planificada de finalización, la condición y las horas registradas en Horas planificadas. <br> Es un resumen de la información más importante, no una exportación campo a campo. Una persona lo revisa y edita antes de enviar una respuesta al cliente. |

## Flujo de trabajo de extremo a extremo

En esta sección se describe el flujo de trabajo de dos partes que participan en esta integración, después de conectar las instancias de Workfront de sus organizaciones respetadas.

Estamos utilizando un flujo de trabajo de cliente y proveedor como ejemplos.

### Flujo de trabajo del cliente

Como solicitante en la organización del cliente, puede hacer lo siguiente:

1. Cree o pídale a un administrador que cree un formulario de solicitud, lo publique y lo comparta con la organización del proveedor conectado.

2. Abra el formulario publicado en el área Solicitudes, introduzca una solicitud y adjunte los archivos necesarios.

3. Revise cómo se asigna el contenido a los campos del formulario, y acéptelo y envíelo.

### Flujo de trabajo del proveedor

Como administrador de trabajo en la organización del proveedor, haga lo siguiente:

1. Reciba la solicitud en el área de Solicitudes como una copia de solo lectura.

2. Discuta la solicitud a través de comentarios hasta que ambos lados estén alineados y luego acéptela.

3. Convierta la solicitud en un proyecto, eligiendo el portafolio, el programa y la plantilla, si es necesario.

4. Elija qué campos de proyecto se reflejan en la solicitud del cliente.

5. Responda a las preguntas de estado en los comentarios o genere una actualización de estado de borrador, revísela y publíquela en su solicitud. También se muestra en la solicitud original del cliente.

   A partir de ese momento, la solicitud del lado del proveedor actúa como una réplica de la solicitud original del cliente, por lo que los comentarios y los datos acordados permanecen sincronizados.

## Seguridad y gobernanza

Mantener los datos de cada organización protegidos es un requisito de diseño básico.

Una de las líneas de base que queremos que la versión beta establezca es la facilidad con la que los equipos de TI y seguridad pueden aprobar y administrar una conexión entre instancias.

Las siguientes son ventajas del flujo de trabajo de la organización conectada:

* **Sin acceso entre instancias**: no se necesitan usuarios de la organización asociada en su instancia, por lo que no hay inicios de sesión de invitados ni licencias adicionales.

* **Uso compartido mínimo necesario**: Solo se comparten los datos configurados para la sincronización. Todo lo demás permanece en su instancia de origen.

* **Controles independientes**: Cada organización mantiene sus propios usuarios, permisos y flujos de trabajo.

* **Ámbito de nivel de equipo**: las solicitudes están pensadas para llegar únicamente a los equipos de la agencia configurados para trabajar con ese cliente, utilizando los controles de acceso de Workfront existentes.

## Perspectiva de hoja de ruta

Las fases siguientes describen nuestro plan de desarrollo y lanzamiento actual. La secuencia puede cambiar según lo que aprendamos durante la fase beta. Las fases posteriores no son compromisos.

<table>
<tbody>
<tr class="odd">
<td><strong>Fase</strong></td>
<td><strong>Enfoque y capacidades planificadas</strong></td>
<td><strong>Estado</strong></td>
</tr>
<tr class="even">
<td><strong>Fase 1</strong></td>
<td>Conectar instancias y poner en marcha el trabajo: formularios de solicitud, entrada asistida por IA, solicitudes duplicadas, conversión de proyectos, comentarios y redacción de estado.</td>
<td>En la versión beta</td>
</tr>
<tr class="odd">
<td><strong>Fase 2</strong></td>
<td><ul>
<li><p>Revisión y aprobación mediante Frame y la experiencia unificada de revisión y aprobación</p></li>
<li><p>Las revisiones pendientes aparecen en Workfront o Frame, independientemente de dónde trabaje la parte interesada</p></li>
<li><p>Las anotaciones permanecen vinculadas al archivo de trabajo, por lo que los equipos creativos ven los comentarios en un solo lugar</p></li>
</ul></td>
<td>Planificados</td>
</tr>
<tr class="even">
<td><strong>Fase 3</strong></td>
<td><ul>
<li><p>Asignación de trabajo basada en tareas además de solicitudes</p></li>
<li><p>Estado más automatizado, informado por campos compartidos o no compartidos</p></li>
<li><p>Un nuevo tipo de objeto de envío, con metadatos definidos durante la información y heredados por el recurso aprobado final</p></li>
<li><p>Envío directo de activos finales aprobados al AEM de la marca, lo que reduce la entrada manual de metadatos</p></li>
</ul></td>
<td>Planificados</td>
</tr>
<tr class="odd">
<td><strong>Fase 4</strong></td>
<td><ul>
<li><p>Contexto compartido entre socios</p></li>
<li><p>Uso de Adobe Brand Intelligence <!--by the agency--> antes de la revisión, con acceso controlado por el equipo</p></li>
<li><p>Capacidades basadas en el contexto, como la estimación</p></li>
</ul></td>
<td>A largo plazo</td>
</tr>
</tbody>
</table>

## Participar en la versión beta

Hable con el administrador del programa beta de Adobe para participar en la versión beta.

### Lo que pedimos a los participantes

* Únase a una llamada de comentarios semanal.

* Reserve aproximadamente una hora por semana para realizar pruebas prácticas por su cuenta. Las sesiones de trabajo en directo en la llamada son una opción.

* Llevar las perspectivas de ambos socios a las reuniones, siempre que sea posible.

* Identifique los entornos de Workfront a los que conectarse y proporcione cuentas de administración para un pequeño número de ingenieros de Adobe para que puedan validar la conexión.

### Lo que queremos aprender

* ¿Es la duplicación de un objeto y la sincronización de solo los datos seleccionados el modelo de uso compartido correcto? ¿Es lo suficientemente flexible para cada lado?

* ¿Es correcta la secuenciación de fases o debería llegar antes una capacidad posterior?

* ¿Qué puntos de contacto faltan en la colaboración?

* ¿Cómo deberían funcionar la asignación y la asignación de nombres de campo entre las dos instancias?

  En la actualidad, el formulario y la solicitud son propiedad del cliente y el proveedor los ve de solo lectura con los nombres de campo del cliente.

* ¿Qué necesita el departamento de TI para aprobar y administrar una conexión?




<!--

Original pdf from team:

**ADOBE WORKFRONT | BETA PROGRAM**

**Agency Brand Connectors**

Product overview for beta participants

# **Overview**

Agency Brand Connectors lets a brand and its agency collaborate on work when both organizations run Adobe Workfront. Each side keeps working in its own Workfront instance, with its own users, permissions, and workflows. Work objects are mirrored between the two instances, and only the data both sides agree to share is synchronized.

The result is a shared view of requests, status, and decisions without guest logins, duplicate licenses, or long email threads.

# **The challenge this addresses**

When a brand and an agency are both invested in Workfront, they should be able to work together without either one paying twice or moving into the other's system. Today the collaboration usually looks like this:

  - Requests and briefs travel through email threads that are hard to follow.

  - Handoffs are manual, with little auditability.

  - Working inside a partner's system means guest logins, extra licenses, or both.

  - Multiple copies of files circulate, and no one is sure which is the source of truth.

  - Status is hard to see, so producers and account managers spend time building decks and scheduling update meetings.

# **How it works: the sharing model**

Neither organization accesses an object in the other's instance. Instead, an object such as a request is duplicated and published into the partner's instance, and only the metadata configured for sync is kept up to date between the two copies. Each side manages its own users, permissions, and workflows downstream of that object.

The guiding principle is to share the minimum needed to get the work done, and to keep everything else confidential.

<table>
<tbody>
<tr class="odd">
<td><strong>What is shared</strong></td>
<td><strong>What stays private</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs and request details</p></li>
<li><p>Agreed deadlines and milestones</p></li>
<li><p>Review comments</p></li>
<li><p>Approval decisions</p></li>
<li><p>Final approved assets</p></li>
</ul></td>
<td><ul>
<li><p>Relationships with other clients or other agencies</p></li>
<li><p>Financials, rates, and what is charged to the client</p></li>
<li><p>Resource planning and capacity</p></li>
<li><p>Internal project structure, tasks, and any fields not selected for sharing</p></li>
</ul></td>
</tr>
</tbody>
</table>

# **Features available in the beta**

The first phase of the beta covers connecting two instances and kicking off work.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Feature**                       | **What it does**                                                                                                                                                                                                                                                                                                                      |
| **Connected organizations**       | Links a brand instance and an agency instance. During the beta, Adobe configures the connection. A self-serve setup is being worked on.                                                                                                                                                                                               |
| **Request forms**                 | The brand creates a request form, publishes it, and shares it with a connected organization from the form's Share settings.                                                                                                                                                                                                           |
| **AI-assisted request intake**    | The requester types a prompt and attaches files instead of filling out a long form. The system maps that content to the form fields and shows the mapping for review. The requester accepts the result and submits. This uses Workfront's existing form-filling technology.                                                           |
| **Mirrored requests**             | The submitted request appears in the agency's request area as a read-only copy, including custom field values.                                                                                                                                                                                                                        |
| **Request-to-project conversion** | The agency converts the request into a project and selects the portfolio, program, and template. The new object is linked back to the request. Downstream work on the agency side is not visible to the brand.                                                                                                                        |
| **Two-way comments**              | Comments on the request are visible on both sides and arrive almost immediately, so both parties can work toward agreement in one place.                                                                                                                                                                                              |
| **Request acceptance**            | Once both sides agree, the agency accepts the request and the brand sees that it has been accepted.                                                                                                                                                                                                                                   |
| **AI-drafted status updates**     | When a brand asks for status in a comment, the agency can use a slash command to generate a draft reply. The draft draws on connected objects, such as planned completion date, condition, and hours logged against hours planned. It is a summary, not a field-by-field export, and a person reviews and edits it before publishing. |

# **End-to-end workflow**

## **Brand side**

1.  Create a request form, publish it, and share it with the connected agency.

2.  Open the published form, enter a prompt, and attach any files.

3.  Review how the content maps to the form fields, accept, and submit.

## **Agency side**

1.  Receive the request in the request area as a read-only copy.

2.  Discuss the request through comments until both sides are aligned, then accept it.

3.  Convert the request into a project, choosing the portfolio, program, and template.

4.  Choose which project data is mirrored back to the brand.

5.  Answer status questions in comments, or generate a draft status update, review it, and publish.

From that point on, the request on the agency side acts as a replica of the request on the brand side, so comments and agreed data stay in step.

# **Security and governance**

Keeping each organization's data protected is a core design requirement, and one of the baselines we want the beta to establish is how easily IT and security teams can approve and administer a connection between instances.

  - **No cross-instance access.** No users from the partner organization are needed in your instance, so there are no guest logins and no additional licenses.

  - **Minimum necessary sharing.** Only the data configured for sync is shared. Everything else stays in the originating instance.

  - **Independent controls.** Each organization keeps its own users, permissions, and workflows.

  - **Team-level scoping.** Requests are intended to reach only the agency teams set up to work on that brand, using existing Workfront access controls.

# **Roadmap**

The phases below describe our current plan. Sequencing may change based on what we learn in the beta, and later phases are not commitments.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus and planned capabilities</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connect instances and kick off work: request forms, AI-assisted intake, mirrored requests, project conversion, comments, and status drafting.</td>
<td>In beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Review and approval using Frame and the unified review and approval experience</p></li>
<li><p>Pending reviews appear in Workfront or Frame, wherever the stakeholder works</p></li>
<li><p>Annotations stay tied to the working file so creative teams see feedback in one place</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Task-based work assignment in addition to requests</p></li>
<li><p>More automated status, informed by shared or unshared fields</p></li>
<li><p>A new deliverable object type, with metadata defined during briefing and inherited by the final approved asset</p></li>
<li><p>Direct delivery of approved final assets into the brand's AEM, reducing manual metadata entry</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Shared context between brand and agency</p></li>
<li><p>Use of Adobe Brand Intelligence by the agency before review, with access controlled by team</p></li>
<li><p>Context-informed capabilities such as estimating</p></li>
</ul></td>
<td>Longer term</td>
</tr>
</tbody>
</table>

# **Participating in the beta**

## **What we ask of participants**

  - Join a weekly feedback call.

  - Set aside about one hour per week for hands-on testing. Live working sessions on the call are an option if time is tight.

  - Bring both the brand and the agency perspective where possible.

  - Identify the Workfront environments to connect, and provision admin accounts for a small number of Adobe engineers so they can validate the connection.

## **What we want to learn**

  - Is mirroring an object and syncing only selected data the right sharing model, and is it flexible enough for each side?

  - Is the phase sequencing right, or should a later capability come sooner?

  - What touchpoints are missing from the collaboration?

  - How should field naming and mapping work between brand and agency instances? Today, the form and request are owned by the brand, and the agency sees them read-only with the brand's field names.

  - What does IT need to approve and administer a connection?

The beta runs through the end of the year. For questions or blockers, contact your Adobe beta program manager.


-->