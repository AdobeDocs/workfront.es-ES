---
content-type: reference
navigation-topic: betas
title: "Integración nativa alfa de Adobe Workfront y Frame.io: funciones"
description: Funciones planificadas para la integración nativa alfa de Adobe Workfront y Frame.io
author: Nolan
feature: Product Announcements
hide: true
hidefromtoc: true
source-git-commit: 0ad33f377086f71699c550e2300731056a834e72
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Integración nativa alfa de Adobe Workfront y Frame.io: funciones

## Casos de uso y pruebas de funciones

Con esta integración, nuestro objetivo es permitir que los creativos permanezcan en la herramienta de su elección (CC o Frame.io) para llevar a cabo su creación de contenido y revisiones de compañeros, mientras que los administradores de proyectos coordinan el trabajo e inician y supervisan el proceso de revisión formal desde Workfront. Esto se puede lograr utilizando lo mejor de ambas soluciones: las nuevas aprobaciones de documentos de Workfront para administrar las aprobaciones de contenido, junto con las capacidades de revisión de contenido que ofrece Frame.io. De forma conjunta, las nuevas aprobaciones de documentos y Frame.io formarán nuestra nueva experiencia integral de revisión y aprobación de contenido. 

Para obtener más información sobre cómo funcionará el alfa y las formas en que puede participar, consulte [Integración alfa de Adobe Workfront y Frame.io: información general](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md)


>[!NOTE]
>
>Si ha encontrado estas páginas sin que su empresa participe en este programa alfa, asegúrese de tratar la información aquí con cuidado y póngase en contacto con su administrador de Workfront o Frame.io para obtener más información.

<!--Initial setup and basic test scenario 

As part of the alpha program, we've provisioned a new test Frame.io account for you and connected it to a new group "Frame.io alpha testing" in your existing Workfront Preview or Sandbox environment. To test the delivered functionality please log in to your Workfront Preview or Sandbox instance and  perform the following steps: 

Coordinators: Within Workfront, create a project with the "Frame.io alpha testing" group assigned as project group 

Coordinators: Within Workfront, assign your creatives to the project or Frame enabled tasks and change the project status to "Current" 

Creatives: Check your emails for an invite to the newly created Frame.io project 

Creatives: Click on the "Join project" button within the invitation email to join the Frame.io project, review the creative brief within the project and start your content creation within your CC tool of choice 

Creatives: Upload your created assets to Frame.io and add them to the linked Workfront project (or assigned Frame enabled tasks)  

Coordinators: Within Workfront, see the linked Frame.io assets in your project and assign reviewers / approvers (new document approvals: More help on this feature) 

Stakeholders: Withing Workfront, view your approval request in Workfront Home or Document Details and review the Frame connected document in the Frame.io Viewer. Leave a comment feedback 

Coordinators: Within Workfront, view the stakeholder created comments within the Updates section of the Frame.io connected document in Workfront 

Stakeholders: Make a decision from within the Frame.io Viewer 

Creatives: Within Frame.io, notice the overall approval decision made for your assets 

Creatives: Within Frame.io, Apply the requested changes by adding the updated version to the version stack of the connected asset 

Coordinators: Within Workfront, assign approvers / reviewers to the new version upload and monitor the progress until it reaches sign-off-->

## Planes de funciones

A continuación se proporciona información sobre los casos de uso principales que queremos abordar y las funciones que tenemos planificadas actualmente para hacerlo. <!--, along with documentation to get you started testing.-->


### Los administradores de Workfront pueden configurar una conexión entre los grupos de Workfront y las cuentas de Frame.io

* _En Workfront, puede conectar un grupo de Workfront a una cuenta de Frame.io_

* Se creará un nuevo equipo de Frame.io dentro de Frame.io que represente al grupo de Workfront conectado

**Mejoras potenciales en futuras versiones:**

* Desconectar un grupo de Workfront de una cuenta de Frame.io

* Conectar un grupo de Workfront a un equipo de Frame.io existente

### Los coordinadores de proyectos pueden configurar qué proyectos de Workfront se envían a Frame.io y hacer que los elementos creativos asignados en Workfront se agreguen al proyecto en Frame.io

* Capacidad para marcar proyectos de Workfront como Frame.io habilitado al asignar un grupo conectado a Frame

* _Mejora: Capacidad para alternar tareas dentro de proyectos de Workfront como tareas de marco, lo que a su vez creará carpetas de tareas dentro de Frame.io_

* Cuando el estado de un proyecto de Workfront se establece en Actual, se crea un proyecto conectado correspondiente en Frame, los usuarios asignados de Workfront se añaden al proyecto de Frame y se les envía una notificación por correo electrónico desde Frame.io

   * Todos los miembros del proyecto de Workfront (usuarios y equipos) se añadirán como colaboradores al proyecto Frame.io (en la creación del proyecto y más adelante)

   * _Cambio: los usuarios y equipos asignados a tareas de Workfront con Frame habilitado se añadirán como colaboradores al proyecto Frame.io y se les notificará (durante la creación del proyecto y posteriormente)_

* Los documentos (Creative Briefs) añadidos al proyecto y las tareas activadas por Frame se insertarán en el proyecto Frame.io (en la carpeta de trabajo correspondiente) cuando se cree el proyecto (déclencheur: el estado del proyecto se establece en Actual)

   * Le recomendamos que limite la cantidad de documentos añadidos a su proyecto antes de activarlos únicamente para sus informes creativos, a fin de evitar enviar varios documentos innecesarios a Frame.io

* _Mejora: Los usuarios/equipos a los que se les haya anulado explícitamente la asignación de una tarea de Workfront habilitada para tramas se eliminarán del proyecto Frame.io_

**Mejoras potenciales en futuras versiones:**

* Las tareas con tramas activadas se pueden configurar en plantillas de proyecto

* Las cargas de nuevas versiones a informes creativos se enviarán a Frame

* Sincronización optimizada de proyectos (desconexión de proyectos, resincronización de proyectos y documentos, etc.)

### Dentro de Frame.io, los creativos pueden enviar los recursos creados al proyecto de Workfront para su revisión formal

* Capacidad para conectar un solo recurso Frame.io a un proyecto o tarea de WF. Se creará una referencia de recurso en Workfront

* Las cargas de nuevas versiones dentro de Frame.io crearán automáticamente nuevas versiones de documentos dentro de Workfront en los recursos conectados

* _Mejora: Capacidad para marcar las tareas de Workfront a las que se hace referencia como completadas desde Frame.io_

* _Mejora: Si se elimina el documento de Workfront conectado, permanece dentro de Frame.io y se puede volver a conectar con la misma tarea de proyecto o con otra_

**Mejoras potenciales en futuras versiones:**

* Capacidad para enviar varios recursos de Frame.io a Workfront a la vez

* Registro de tiempo de proyectos/tareas de Workfront desde Frame.io

### Los coordinadores de proyectos pueden asignar el proceso de aprobación formal a documentos vinculados desde Frame.io

* Los usuarios y equipos de Workfront se pueden añadir a las nuevas aprobaciones de documentos para los documentos conectados de Frame.io

* _Mejora: Cuando un usuario/equipo deja de compartirse desde un documento con Frame habilitado, también perderá su acceso al recurso en el visor de Frame.io_

**Mejoras potenciales en futuras versiones:**

* Enviar varios recursos como una sola revisión

* Asignar aprobadores/revisores de forma masiva a documentos de Workfront

### Las partes interesadas pueden realizar su revisión y aprobación dentro del visor de Frame.io

* Se notificará a las partes interesadas y podrán ver el documento conectado a Frame en el visor de Frame.io

* Se puede acceder al Visor de Frame.io desde diferentes ubicaciones dentro de Workfront, por ejemplo, lista de documentos, detalles de documentos o inicio de Workfront

* Capacidad para aprovechar las capacidades existentes de revisión y comentarios proporcionadas por el visor Frame.io, que se sincronizará con el flujo de actualización de Workfront

* _Capacidad para tomar una nueva decisión de aprobación de documentos desde el visor de Frame.io_

### Dentro de Frame.io, se informará a los creativos sobre la decisión general tomada en el recurso Frame.io conectado

* _Mejora: El estado general de aprobación del documento se mostrará en el recurso dentro de Frame.io_

### AEM Los coordinadores de proyecto pueden enviar los recursos finales a los

* _AEM Mejora: los documentos conectados en marco, incluidos los metadatos, se pueden enviar a los usuarios mediante el conector de Workfront AEM + Asset CS existente._