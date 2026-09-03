---
title: Preguntas y prácticas recomendadas de CX Coworker
content-type: reference
description: Conozca las prácticas recomendadas para utilizar Coworker en Workfront y vea una lista de ejemplos de mensajes.
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 2%

---

# Preguntas y prácticas recomendadas de CX Coworker

&lt;!—NO USE ESTO—En lugar de vincular al artículo de indicaciones de ejemplo de MCP, asegúrese de que esté actualizado con las últimas versiones de MCP—>

>[!IMPORTANT]
>
>CX Coworker no está disponible actualmente para organizaciones de atención médica, finanzas u otras industrias con datos confidenciales. Estas organizaciones disponen de un asistente de IA. Para obtener más información, consulte [Descripción general del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

Con CX Coworker, puede utilizar lenguaje natural para interactuar con Workfront Workflow y Workfront Planning.

Sus compañeros forman parte de Adobe Experience Cloud Agent Orchestrator.

Para obtener más información sobre Agent Orchestrator, consulte [Adobe Experience Platform Agent Orchestrator](https://experienceleague.adobe.com/es/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator).

## Requisitos de acceso

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Seleccionar, Prime o Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar o claro</p>
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td><p>Para cualquier funcionalidad fuera de las aptitudes básicas, su organización debe haber adquirido Adobe Agent Orchestrator.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Debe tener los permisos adecuados para interactuar con cualquier objeto a través de Coworker.</p> <p>Por ejemplo, para recibir información sobre un proyecto a través de Colaborador, debe tener al menos permiso de visualización en ese proyecto.</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

* El administrador de Workfront debe haber habilitado el Asistente de IA para su organización.

  Para obtener más información, consulte [Requisitos previos para el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant) en el artículo Información general del asistente de IA.
* El administrador de Workfront debe haber habilitado el asistente de IA para su nivel de acceso.

  Para obtener más información, consulte [Habilitar o deshabilitar el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Consideraciones

Tenga en cuenta las siguientes restricciones al utilizar CX Coworker:

### Reversibilidad

Algunas acciones se pueden revertir. Por ejemplo, si se crea un objeto, esa creación se puede invertir.

Sin embargo, algunas acciones, como la eliminación de objetos, **no** se pueden revertir. Se recomienda tener esto en cuenta al realizar acciones en los datos a través de Coworker.

### Restricciones de cobertura de datos/objetos

* La consulta y la creación de informes sobre campos personalizados se encuentran en sus primeras etapas, y algunas habilidades (como los ayudantes de consulta basados en API) aún no administran campos personalizados arbitrarios para la agregación y el filtrado.

### Limitaciones de interacción/experiencia de usuario

* Actualmente, CX Coworker no &quot;aprende&quot; a largo plazo del estilo o las preferencias de un usuario individual. Cada chat utiliza únicamente la conversación actual y el conocimiento del producto.
* El contexto de conversación se mantiene dentro de una sola sesión de chat. Al abrir una página nueva o cerrar el asistente, se restablece el historial de conversaciones.
* Si los procedimientos de aprobación se encuentran en una aplicación externa como Confluence o SharePoint y solo están vinculados a través de campos URL, el colaborador no recupera ni razona actualmente a través de esas páginas.

### Almacenamiento de datos / Claves gestionadas por el cliente

* Como CX Coworker forma parte de Adobe Experience Platform Agent Orchestrator, los datos de sus interacciones con Coworker se almacenan en Adobe Experience Platform, no en Workfront. Por lo tanto, estos datos no están cubiertos por los acuerdos de Claves administradas por el cliente de Workfront (BYOK).

## Aptitudes básicas de IA de uso general

>[!IMPORTANT]
>
>Estas funciones de uso general están disponibles para todos los usuarios cuya organización tenga registrado un Contrato de Adobe AI firmado.

Para obtener prácticas recomendadas y preguntas sobre estas habilidades de uso general, consulte [Preguntas y prácticas recomendadas del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md).

<!--Follow up with Oznur-->

### Conocimiento del producto

CX Coworker puede proporcionar instrucciones o información de referencia extraída de la documentación de Workfront.

Para obtener más información sobre cómo extraer información de la documentación de Workfront, consulte [Obtener ayuda del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

Ejemplo: ¿Cómo cambio el tipo de duración de la tarea?

### Resumen de proyecto, tarea y problema

CX Coworker puede resumir el proyecto, las tareas o los problemas <!--, or documents--> que se han cargado a Workfront.

Para obtener más información acerca de los resúmenes de proyectos, tareas y problemas, vea [Resumir con el Asistente para IA](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

Ejemplo: Resuma el proyecto llamado Campaña de otoño de 2026.

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## Coworker de CX en Workfront

* [Información del proyecto, la tarea y el problema](#project-task-and-issue-information)
* [Administración de proyectos y trabajo](#project-and-work-management)
* [Contenido y aprobaciones](#content-and-approvals)

### Información del proyecto, la tarea y el problema

CX Coworker puede proporcionarle información sobre el proyecto, las tareas y los problemas, incluidos los resúmenes y el estado del proyecto.

Consulte las solicitudes de ejemplo para la aprobación de documentos y recursos en las siguientes áreas:

* [Buscar información sobre proyectos, tareas o problemas](#find-information-about-projects-tasks-or-issues)
* [Resumir proyectos, tareas o problemas](#summarize-projects-tasks-or-issues)
* [Mostrar estado del proyecto para proyectos, programas o portafolios](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### Buscar información sobre proyectos, tareas o problemas

* Proyectos
  * Mostrar todos los proyectos activos del equipo de marketing de marca
  * Necesita una lista de proyectos en el portafolio de campañas del cuarto trimestre en la categoría &quot;Digital&quot;.
  * Mostrar los proyectos administrados por usuarios de la compañía de servicios de Creative que son jefes de proyecto.
* Tareas
  * Consígueme todas las tareas asignadas a Joan Harris.
  * Mostrarme tareas en la categoría &quot;Diseño&quot; asignadas al equipo de experiencia de usuario.
  * Necesito tareas asignadas a redactores en el programa de promociones de vacaciones.
* Problemas
  * Mostrarme todos los problemas en el proyecto &quot;Rediseño del sitio web&quot; en la categoría &quot;Técnico&quot;.
  * Consígueme todos los problemas sin resolver notificados por el grupo de control de calidad.
  * Necesito problemas asignados a los desarrolladores de la empresa Global Tech.

#### Resumir proyectos, tareas o problemas

* &quot;Resumir este proyecto&quot;
* &quot;Resumir la última semana de este proyecto&quot;

#### Mostrar estado del proyecto para proyectos, programas o portafolios

>[!NOTE]
>
>Su organización debe estar inscrita en el estado beta del proyecto para utilizar esta función.

* &quot;Mostrar el estado de mis proyectos activos&quot;
* &quot;Muéstrame la salud de este programa&quot;

### Administración de proyectos y trabajo

Puede utilizar CX Coworker para crear y administrar proyectos, incluidas tareas y asignaciones.

Consulte las solicitudes de ejemplo para la administración de proyectos y trabajos en las siguientes áreas:

* [Crear, actualizar o eliminar proyectos](#create-update-or-delete-projects)
* [Identificar la plantilla de proyecto correcta en función de las peticiones de datos del usuario](#identify-the-right-project-template-based-on-user-prompt)
* [Agregar, editar o personalizar tareas en un proyecto](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### Crear, actualizar o eliminar proyectos

Puede crear proyectos desde cero o desde plantillas, actualizarlos y eliminarlos.

* Cree un proyecto en blanco llamado Entorno aislado de innovación del segundo trimestre a partir del 10 de marzo y hasta el 30 de abril. Póngame como el propietario.
* Cree un proyecto llamado Lucent AI Launch - NA con la plantilla Campaña de marketing integrada. Comience el 5 de febrero y establézcalo en Actual.
* Cree un proyecto llamado Rediseño del sitio web: EMEA, a partir del 1 de marzo y hasta el 15 de junio. Es de alta prioridad, propiedad de EMEA Marketing, patrocinado por el vicepresidente de Marketing, presupuestado en 250.000 $ con unas 1.200 horas planificadas, centrado en Europa con el objetivo de mejorar las conversiones.
* Para el proyecto Lucent AI Launch - NA, muévalo al segundo trimestre, cambie el objetivo para impulsar pruebas gratuitas, lleve el final a mediados de abril, aumente el presupuesto a 150 000 dólares y márquelo como urgente.
* Mostrar todos los proyectos de marketing actuales que finalizan en el segundo trimestre y que tienen prioridad alta o urgente, ordenados por fecha de finalización más temprana.

#### Agregar o editar tareas

Puede agregar o editar tareas en un proyecto, así como personalizar la lista de tareas de la plantilla utilizada para crear un proyecto.

* Agregue una nueva tarea denominada Control de calidad de la página de aterrizaje al proyecto y programe su ejecución del 22 al 26 de abril.
* Actualice la tarea Revisión de diseño para que finalice el 18 de abril y asígnela al equipo creativo.
* Elimine la tarea de producción Imprimir recurso del proyecto.
* Mostrarme todas las tareas de este proyecto que no se hayan completado y cuyo inicio está programado para entre el 1 y el 30 de abril.
* Establezca la Aprobación legal como predecesora de la tarea de Campaign Launch.
* Añada una nueva tarea llamada Copia final en polaco programada para del 15 al 16 de abril, mueva la tarea Revisar copia al 10 de abril, elimine la tarea Redondeo de revisión adicional y establezca Copia final en polaco como predecesora de la creación de correo electrónico.
* Durante el flujo de creación del proyecto, intente proporcionar toda la información posible sobre las entregas que, idealmente, deberían convertirse en tareas dentro del proyecto.

#### Crear, actualizar o eliminar asignaciones

Puede crear, actualizar y eliminar asignaciones de usuarios o de funciones.

* Para el proyecto &quot;Diseño de la página de aterrizaje para el lanzamiento del producto&quot;, identifique los roles de trabajo adecuados y las horas planificadas recomendadas para todas las tareas sin asignar actualmente.
* Tengo varias tareas sin asignar, como &quot;Implementar el seguimiento de GA4 para el sitio de campaña&quot;, &quot;Configurar eventos de conversión&quot; y &quot;Validar datos de análisis&quot;. ¿Puede sugerir las funciones del puesto y las horas estimadas adecuadas para cada uno?
* Para las tareas creativas &quot;Crear 3 variantes de banner para anuncios en pantalla de EMEA&quot;, &quot;Aplicar revisiones&quot; y &quot;Exportar recursos finales&quot;, asigne las mejores funciones y estime el esfuerzo necesario para cada tarea.
* En los proyectos &quot;Lanzamiento de productos en el segundo trimestre&quot;, &quot;Rediseño del sitio web - EMEA&quot; y &quot;Campaña de medios de pago - NA&quot;, se identifican todas las tareas sin asignar y se asignan las funciones de trabajo adecuadas con las horas planificadas recomendadas para cada una.

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### Contenido y aprobaciones

CX Coworker puede ayudar a administrar las aprobaciones de documentos y recursos en Workfront.

Tenga en cuenta lo siguiente al trabajar con aprobaciones de documentos y recursos:

* Deben habilitarse las aprobaciones de contenido para su organización para poder utilizar esta funcionalidad en Coworker.
* AI no puede aprobar o rechazar en nombre de los seres humanos. Las decisiones se basan en los usuarios, excepto en el Revisor de IA de Workfront.

  Para obtener más información sobre Workfront AI Reviewer, consulte [Introducción al Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).
* Esta funcionalidad existe en Workfront y no se puede usar para interactuar con herramientas externas o proveedores de documentos.
* Para obtener la mejor experiencia, utilice esta funcionalidad con la experiencia de aprobaciones unificadas.

  Para obtener más información sobre las aprobaciones unificadas, consulte [Resumen de aprobaciones unificadas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

Consulte las solicitudes de ejemplo para la aprobación de documentos y recursos en las siguientes áreas:

* [Adición o eliminación de participantes de aprobación](#add-or-remove-approval-participants)
* [Recordar a las partes interesadas un único recurso pendiente de revisión](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [Agregar, actualizar o aplicar plantillas de aprobación para un solo recurso](#add-update-or-apply-approval-templates-for-a-single-asset)

#### Adición o eliminación de participantes de aprobación

* Agregue a Sarah Chen y Miguel Álvarez como aprobadores en el documento actual.
* Eliminar Jennifer Otto de esta aprobación.
* Elimine a cualquier persona que no haya tomado una decisión de aprobación.
* Añada una nueva etapa al spring-campaign.pdf llamada &quot;Revisión final&quot;.
* Agregue a Mark y Sarah como aprobadores y a Phil como revisor en la segunda etapa de la campaña de invierno.pdf
* Para la campaña de invierno.pdf, dé a la primera etapa un plazo para hoy a las 5 pm, y la revisión final un plazo para mañana a las 5 pm
* Añada una Etapa de comprobación final a fall-campaign.png con una fecha límite para el jueves a las 5 p. m. e incluya a Jim y Pam como aprobadores, también a Oscar como revisor
* Agregue Mark Jones a fall-campaign.png en las fases primera y última como revisor.
* Vamos a obtener una aprobación de varias etapas creado para el fall-campaign.png con 3 etapas, 1 Diseño 2 Redacción y 3 Legal. Solo necesito una decisión para cada etapa. Agregue a Mike, Sally, Jane al diseño, Chris, Richard, Mark a la redacción y Phil, Tom y Sarah a Legal.

#### Recordar a las partes interesadas un único recurso pendiente de revisión

* Envíe un recordatorio a los aprobadores del recurso &quot;Vídeo de campaña de primavera&quot; que no hayan respondido.
* Recuerde a todos los usuarios que no hayan aprobado este recurso &quot;Vídeo de campaña de primavera&quot;.
* ¿Quién no ha tomado una decisión aún sobre el recurso &quot;PDF de directrices de marca&quot;? Recuérdeles.

#### Agregar, actualizar o aplicar plantillas de aprobación para un solo recurso

* Aplique la plantilla de aprobación &quot;Lanzamiento de marketing&quot; al recurso con el nombre &quot;Vídeo de campaña de primavera&quot;.
* Cree una nueva plantilla de aprobación con tres fases: revisión de Creative, legal y aprobación final.
* Añade a Julia Santos y Shane Baker a la etapa 1.
* Edite la plantilla &quot;Lanzamiento de producto&quot; para añadir Elizabeth Peterson a la fase de aprobación final.
* Cree una plantilla denominada &quot;Revisión urgente&quot; con una fase y asígnela a Olivia Kim.
* Actualice la plantilla &quot;Creative Review&quot; eliminando a Rick Kuvec y añadiendo a Karen Sterling a la fase 2.


## CX Coworker en Workfront Planning

### Trabajo con registros de Planning

* [Crear, eliminar, duplicar o restaurar registros](#create-delete-duplicate-or-restore-records)
* [Vincular registros a otros registros](#link-records-to-other-records)
* [Editar, actualizar o agregar un campo a un registro](#edit-update-or-append-a-field-to-a-record)
* [Acceder a historial de cambios de registro](#access-record-change-history)

#### Crear, eliminar, duplicar o restaurar registros

* Cree un nuevo registro de campaña llamado Rebajas de verano de 2026
* Añade un nuevo registro de producto con el nombre Widget Pro y el precio $299
* ¿Puede crear un nuevo registro de posibles clientes para John Smith?
* Elimine el registro de campaña denominado Promoción antigua
* Quitar el registro de prueba que acabo de crear
* ¿Puede eliminar el ID de registro Rc123abc456?
* Duplicación del registro de campaña del primer trimestre
* ¿Puede copiar esta campaña para crear una nueva?
* Haga una copia de la campaña de promoción de vacaciones
* Restaurar la campaña que eliminé accidentalmente
* ¿Puede recuperar el registro del proyecto eliminado?
* Si elimino accidentalmente un registro, ¿puede restaurarlo?

#### Vincular registros a otros registros

* Vinculación del registro de la campaña de verano a la iniciativa del segundo trimestre
* ¿Puede conectar este producto a las campañas de marketing relacionadas?
* Necesito asociar estos tres posibles clientes con el registro de cuenta de empresa

#### Editar, actualizar o agregar un campo a un registro

* Actualice el campo de presupuesto de la campaña de verano a 75 000 $
* ¿Puede cambiar el estado de este registro de proyecto a Completado?
* Agregue John Doe al campo de los integrantes del equipo para esta iniciativa

#### Acceder a historial de cambios de registro

* Mostrar el historial de cambios del registro de campaña de verano
* ¿Puede mostrar quién modificó este proyecto y qué cambió?
* Necesito ver todas las actualizaciones realizadas en este registro en la última semana

### Uso de System Designer en Workfront Planning

* [Creación y configuración de espacios de trabajo](#create-and-configure-workspaces)
* [Definición de tipos de registros](#define-record-types)
* [Campos de diseño y campos de fórmula](#design-fields-and-formula-fields)
* [Creación de vistas personalizadas](#build-custom-views)


#### Creación y configuración de espacios de trabajo

* Cree un nuevo espacio de trabajo de Planning llamado Campañas de marketing 2026
* Actualizar mi espacio de trabajo de planificación de productos para cambiar el color a azul y agregar una descripción
* Mostrar todos los espacios de trabajo de Planning a los que tengo acceso

#### Definición de tipos de registros

* Crear un nuevo tipo de registro llamado Campañas en mi espacio de trabajo de Planning
* Actualice el tipo de registro de Iniciativas para cambiar su icono y descripción
* Mostrarme todos los tipos de registros en mi área de trabajo de planificación de marketing

#### Campos de diseño y campos de fórmula

* Agregar un campo de Presupuesto a mi tipo de registro de Campañas de planificación con tipo de divisa
* Cree un campo de fórmula en Planning que calcule los días restantes hasta la fecha de finalización de la campaña
* Actualizar el campo Prioridad en mi espacio de trabajo de Planning para agregar más opciones desplegables

#### Creación de vistas personalizadas

* Crear una vista de cronología en Planning para ver mi programación de campaña por fechas de inicio y finalización
* Agregar una nueva vista de tabla a Mis iniciativas de planificación que filtre solamente el estado activo
* Duplique la vista Campañas activas de Planning y modifique la ordenación.
