---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Herramientas del servidor MCP de Adobe Workfront
description: Lista de referencia de las herramientas disponibles a través del servidor MCP de Adobe Workfront, agrupadas por área de Workfront.
author: Courtney
feature: Get Started with Workfront
source-git-commit: a2b2da49e9aba808dc7567bd5a7f29adeb381c1d
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 9%

---


# Herramientas del servidor MCP de Adobe Workfront

Este artículo enumera las herramientas que expone el servidor MCP de [!DNL Adobe Workfront] a una plataforma independiente de IA conectada. La plataforma llama a estas herramientas en su nombre cuando le pide que busque, cree, actualice o elimine elementos de Workfront.

Para obtener información sobre cómo usar estas herramientas a través de una plataforma agéntica de IA, consulte [Usar el servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md). Para obtener información sobre cómo configurar la conexión, consulte [Configuración del servidor MCP de Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

>[!IMPORTANT]
>
>La plataforma agéntica de IA actúa en Workfront con la cuenta de Workfront, el nivel de acceso y los permisos de objeto. Una herramienta solo funciona si tiene el acceso correspondiente en Workfront. Adobe no se responsabiliza por los cambios que realice la plataforma agéntica de IA en sus datos de Workfront.


## Leer y escribir acciones

Cada herramienta de las tablas siguientes se clasifica en la columna Acción como una acción Leer o Escribir:

* **Leer**: recupera información de Workfront sin cambiar los datos. Por ejemplo, buscar un proyecto, enumerar documentos u obtener los detalles de un registro.
* **Escribir**: crea, actualiza o elimina datos de Workfront. Por ejemplo, crear un proyecto, actualizar un registro o eliminar una vista.

El administrador de Workfront controla qué categorías de herramientas puede utilizar la plataforma agéntica de IA mediante dos toggles en Preferencias del sistema:

* **Herramientas MCP de solo lectura** (habilitadas de forma predeterminada)
* **Escribir herramientas MCP** (deshabilitada de forma predeterminada)

Si la plataforma agéntica de IA puede encontrar elementos de Workfront pero no puede crearlos, actualizarlos o eliminarlos, pídale al administrador de Workfront que habilite las acciones de escritura. Para obtener más información, consulte [Requisitos previos de administración](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#admin-prerequisites) en *Configuración del servidor MCP de Adobe Workfront*.

## Herramientas de aprobaciones

### Documentos

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Buscar versión del documento por nombre | `approvals_find_document_version_by_name` | Busca el identificador de la versión actual de un documento por nombre de archivo. Admite coincidencias parciales. | Leer |
| Obtener documento por ID de versión | `approvals_get_document_by_version_id` | Obtiene detalles del documento (nombre, tamaño, fecha de carga, cargador) para un ID de versión de documento conocido. | Leer |
| Obtener documentos por proyecto | `approvals_get_documents_by_project` | Enumera los documentos de un proyecto de Workfront, con el ID de versión actual de cada documento. | Leer |
| Resolver ámbito del documento | `approvals_resolve_document_scope` | Expande un proyecto o carpeta a la lista de identificadores de versión de documento que contiene. Admite ámbitos de proyecto, carpeta y carpeta por nombre. | Leer |

<!--
| List AEM-linked folders* | `approvals_list_aem_linked_folders` | Lists Workfront document folders that are linked to Adobe Experience Manager. | Read |
| Send documents to AEM folder* | `approvals_send_documents_to_aem_folder` | Moves one or more Workfront documents to an AEM-linked folder. | Write |

*You must have a native [!DNL Adobe Experience Manager] integration configured in your Workfront instance to use these tools. For more information, see [Overview of Adobe Experience Manager Assets integrations](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/aem-asset-integrations.md).


*Sending documents to an AEM folder is not yet supported for projects on Adobe cloud storage. Support is expected in a future release.

-->

### Flujos de trabajo de aprobación

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Obtener información del flujo de trabajo de aprobación | `approvals_get_approval_info` | Devuelve el flujo de trabajo de aprobación actual (fases, participantes, estado) de una versión de documento. | Leer |
| Crear o actualizar flujo de trabajo de aprobación | `approvals_create_or_update_approval_workflow` | Crea o actualiza las fases del flujo de trabajo de aprobación para una versión de documento. Admite dependencias de escenario lineales y paralelas (gráfico). | Escritura |
| Crear aprobación a partir de plantilla | `approvals_create_approval_from_template` | Crea un flujo de trabajo de aprobación en un documento utilizando una plantilla existente. | Escritura |
| Eliminar fase de aprobación | `approvals_delete_approval_stage` | Elimina una sola etapa de un flujo de trabajo de aprobación por nombre o posición. Solo se pueden eliminar las fases no iniciadas. | Escritura |

<!--
| Request document approval | `approvals_request_document_approval` | Opens a guided form for requesting approval on a document version (title, approvers/reviewers, optional due date and message). | Write |
-->

### Recordatorios

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Enviar recordatorio a los participantes | `approvals_send_reminder_to_participants` | Envía correos electrónicos de recordatorio a participantes específicos en una fase de aprobación. Solo funciona para fases iniciadas, no completadas y no bloqueadas. | Escritura |
| Enviar recordatorio a los participantes indecisos | `approvals_send_reminder_to_undecided` | Envía correos electrónicos de recordatorio a todos los participantes indecisos (notificados, abiertos o comentados) en una fase de aprobación. | Escritura |

### Plantillas de aprobación

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Enumerar plantillas de aprobación | `approvals_list_templates` | Muestra las plantillas de aprobación disponibles en esta instancia de Workfront. Admite el filtrado por creador, participante y la ordenación por uso. | Leer |
| Buscar plantilla por nombre | `approvals_search_template_by_name` | Busca plantillas de aprobación por nombre (coincidencia parcial sin distinción de mayúsculas y minúsculas). | Leer |
| Crear plantilla de aprobación | `approvals_create_template` | Crea una nueva plantilla de aprobación con dependencias de fase lineales o basadas en gráficos. | Escritura |
| Actualizar plantilla de aprobación | `approvals_update_template` | Actualiza una plantilla existente con modificaciones estructuradas (añadir o quitar participantes, cambiar el nombre de las fases, establecer plazos, etc.). | Escritura |

### Búsquedas y usuarios

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Obtener usuario actual | `approvals_get_current_user` | Devuelve la identidad de Workfront del usuario que realiza la llamada, incluidos el nombre, el ID de usuario, el nombre del equipo de inicio y el ID del equipo de inicio. | Leer |
| Buscar usuario por nombre | `approvals_find_user_by_name` | Busca el ID de un usuario de Workfront por nombre (coincidencia parcial o parcial). Devuelve el nombre, el ID, el correo electrónico, el título y la dirección URL del avatar. | Leer |
| Buscar equipo por nombre | `approvals_find_team_by_name` | Busca el ID de un equipo de Workfront por nombre (coincidencia parcial o parcial). | Leer |
| Buscar proyecto por nombre | `approvals_find_project_by_name` | Busca proyectos de Workfront por coincidencia de nombre parcial en todo el sistema. | Leer |
| Obtener proyectos por propietario | `approvals_get_projects_by_owner` | Enumera proyectos de Workfront en los que el usuario que realiza la llamada es el propietario. | Leer |
| Obtener región de Adobe | `approvals_get_adobe_region` | Devuelve el nombre de Adobe de una región de proveedor de la nube. | Leer |

## Herramientas de planificación

### Espacios de trabajo

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Obtener espacio de trabajo | `planning_get_workspace` | Recupera todos los detalles de un espacio de trabajo por ID o alias. | Leer |
| Obtener lista de Workspace | `planning_get_workspace_list` | Enumera todos los espacios de trabajo disponibles con paginación basada en cursor. | Leer |
| Crear espacio de trabajo | `planning_create_workspace` | Crea un nuevo espacio de trabajo vacío para organizar los tipos de registro, los campos y los datos. | Escritura |
| Crear espacio de trabajo desde plantilla | `planning_create_workspace_from_template` | Crea un nuevo espacio de trabajo rellenado previamente mediante una plantilla existente. | Escritura |
| Actualizar Workspace | `planning_update_workspace` | Actualiza parcialmente un espacio de trabajo: nombre, descripción, icono, secciones o propietario. | Escritura |
| Eliminar espacio de trabajo | `planning_delete_workspace` | Elimina permanentemente un espacio de trabajo y todos sus datos. | Escritura |
| Convertir espacio de trabajo en plantilla | `planning_convert_workspace_to_template` | Guarda un espacio de trabajo existente como plantilla reutilizable (requiere administrador). | Escritura |
| Obtener uso compartido de Workspace | `planning_get_workspace_sharing` | Devuelve la configuración actual de uso compartido y permisos para un espacio de trabajo. | Leer |
| Modificar uso compartido de Workspace | `planning_modify_workspace_sharing` | Actualiza quién tiene acceso a un espacio de trabajo y con qué nivel de permisos. | Escritura |

### Tipos de registro

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Obtener tipo de registro | `planning_get_record_type` | Obtiene todos los detalles de un tipo de registro, incluidos sus campos y vistas. | Leer |
| Crear tipos de registro | `planning_create_record_types` | Crea uno o varios tipos de registros en una sección de Workspace. | Escritura |
| Actualizar tipo de registro | `planning_update_record_type` | Actualiza parcialmente el nombre, la descripción, el icono o el color de un tipo de registro. | Escritura |
| Eliminar tipo de registro | `planning_delete_record_type` | Elimina permanentemente un tipo de registro y todos sus registros, campos y vistas. | Escritura |
| Enumerar tipos de registros globales | `planning_list_global_record_types` | Enumera todos los tipos de registros definidos de forma centralizada (globales) visibles para el usuario actual. | Leer |
| Enumerar tipos de registros globales agregables | `planning_list_addable_global_record_types` | Enumera los tipos de registros globales que se pueden agregar a un espacio de trabajo específico. | Leer |
| Añadir tipo de registro global al espacio de trabajo | `planning_add_global_record_type_to_workspace` | Vincula un tipo de registro global a un espacio de trabajo especificado. | Escritura |
| Quitar el tipo de registro global de Workspace | `planning_remove_global_record_type_from_workspace` | Desvincula un tipo de registro global de un espacio de trabajo; elimina todos sus registros de ese espacio de trabajo. | Escritura |
| Obtener espacios de trabajo de registro externos | `planning_get_external_record_workspaces` | Busca qué espacios de trabajo y tipos de registros están conectados a un registro externo específico. | Leer |
| Obtener el uso compartido del tipo de registro | `planning_get_record_type_sharing` | Devuelve el uso compartido y los permisos para un tipo de registro específico. | Leer |
| Modificar uso compartido de tipo de registro | `planning_modify_record_type_sharing` | Actualiza quién puede tener acceso a un tipo de registro y en qué nivel de permisos. | Escritura |

### Registros

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Obtener registro | `planning_get_record` | Recupera todos los detalles de un único registro por ID. | Leer |
| Búsqueda de registros | `planning_search_records` | Busca y filtra registros dentro de un tipo de registro. | Leer |
| Acciones de registro masivo | `planning_bulk_record_actions` | Crea, actualiza, elimina o restaura varios registros en una sola solicitud. | Escritura |
| Crear registro de conexión | `planning_create_connection_record` | Crea un nuevo registro en un sistema externo conectado (por ejemplo, un proyecto de Workfront). | Escritura |
| Actualizar orden de registros | `planning_update_records_order` | Cambia el orden de visualización de los registros dentro de un tipo de registro. | Escritura |
| Obtener registro de cambios | `planning_get_record_change_log` | Devuelve el historial de edición a nivel de campo de un registro. | Leer |
| Obtener uso compartido de registros | `planning_get_record_sharing` | Devuelve la configuración de uso compartido de un registro específico. | Leer |
| Modificación del uso compartido de registros | `planning_modify_records_sharing` | Actualiza quién puede tener acceso a uno o más registros y con qué nivel de permisos. | Escritura |

### Campos

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Obtener campo | `planning_get_field` | Recupera los detalles completos y el esquema de valores de un campo por ID. | Leer |
| Crear campos | `planning_create_fields` | Agrega uno o más campos (columnas) a un tipo de registro. | Escritura |
| Actualizar campo | `planning_update_field` | Actualiza parcialmente el nombre, descripción, opciones o configuración de un campo. | Escritura |
| Eliminar campo | `planning_delete_field` | Quita permanentemente un campo y todos sus datos de un tipo de registro. | Escritura |

### Vistas

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Obtener vista | `planning_get_view` | Devuelve los detalles completos de una vista por ID. | Leer |
| Crear vista | `planning_create_view` | Crea una nueva vista de tabla, cronología o calendario para un tipo de registro. | Escritura |
| Actualizar vista | `planning_update_view` | Actualiza parcialmente la configuración, los filtros o la ordenación de una vista existente. | Escritura |
| Eliminar vista | `planning_delete_view` | Elimina permanentemente una vista (los registros no se ven afectados). | Escritura |
| Obtener uso compartido de vistas | `planning_get_view_sharing` | Devuelve la configuración de uso compartido de una vista específica. | Leer |
| Modificar uso compartido de vistas | `planning_modify_view_sharing` | Actualiza quién puede acceder a una vista y con qué nivel de permisos. | Escritura |

### Plantillas

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Obtener lista de plantillas | `planning_get_template_list` | Muestra todas las plantillas de Workspace disponibles con información de resumen. | Leer |
| Obtener plantilla | `planning_get_template` | Recupera todos los detalles de una plantilla específica por ID. | Leer |

### Búsqueda y utilidades

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Búsqueda de recursos | `planning_search_resources` | Busca por nombre en espacios de trabajo, tipos de registro y vistas. | Leer |
| Buscar datos compartidos | `planning_search_sharing_data` | Busca usuarios, grupos, equipos, funciones y empresas por nombre para compartir y permisos. | Leer |
| Buscar usuarios | `planning_search_users` | Busca usuarios compatibles con la paginación. | Leer |

## Herramientas de flujo de trabajo

Las herramientas de flujo de trabajo son las acciones de uso general que utiliza la plataforma agéntica de IA para trabajar con cualquier objeto de Workfront: proyectos, tareas, problemas, horas, asignaciones, programas, portafolios, etc.

| Título | Nombre de herramienta | Qué hace | Acción |
|---|---|---|---|
| Buscar objetos | `workflow_search_any_object` | Busca objetos de Workfront con parámetros de filtro, orden y paginación flexibles. | Leer |
| Crear objeto | `workflow_create_any_object` | Crea un nuevo objeto de Workfront, como un proyecto, una tarea, un problema, una hora, una asignación, un programa o un portafolio. | Escritura |
| Actualizar objeto | `workflow_update_any_object` | Actualiza los campos de un objeto de Workfront existente. | Escritura |
| Eliminar objeto | `workflow_delete_any_object` | Elimina un objeto de Workfront por ID. Requiere confirmación explícita del usuario antes de realizar la acción. | Escritura |
| Resolver nombres de campo | `workflow_resolve_field_names_any_object` | Convierte los nombres de campo o las etiquetas proporcionados por el usuario en los nombres de campo de la API de Workfront subyacentes para que la plataforma agéntica de IA pueda crear solicitudes precisas. | Leer |

## Actualización de las herramientas

Cuando Adobe lanza una nueva versión del servidor MCP de Workfront, la plataforma agéntica de IA utiliza el conjunto de herramientas actualizado automáticamente. No es necesario que vuelva a conectarse o cambie nada de su lado.



## Herramientas adicionales próximamente

Estamos trabajando para agregar las siguientes herramientas al servidor MCP de Workfront en el futuro:

* Comentarios
* Tableros

