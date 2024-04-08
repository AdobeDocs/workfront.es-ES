---
product-area: documents
navigation-topic: approvals
title: Resumen de revisión y aprobación de recursos
description: Obtenga más información acerca del proceso formal de revisión y aprobación en Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 959bd3cab0de8b76c94fad1be5b6b2b8b7ae904b
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Resumen de revisión y aprobación de recursos

El nuevo flujo de trabajo de revisión y aprobación de recursos se basa en una estrecha integración entre Workfront y Frame.io. Esta integración aprovecha al máximo lo que cada producto tiene para ofrecer y lo combina para crear una experiencia que permita a todas las personas involucradas en la creación de contenido trabajar en las herramientas de su elección, mientras tienen acceso a comentarios, archivos y actualizaciones de estado sincronizadas entre ambos sistemas en tiempo real.

Para obtener más información sobre Frame.io, consulte [Introducción a Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Inicio y planificación del trabajo en Workfront

El administrador de Workfront permite la integración entre Workfront y Frame.io configurando la cuenta predeterminada de Frame.io en el área de Configuración y designando a continuación a los usuarios de Frame.io en Workfront. Esto permite al coordinador planificar e iniciar el trabajo mediante proyectos de Workfront y flujos de trabajo formales de revisión y aprobación.

### Configuración de una cuenta predeterminada de Frame.io

Los administradores de Workfront inician la integración de Workfront y Frame.io agregando una cuenta predeterminada de Frame.io en el área de Configuración de Workfront. Una vez configurada una cuenta predeterminada de Frame.io, todos los proyectos creados en Workfront tienen un proyecto de reflejo creado en Frame.io.

Para obtener más información, consulte [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Habilitar usuarios de Frame.io

Los usuarios de Workfront que utilicen Frame.io con regularidad deben marcarse como usuarios de Frame.io. Los administradores de Workfront pueden designar a los usuarios de Frame.io en el Perfil de usuario de Workfront.

Cuando un usuario está marcado como usuario de Frame.io en Workfront y se añade a un proyecto,

* Se añaden como Collaborator en Frame.io
* Pueden enviar recursos desde Frame.io a Workfront para su revisión y aprobación formales
* Pueden ver información en la carpeta de sincronización unidireccional desde Workfront

>[!TIP]
>
>Recomendamos habilitar a los usuarios que trabajan regularmente en herramientas creativas y cargan recursos para su revisión y aprobación como usuarios de Frame.io.

Para obtener más información, consulte [].

![](assets/Frame-enabled-user.png)


### Cree un proyecto conectado con Frame.io

Una vez añadida la cuenta predeterminada de Frame.io y designados los usuarios de Frame.io, los coordinadores de proyectos pueden crear proyectos de Workfront conectados con Frame.io. Al crear un proyecto conectado, puede

* **Asignar usuarios de Frame.io a tareas**: Se notifica por correo electrónico a los usuarios habilitados para Frame.io cuando se les asigna una tarea, indicando que hay trabajo por completar.
* **Uso compartido del proyecto con usuarios de Frame.io**: Los proyectos compartidos con usuarios con Frame.io habilitado les conceden acceso al proyecto dentro de Frame.io.
* **Comparta materiales creativos con Frame.io**: puede enviar instrucciones y materiales desde Workfront directamente al usuario creativo en Frame.io utilizando una carpeta de proyecto de sincronización unidireccional.
* **Seguimiento del progreso de tareas**: los creativos pueden enviar los recursos finalizados y marcar las tareas como completadas sin salir de Frame.io.

Para obtener más información, consulte [].

<!--Preassign approval templates to tasks coming in the future-->


## Creación y colaboración de contenido en Frame.io

Los creativos pueden permanecer en sus herramientas de elección y tener la libertad de crear, iterar y realizar revisiones de compañeros dentro de Frame.io.

Cuando se agrega un elemento creativo a un proyecto conectado, puede hacer lo siguiente sin salir de Frame.io:

* Instrucciones de acceso del coordinador del proyecto
* Realización de revisiones informales entre iguales
* Enviar los recursos finalizados a Workfront para su revisión y aprobación formales
* Cambiar el estado de una tarea o marcarla como completada
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Para obtener más información sobre la revisión de recursos en Frame.io, consulte

## Revisión y aprobación de recursos

Una vez que un creativo envía un recurso terminado a Workfront desde Frame.io, el coordinador del proyecto puede iniciar el proceso formal de revisión y aprobación en Workfront.

Una vez creada la aprobación, los usuarios vuelven a Frame.io para realizar comentarios sobre el recurso y registrarlo. También pueden tomar la decisión de aprobación en el visor Frame.io.

### Iniciar revisiones y aprobaciones formales en Workfront

Los coordinadores de proyectos pueden crear revisiones y aprobaciones únicas o plantillas de aprobación reutilizables en el área de Configuración de Workfront. Toda la actividad de revisión y aprobación realizada en Frame.io también se registra en Workfront.

#### Agregar revisores y aprobadores

Los coordinadores de proyecto tienen la opción de asignar revisores, aprobadores o una combinación de ambos:

* **Revisores** puede realizar comentarios en los recursos y marcarlos. Una vez finalizada, puede marcar su revisión como completada. <!--example of when to add reviewers-->
* **Aprobadores** puede realizar comentarios en los recursos y marcarlos. Deben tomar la decisión de adelantar el proceso de aprobación.


#### Creación de un flujo de trabajo de revisión y aprobación

Los revisores y aprobadores pueden agregarse a un flujo de trabajo de aprobación de un solo uso o a una plantilla de aprobación:

<!--can also assign teams and set deadline-->
Correo electrónico: los correos electrónicos de fecha límite 72, 24 y dentro del plazo.

* **Aprobaciones de un solo uso**: Establecer plazos de aprobación

* **Plantillas de aprobación**
En el área Configuración de Workfront, los usuarios con una licencia Estándar pueden crear plantillas de aprobación reutilizables. Dentro de una plantilla, los usuarios pueden especificar un periodo de tiempo y agregar revisores y aprobadores. <!--do we want to mention any upcoming plans here? -->

  Una vez creada una plantilla, se puede aplicar a los recursos enviados desde Frame.io para iniciar el proceso formal de revisión y aprobación en Workfront.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Cargue un recurso de Workfront y envíelo a un marco para su revisión y aprobación. ¿Próximamente?

### Aprobar recursos en Frame.io

Las partes interesadas pueden revisar y aprobar los recursos conectados con el visor Frame.io.

#### Acceso al visor de Frame.io

Los usuarios pueden acceder al visor Frame.io de las siguientes maneras:

* El widget Esperando mi aprobación en la nueva área de inicio de Workfront
* Notificaciones por correo electrónico de Workfront.

Se solicitará a los usuarios externos de Workfront que creen un inicio de sesión de Frame.io para revisar y aprobar los recursos.

#### Comentario y marcado de recursos

Todos los comentarios realizados en el visor Frame.io también se registran en la pestaña Workfront Update. Las respuestas realizadas en Workfront no aparecen en Frame.io. Los comentarios marcados como Solo equipo no aparecerán en la pestaña Actualizaciones de Workfront.

#### Tomar una decisión

Los aprobadores deben tomar una de las siguientes decisiones:

* Aprobar: esto
* Aprobar con cambios
* Necesita trabajo

Los revisores pueden marcar su revisión como completada dentro de los visores de Frame.io.

<!-- include screenshot from frame.io-->



<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Seguimiento de métricas de revisión y aprobación

¿Widgets en el informe de velocidad de aprobación de inicio?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Ejemplo de flujo de trabajo de aprobación de recursos

¿intro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
