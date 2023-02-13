---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Información general del proceso de aprobación
description: Puede crear un proceso de aprobación y adjuntarlo a un objeto para asegurarse de que los usuarios designados revisen ciertos cambios antes de que el objeto avance.
author: Courtney
feature: Work Management
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# Información general del proceso de aprobación

Puede crear un proceso de aprobación y adjuntarlo a un objeto para asegurarse de que los usuarios designados revisen ciertos cambios antes de que el objeto avance.

Esta opción está disponible para los siguientes tipos de objetos en Adobe Workfront:

* Elemento de trabajo (proyecto, tarea o problema, plantilla, tarea de plantilla)
* Documento
*  Proof

Para obtener instrucciones sobre la creación de un proceso de aprobación, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Este artículo contiene información general sobre los procesos de aprobación asociados con elementos de trabajo.

## Tipos de procesos de aprobación

Si es administrador de Adobe Workfront o usuario con acceso administrativo a procesos de aprobación, puede crear los siguientes procesos de aprobación para proyectos, tareas y problemas:

* **Un proceso de aprobación global a nivel del sistema**: Los usuarios pueden adjuntarlas a cualquiera de las siguientes opciones:

   * Proyecto, tarea o problema en la sección Aprobaciones
   * En el cuadro Editar proyecto, el área Proceso de Aprobación Predeterminado de Tarea
   * En la sección Detalles de cola o Tema de cola de un proyecto, en las áreas Proceso de aprobación predeterminado . El proyecto debe estar habilitado como cola de solicitudes.

* **Un proceso de aprobación global de nivel de grupo**: Los usuarios pueden adjuntarlas a lo siguiente:

   * Proyecto, tarea o problema perteneciente al grupo asociado al proceso de aprobación en la sección Aprobaciones
   * En el cuadro Editar proyecto, el área del proceso de aprobación predeterminado de la tarea de un proyecto que pertenece al grupo asociado al proceso de aprobación
   * En la sección Detalles de cola o Tema de cola de un proyecto, en las áreas Proceso de aprobación predeterminado . El proyecto debe estar habilitado como cola de solicitud y pertenecer al grupo asociado al proceso de aprobación.

   Para obtener información sobre la creación de procesos de aprobación a nivel de sistema o de grupo, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Un proceso de aprobación de un solo uso**: Para su uso con un solo proyecto, tarea, problema, plantilla o tarea de plantilla. Este tipo de proceso de aprobación solo afecta al objeto asociado a él y no está disponible para asociarse a ningún otro objeto.

   Para obtener información sobre la creación de un proceso de aprobación de un solo uso, consulte [Asociar un proceso de aprobación nuevo o existente al trabajo](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>Este artículo utiliza el término &quot;proceso de aprobación global&quot; para diferenciar del &quot;proceso de aprobación de un solo uso&quot;. Un proceso de aprobación global se puede utilizar repetidamente.
>
>El término &quot;proceso de aprobación global de nivel de grupo&quot; hace referencia a un proceso de aprobación que puede utilizarse repetidamente para elementos y con estados asociados únicamente a un grupo específico.

Para obtener información sobre la creación de un proceso de aprobación a nivel de sistema o de un proceso de aprobación a nivel de grupo, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Consideraciones sobre los procesos de aprobación

* Debe crear el proyecto, la tarea, el problema, la plantilla o la tarea de plantilla antes de poder asociar el proceso de aprobación a ellos.
* Un proceso de aprobación siempre se asocia con dos cosas esenciales:

   * Cada proceso de aprobación corresponde a un determinado estado de elemento de trabajo en el sistema Workfront. Cuando se cambia el estado de un elemento de trabajo, una aprobación adjunta para ese estado requiere que el cambio de estado se confirme antes de que se pueda asignar el nuevo estado al elemento.

      >[!TIP]
      >
      >
      >   
      >   
      >   * Puede asociar una aprobación de nivel de grupo a un estado global o de nivel de grupo.
      >   * No se puede cambiar el estado de un elemento mediante un proceso de aprobación a un estado distinto del asociado al proceso de aprobación.

         >   
         >   
         >     Por ejemplo, si tiene una aprobación de tarea asociada con el estado In Progress, la tarea cambia automáticamente su estado a In Progress cuando se concede la aprobación. No puede cambiar automáticamente su estado a Completado o a cualquier otro estado que no esté asociado con la aprobación.


   * Las entidades asociadas a un proceso de aprobación pueden ser usuarios, funciones de trabajo o equipos. Los usuarios son responsables en última instancia de aceptar o rechazar la aprobación. Puede asignar aprobaciones a usuarios que cumplan una determinada función en el proyecto. Por ejemplo, puede asignar una aprobación a un propietario del proyecto o a un patrocinador. Para obtener más información, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

      Existen los siguientes escenarios:

      * Cuando se asigna una aprobación a funciones de trabajo, cualquier usuario del equipo de proyecto asociado a la función de trabajo puede tomar una decisión sobre la aprobación. La función asociada a la aprobación puede ser su función principal o cualquier otra función.

         Para obtener información acerca del equipo del proyecto, consulte [Información general del equipo del proyecto](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Al asignar una aprobación a un equipo, cualquier miembro de este puede tomar una decisión sobre la aprobación. El equipo asociado con la aprobación puede ser su equipo de origen o cualquiera de sus otros equipos.

         Para obtener información sobre las funciones y los equipos de un usuario, consulte [Edición del perfil de un usuario](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Al crear un elemento de trabajo, no se adjunta automáticamente un proceso de aprobación. Debe adjuntar uno manualmente si desea utilizar uno. Para obtener información sobre cómo adjuntar un proceso de aprobación a un elemento, consulte [Asociar un proceso de aprobación nuevo o existente al trabajo](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* El administrador de Workfront o un usuario con acceso administrativo a los procesos de aprobación pueden crear procesos de aprobación globales a nivel de sistema para su uso en todo el sistema. Un administrador de grupo con acceso administrativo a procesos de aprobación puede crear un proceso de aprobación global de nivel de grupo para que lo utilice únicamente un grupo determinado que administra.
* Si no desea utilizar un proceso de aprobación global predefinido de nivel de sistema o de grupo para un elemento de trabajo, puede crear y adjuntar un proceso de aprobación de un solo uso cuando tenga permisos de gestión al objeto para el que desee adjuntar el proceso de aprobación.

   >[!NOTE]
   Puede utilizar un proceso de aprobación de un solo uso solo una vez para el elemento específico para el que se creó. Puede asociar estados globales, así como estados a nivel de grupo, para procesos de aprobación de un solo uso para proyectos, tareas, problemas, plantillas y tareas de plantilla.

* Al adjuntar un proceso de aprobación de nivel de grupo a un elemento mediante estados personalizados de nivel de grupo, al cambiar el Grupo del proyecto, puede que se cree un conflicto entre los estados de aprobación del grupo anterior y los existentes a nivel del sistema. Considere la posibilidad de eliminar los procesos de aprobación de nivel de grupo en el proyecto, o sus tareas o problemas antes de actualizar el grupo. Para obtener información sobre la creación de procesos de aprobación a nivel de grupo, consulte [Procesos de aprobación a nivel de grupo](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Para obtener información sobre la creación de estados de grupos personalizados, consulte [Crear o editar un estado de grupo](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Para obtener información sobre la actualización del Grupo de un proyecto, consulte [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).

## Flujo de trabajo del proceso de aprobación

En esta sección se explica lo siguiente sobre la aprobación de elementos de trabajo:

* [Cómo dependen los procesos de aprobación de los estados](#how-approval-processes-rely-on-statuses)
* [Uso de un flujo de trabajo habitual en un proceso de aprobación](#how-a-typical-workflow-uses-an-approval-process)

### Cómo dependen los procesos de aprobación de los estados {#how-approval-processes-rely-on-statuses}

Al adjuntar un estado a un proceso de aprobación, se garantiza que el elemento se desplace por los departamentos en el orden correcto.

**Ejemplo:** Puede adjuntar un proceso de aprobación al estado del Departamento de marketing que requiera la aprobación del departamento de finanzas. Luego, cuando alguien cambia el estado de un elemento de trabajo a &quot;Departamento de mercadotecnia&quot;, el elemento no puede moverse a ese departamento hasta que el departamento de finanzas lo cierre.

Para obtener más información sobre los estados de los elementos de trabajo, consulte los siguientes artículos:

* [Acceso a la lista de estados de proyectos del sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Acceso a la lista de estados de tareas del sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Acceda a la lista de estados de problemas del sistema](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Uso de un flujo de trabajo habitual en un proceso de aprobación {#how-a-typical-workflow-uses-an-approval-process}

El siguiente escenario ilustra cómo un proceso de aprobación ayuda a los usuarios a aprobar el trabajo mientras un objeto de Workfront progresa a través de un flujo de trabajo de varios pasos en este orden:

1. El administrador de Workfront o un usuario con acceso administrativo a procesos de aprobación crea un proceso de aprobación para un proyecto, tarea o problema.

   >[!NOTE]
   Puede adjuntar procesos de aprobación de proyectos a una plantilla y procesos de aprobación de tareas a una tarea de plantilla. Después de ello, cuando alguien utiliza la plantilla para crear un proyecto, el proceso de aprobación se convierte en un proceso de aprobación de proyecto o tarea, respectivamente. Un proceso de aprobación de un solo uso adjunto a una plantilla o tarea de plantilla sigue siendo un proceso de aprobación de un solo uso para proyectos y tareas.

1. Un usuario con permiso de gestión del proyecto, la tarea o el problema adjunta el proceso de aprobación al elemento o crea una aprobación de un solo uso para el elemento.
1. Un usuario asignado al elemento de trabajo cambia su estado al estado que inicia el proceso de aprobación y este comienza. (La persona que creó el proceso de aprobación definió la relación entre el estado y el proceso de aprobación).
1. Los aprobadores designados reciben una notificación sobre el proceso de aprobación pendiente y revisan el elemento de trabajo.
1. El proceso de aprobación finaliza después de que los aprobadores designados aprueben todos los pasos del proceso. O, si rechazan un paso, el estado se restablece a un estado predefinido o se crea un problema. (La persona que creó el proceso de aprobación definió cuál de estos pasos automatizados se produce después de un rechazo).

**Ejemplo:** Un equipo de publicidad ha creado un estado llamado Listo para impresión y un proceso de aprobación llamado Firma de Diseñador/Redactor que están asociados a este estado. Este proceso de aprobación está configurado para:

* Requiere la aprobación del diseñador y redactor del equipo
* Iniciar cada vez que alguien cambie el estado de un elemento de trabajo a Listo para imprimir

El propietario de un proyecto de folleto adjunta el proceso de aprobación de firma de Designer/Copywriter al proyecto de folletos.

Cuando alguien en el proyecto cambia el estado a Listo para impresión, el redactor y diseñador reciben notificaciones en las que se les pide que lo aprueben o lo rechacen. Durante el proceso de aprobación, cuando deliberan sobre si aprobarlo o no, el estado de los proyectos aparece como Listo para imprimir - Pendiente de aprobación.

Después de que ambos aprueben el folleto en Workfront, el estado del proyecto cambia a Listo para imprimir.

## Procesos de aprobación de documentos

Las aprobaciones de documentos se utilizan para una aprobación más general. Los comentarios se capturan en formato de chat en la pestaña Actualizaciones . Puede utilizar los botones de aprobación para aprobar, rechazar o aprobar cambios.

Para añadir aprobadores a un documento después de haberlo cargado en Workfront, consulte [Solicitar aprobaciones de documentos](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Procesos de aprobación de prueba

Las aprobaciones de prueba se utilizan para una revisión más profunda y generalmente incluyen flujos de trabajo más complicados. Los comentarios se capturan con herramientas de marcado en el visor de pruebas. Puede utilizar los botones de aprobación para aprobar, rechazar o aprobar cambios.

Para añadir un flujo de trabajo automatizado a una prueba de documento y designar determinados usuarios en el flujo de trabajo como aprobadores de la prueba, consulte [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Configuración de los procesos de aprobación de elementos de trabajo

Como administrador de Workfront, puede configurar la configuración global para los procesos de aprobación de elementos de trabajo en su sistema. Estos ajustes determinan distintas reglas para los procesos de aprobación, como cuánto tiempo se debe permitir que una decisión de aprobación permanezca abierta o cómo se administra la delegación de aprobación en el sistema. Para obtener más información sobre la configuración del proceso de aprobación, consulte [Configuración de la aprobación global](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
