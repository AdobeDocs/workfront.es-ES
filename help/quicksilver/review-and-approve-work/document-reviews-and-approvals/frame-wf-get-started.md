---
product-area: documents
navigation-topic: approvals
title: Introducción a la revisión y aprobación de recursos con Frame.io
description: Obtenga más información acerca del proceso formal de revisión y aprobación en uso de Workfront y Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: d01a26eaa43b264d11faa88c750f48f0ef1272c4
workflow-type: tm+mt
source-wordcount: '1152'
ht-degree: 0%

---

# Introducción a la revisión y aprobación de recursos con Frame.io

El nuevo flujo de trabajo de revisión y aprobación de recursos se basa en una estrecha integración entre Workfront y Frame.io. Esta integración aprovecha al máximo lo que cada producto tiene para ofrecer y lo combina para crear una experiencia que permita a todos los implicados en la creación de contenido trabajar en las herramientas de su elección, mientras tienen acceso a comentarios, archivos y actualizaciones de estado, todos sincronizados en ambos sistemas en tiempo real.

Para obtener más información sobre Frame.io, consulte [Introducción a Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Inicio y planificación del trabajo en Workfront

El administrador de Workfront permite la integración entre Workfront y Frame.io configurando la cuenta predeterminada de Frame.io en el área de Configuración y designando a continuación a los usuarios de Frame.io en Workfront. Esto permite al coordinador planificar e iniciar el trabajo mediante proyectos de Workfront y flujos de trabajo formales de revisión y aprobación.

### Configurar la cuenta predeterminada de Frame.io [!BADGE Muy pronto]{type=Informative}

Los administradores de Workfront inician la integración de Workfront y Frame.io agregando una cuenta predeterminada de Frame.io en el área de Configuración de Workfront. Una vez configurada la cuenta predeterminada de Frame.io, todos los proyectos creados en Workfront tienen un proyecto de reflejo creado en Frame.io.

>[!IMPORTANT]
>
>Esta función estará disponible próximamente. Por ahora, el equipo de Workfront agrega manualmente las cuentas de Frame.io. Póngase en contacto con el representante de su cuenta de Adobe para obtener ayuda.

<!--For more information, see [Configure the [!DNL Workfront] and [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

 in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Habilitar usuarios de Frame.io Ya está disponible

Los usuarios de Workfront que utilicen Frame.io con regularidad deben marcarse como usuarios de Frame.io. Los administradores de Workfront pueden designar a los usuarios de Frame.io en el Perfil de usuario de Workfront.

>[!TIP]
>
>Recomendamos habilitar a los usuarios que trabajan regularmente en herramientas creativas y cargan recursos para su revisión y aprobación como usuarios de Frame.io.

Cuando un usuario está marcado como usuario de Frame.io en Workfront y se añade a un proyecto:

* Se añaden como Collaborator en Frame.io.
* Pueden enviar recursos desde Frame.io a Workfront para su revisión y aprobación formales.
* Pueden ver información en la carpeta de sincronización unidireccional desde Workfront. [!BADGE Muy pronto]{type=Informative}

Para obtener más información, consulte [Configure las variables [!DNL Workfront] y [!DNL Frame.io] integración](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

![](assets/Frame-enabled-user.png)


### Cree un proyecto conectado con Frame.io

Una vez añadida la cuenta predeterminada de Frame.io y designados los usuarios de Frame.io, los coordinadores de proyectos pueden crear proyectos de Workfront conectados con Frame.io. Al crear un proyecto conectado, puede

* **Asignar usuarios de Frame.io a tareas**: Se notifica por correo electrónico a los usuarios habilitados para Frame.io cuando se les asigna una tarea de Workfront, lo que indica que hay trabajo por completar.
* **Uso compartido del proyecto con usuarios de Frame.io**: Cuando se comparte un proyecto con usuarios con Frame.io habilitado, estos tienen acceso al proyecto tanto dentro de Workfront como dentro de Frame.io.
* **Comparta materiales creativos con Frame.io**: los coordinadores de proyectos pueden enviar instrucciones y materiales desde Workfront directamente al usuario creativo en Frame.io mediante una carpeta de proyecto de sincronización unidireccional. [!BADGE Muy pronto]{type=Informative}
* **Seguimiento del progreso de tareas**: los creativos pueden enviar recursos finalizados y marcar las tareas como completadas, todo sin salir de Frame.io.

Para obtener más información, consulte [Cree un proyecto conectado con Frame.io](/help/quicksilver/manage-work/projects/create-projects/create-frame-connected-project.md).


## Creación y colaboración de contenido en Frame.io

Los creativos pueden permanecer en sus herramientas de elección y tener la libertad de crear, iterar y realizar revisiones de compañeros dentro de Frame.io.

Cuando se agrega un elemento creativo a un proyecto conectado, puede hacer lo siguiente en Frame.io:

<!--* Access instructions from the project coordinator -->
* Realización de revisiones informales entre iguales
* Enviar los recursos finalizados a Workfront para su revisión y aprobación formales
* Cambiar el estado de una tarea o marcarla como completada
* Cargue nuevas versiones y vuelva a enviarlas para su aprobación <!--do they have to send to frame.io again?-->

Para obtener más información sobre Frame.io, consulte [Se me ha invitado a colaborar en un proyecto](https://support.frame.io/en/articles/11125-i-ve-been-invited-to-collaborate-on-a-project).

## Revisión y aprobación de recursos

Una vez que un creativo envía un recurso terminado a Workfront desde Frame.io, el coordinador del proyecto puede iniciar el proceso formal de revisión y aprobación en Workfront.

Una vez creado el flujo de trabajo de aprobación, los revisores y aprobadores vuelven a Frame.io para agregar comentarios y marcar el recurso. También pueden tomar la decisión de aprobación en el visor de Frame.io.

### Iniciar revisiones y aprobaciones formales en Workfront

Los coordinadores de proyectos pueden crear aprobaciones y revisiones únicas o plantillas de aprobación reutilizables. Toda la actividad de revisión y aprobación de Frame.io también se registra en Workfront.

Los coordinadores de proyecto tienen la opción de asignar revisores, aprobadores o una combinación de ambos:

* **Revisores** Puede agregar comentarios y marcar recursos. Una vez finalizada, puede marcar su revisión como completada. No es necesario marcar la revisión como completada para que el recurso avance en el proceso de aprobación.
* **Aprobadores** Puede agregar comentarios y marcar recursos. Deben tomar la decisión de adelantar el proceso de aprobación.


#### Creación de un flujo de trabajo de revisión y aprobación

Los revisores y aprobadores se pueden añadir a un flujo de trabajo de aprobación de un solo uso o a una plantilla de aprobación reutilizable:

* **Aprobaciones de un solo uso**: en el proyecto o la tarea donde reside el recurso, el coordinador del proyecto puede asignar revisores y aprobadores y establecer un plazo de finalización. Se recuerda a los revisores y aprobadores por correo electrónico 72 y 24 horas antes del plazo, así como en el propio plazo.

  Para obtener más información, consulte * [Crear una solicitud de revisión o aprobación para un recurso Frame.io](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-request-for-frame-asset.md).

* **Plantillas de aprobación**: en el área Configuración de Workfront, los coordinadores de proyectos pueden crear plantillas de aprobación reutilizables. En una plantilla, los usuarios pueden agregar revisores y aprobadores, y especificar un periodo de finalización. Cuando la plantilla de aprobación se aplica a un recurso, la fecha límite se calcula a partir del periodo de tiempo especificado.

  Una vez creada una plantilla, se puede aplicar a los recursos enviados desde Frame.io para iniciar el proceso formal de revisión y aprobación en Workfront.

  Para obtener más información, consulte [Crear una plantilla de aprobación](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)


![](assets/assign-template.png)


#### Acceso al visor de Frame.io

Los usuarios pueden acceder al visor Frame.io de las siguientes maneras:

* Notificaciones por correo electrónico de Workfront
* El widget Esperando mi aprobación en la nueva área de inicio de Workfront
  ![](assets/awaiting-my-approval.png)

>[!NOTE]
>
>Se notifica a los usuarios externos de Workfront por correo electrónico y se les pedirá que creen un inicio de sesión de Frame.io para revisar y aprobar los recursos.

#### Agregar comentarios y marcar recursos

Todos los comentarios realizados en el visor Frame.io también se registran en la pestaña Actualizaciones de Workfront. Las respuestas realizadas en Workfront no aparecen en Frame.io. Si los comentarios están marcados como &quot;Solo equipo&quot; en el visor de Frame.io, no aparecerán en la pestaña Actualizaciones de Workfront.

#### Tomar una decisión

Una vez completada toda la actividad de revisión, los aprobadores deben tomar una de las siguientes decisiones:

* **Aprobar**: el recurso no necesita cambios y está listo para usarse.
* **Aprobar con cambios**: el recurso necesita cambios y está listo para usarlo una vez que se realicen. No se requiere una aprobación adicional.
* **Necesita trabajo**: el recurso necesita cambios y no está listo para usarse. Una vez realizados los cambios especificados, el recurso debe cargarse como una nueva versión y pasar por otra ronda de aprobaciones. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Los revisores pueden marcar su revisión como completada dentro del visor de Frame.io, pero esto no es necesario para que el recurso avance en el proceso de aprobación.

Para obtener más información sobre las decisiones en Workfront, consulte [Resumen del estado de decisión del documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![](assets/frame-viewer-and-decision.png)


<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Seguimiento de métricas de revisión y aprobación

Los coordinadores de proyecto pueden monitorizar el progreso de todas las aprobaciones en vuelo en el área de inicio de Workfront con el siguiente widget:

* **Todas las aprobaciones**: Muestra dos gráficos con información sobre el tiempo medio de aprobación y las decisiones, así como vistas de lista de aprobaciones pendientes y vencidas.
  ![](assets/all-approvals.png)