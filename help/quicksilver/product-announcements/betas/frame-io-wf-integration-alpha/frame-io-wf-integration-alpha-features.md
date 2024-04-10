---
content-type: reference
navigation-topic: betas
title: "Integración nativa beta de Adobe Workfront y Frame.io: funciones"
description: Funciones planificadas para la integración beta nativa de Adobe Workfront y Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
exl-id: a1603a06-957b-4d52-89f3-f0cec1a4e02c
source-git-commit: b7a0fe333f0d8f17bc2d6c612d8cff6ee484c935
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 0%

---

# Integración nativa beta de Adobe Workfront y Frame.io: funciones y pruebas

Con esta integración, nuestro objetivo es permitir que los creativos permanezcan en la herramienta de su elección (CC o Frame.io) para llevar a cabo su creación de contenido y revisiones de compañeros, mientras que los administradores de proyectos coordinan el trabajo e inician y supervisan el proceso de revisión formal desde Workfront. Esto se puede lograr utilizando lo mejor de ambas soluciones: las nuevas aprobaciones de documentos de Workfront para administrar las aprobaciones de contenido, junto con las capacidades de revisión de contenido que ofrece Frame.io. De forma conjunta, las nuevas aprobaciones de documentos y Frame.io formarán nuestra nueva experiencia integral de revisión y aprobación de contenido. 

Para obtener más información sobre el funcionamiento de la versión beta y las formas de participación, consulte [Integración beta de Adobe Workfront y Frame.io: información general](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).

>[!NOTE]
>
>Si ha encontrado estas páginas sin que su empresa participe en este programa beta, asegúrese de tratar la información aquí con cuidado y póngase en contacto con su administrador de Workfront o Frame.io para obtener más información.
>

## Vídeo de demostración

>[!VIDEO](https://video.tv.adobe.com/v/3426406/)

## Escenario de prueba básico

Para permitirle probar fácilmente las nuevas funciones del programa beta, hemos creado una nueva cuenta de prueba Frame.io y la hemos conectado a un nuevo grupo llamado `Frame.io testing` en su entorno de vista previa de Workfront o de zona protegida.

Para probar la funcionalidad, inicie sesión en la vista previa de Workfront o en la instancia de zona protegida y realice los siguientes pasos:

1. **Coordinadores:** En Workfront, cree un proyecto con `Frame.io testing` grupo asignado como grupo de proyecto.

1. **Coordinadores:** En Workfront, marque las tareas que requieren trabajo creativo como habilitadas para marcos (en detalles de tareas) y asígnele los elementos creativos (asígnese también si desea probar todo el flujo de trabajo).

>[!NOTE]
>
>Las subtareas no pueden marcarse como Marco habilitado.
>

1. **Coordinadores:** Cargue su informe creativo y cambie el estado del proyecto a Actual.

1. **Creativos:** Busque en sus correos electrónicos una invitación al proyecto Frame.io recién creado

1. **Creativos:** Haga clic en el botón &quot;Unirse al proyecto&quot; del mensaje de correo electrónico de invitación para unirse al proyecto de Frame.io, revise las instrucciones creativas del proyecto e inicie la creación de contenido en la herramienta de Creative Cloud que elija.

1. **Creativos:** Cargue los recursos creados en Frame.io y agréguelos al proyecto de Workfront vinculado seleccionando una de las tareas asignadas con Frame habilitado. Seleccione la opción para marcar la tarea como completada.

1. **Coordinadores:** En Workfront, busque los recursos de Frame.io vinculados en la tarea con marco habilitado y compruebe que el estado de la tarea se haya cambiado a &quot;completada&quot;.

1. **Coordinadores:** Asigne revisores/aprobadores al recurso Frame.io vinculado. Asígnese también como aprobador si desea probar todo el flujo de trabajo. (Para obtener más información sobre la asignación de revisores/aprobadores, consulte [Agregar aprobadores o revisores adicionales a un documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/add-additional-reviewers-or-approvers.md)).

1. **Partes interesadas:** En Workfront, consulte la solicitud de aprobación en Inicio, Detalles del documento o en la notificación por correo electrónico recibida. Abra el recurso en el visor de Frame.io, deje un comentario que contenga comentarios y tome una decisión.

1. **Coordinadores:** En Workfront, vea los comentarios creados por las partes interesadas en la sección Actualizaciones del documento conectado a Frame.io, así como la decisión en la sección Aprobación o en el panel Resumen del documento.

1. **Creativos:** En Frame.io, observe la decisión de aprobación general tomada para sus recursos.

1. **Creativos:** En Frame.io, aplique los cambios solicitados agregando la versión actualizada a la pila de versiones del recurso conectado.

1. **Coordinadores:** En Workfront, asigne aprobadores y revisores a la versión recién cargada y supervise el progreso hasta que llegue a la desactivación.

## Escenario de prueba detallado

Para los participantes que buscan probar funcionalidades adicionales, hemos creado un escenario de prueba más involucrado. Puede descargar una guía para este escenario de prueba detallado aquí: [Tutorial del escenario de prueba detallado de WF + Frame.io](/help/quicksilver/product-announcements/betas/assets/MVP-WF-Frame-Detailed-Walk-Through.pdf).



## Planes de funciones

A continuación se proporciona información sobre los casos de uso principales que queremos abordar y las funciones que tenemos planificadas actualmente para hacerlo. <!--, along with documentation to get you started testing.-->

>[!NOTE]
>
>Viñetas debajo de a **&quot;Posibles mejoras en futuras versiones&quot;** El encabezado de puede incluirse o no en una versión futura, según los comentarios de la versión beta y los planes de desarrollo en evolución.
>

### Los administradores de Workfront pueden configurar una conexión entre los grupos de Workfront y las cuentas de Frame.io

* En Workfront, puede conectar un grupo de Workfront a una cuenta de Frame.io

* Se creará un nuevo equipo de Frame.io dentro de Frame.io que represente al grupo de Workfront conectado (tenga en cuenta que esta función solo se ha habilitado para clientes que utilicen la integración en producción). Los clientes que sigan probando la zona protegida o la vista previa tendrán la conexión configurada por el equipo de Adobe).

**Mejoras potenciales en futuras versiones:**

* Desconectar un grupo de Workfront de una cuenta de Frame.io

* Conectar un grupo de Workfront a un equipo de Frame.io existente

### Los coordinadores de proyectos pueden configurar qué proyectos de Workfront se envían a Frame.io y hacer que los elementos creativos asignados en Workfront se agreguen al proyecto en Frame.io

* Capacidad para marcar proyectos de Workfront como Frame.io habilitado al asignar un grupo conectado a Frame

* Capacidad para alternar tareas dentro de proyectos de Workfront como tareas de marco, lo que a su vez crea carpetas de tareas dentro de Frame.io

* Dado que un proyecto de Workfront tiene un grupo conectado a Frame asignado y al menos una tarea habilitada para Frame, cuando el estado del proyecto de Workfront se establece en Actual, se crea un proyecto conectado correspondiente en Frame, los usuarios asignados de Workfront se añaden al proyecto de Frame y se les envía una notificación por correo electrónico desde Frame.io

   * Los usuarios y equipos asignados a tareas de Workfront con Frame habilitado se añadirán como colaboradores al proyecto Frame.io y se les notificará (durante la creación del proyecto y posteriormente)

* Los documentos (Creative Briefs) añadidos al proyecto y las tareas activadas por Frame se insertarán en el proyecto Frame.io (en la carpeta de trabajo correspondiente) cuando se cree el proyecto (déclencheur: el estado del proyecto se establece en Actual)

   * Le recomendamos que limite la cantidad de documentos añadidos a su proyecto antes de activarlos únicamente para sus informes creativos, a fin de evitar enviar varios documentos innecesarios a Frame.io

   * Los documentos o las tareas que se agreguen después de la sincronización inicial del proyecto no se insertarán en Frame.io, solo los usuarios o equipos

**Mejoras potenciales en futuras versiones:**

* Las tareas con tramas activadas se pueden configurar en plantillas de proyecto

* Las cargas de nuevas versiones a informes creativos se enviarán a Frame

* Sincronización optimizada de proyectos (desconexión de proyectos, resincronización de proyectos y documentos, etc.)

### Dentro de Frame.io, los creativos pueden enviar los recursos creados al proyecto de Workfront para su revisión formal

* Capacidad para conectar un solo recurso Frame.io a un proyecto o tarea de WF. Se creará una referencia de recurso en Workfront

* Las cargas de nuevas versiones dentro de Frame.io crearán automáticamente nuevas versiones de documentos dentro de Workfront en los recursos conectados

* Capacidad para marcar las tareas de Workfront a las que se hace referencia como completadas desde Frame.io

* Si se elimina el documento de Workfront conectado, permanecerá en Frame.io y se podrá volver a conectar con la misma tarea de proyecto o con cualquier otra

**Mejoras potenciales en futuras versiones:**

* Capacidad para enviar varios recursos de Frame.io a Workfront a la vez

* Registro de tiempo de proyectos/tareas de Workfront desde Frame.io

### Los coordinadores de proyectos pueden asignar el proceso de aprobación formal a documentos vinculados desde Frame.io

* Los usuarios y equipos de Workfront se pueden añadir a las nuevas aprobaciones de documentos para los documentos conectados de Frame.io

* Cuando un usuario o equipo deja de compartirse en un documento con Frame habilitado, también perderá su acceso al recurso en Frame.io Viewer

**Mejoras potenciales en futuras versiones:**

* Enviar varios recursos como una sola revisión

* Asignar aprobadores/revisores de forma masiva a documentos de Workfront

### Las partes interesadas pueden realizar su revisión y aprobación dentro del visor de Frame.io

* Se notificará a las partes interesadas y podrán ver el documento conectado a Frame en el visor de Frame.io

* Se puede acceder al Visor de Frame.io desde diferentes ubicaciones dentro de Workfront, por ejemplo, lista de documentos, detalles de documentos o inicio de Workfront

* Capacidad para aprovechar las capacidades existentes de revisión y comentarios proporcionadas por el visor Frame.io, que se sincronizará con el flujo de actualización de Workfront

* Capacidad para tomar una nueva decisión de aprobación de documentos desde el visor de Frame.io
