---
content-type: release-notes
navigation-topic: product-releases-archive
title: Actividad de la versión beta 4 de 2018.1
description: Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión beta 4 de 2018.1. La funcionalidad estaba disponible en el entorno de vista previa el 24 de enero de 2018. Estará disponible en el entorno de producción en marzo de 2018.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 8e016f12-bc72-475c-a8cc-38ded4351f88
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '2435'
ht-degree: 0%

---

# Actividad de la versión beta 4 de 2018.1

Esta página describe todos los cambios disponibles más recientemente en el entorno de vista previa con la versión beta 4 de 2018.1. La funcionalidad estaba disponible en el entorno de vista previa el 24 de enero de 2018. Estará disponible en el entorno de producción en marzo de 2018.

>[!IMPORTANT]
>
> La funcionalidad descrita en esta página está sujeta a cambios antes de su disponibilidad en el entorno de producción de.

Para ver una lista de todos los cambios realizados en 2018.1, consulte  [información general sobre la actividad de la versión 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

La versión beta 4 de 2018.1 contiene mejoras tanto para administradores de Workfront como para otros usuarios:

**Para administradores**

* [Programaciones administradas por administradores de grupo](#schedules-managed-by-group-administrators)

**Para todos los usuarios**

* [Mejoras de corrección en Workfront](#proofing-improvements-within-workfront)
* [Creación de pruebas en Workfront Proof: experiencia del usuario mejorada y funcionalidad adicional](#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality)
* [Mejoras de revisión en Workfront y Workfront Proof](#proofing-improvements-within-workfront-and-workfront-proof)
* [Aspecto actualizado con la integración de Basecamp en Workfront Proof](#updated-look-and-feel-with-basecamp-integration-in-workfront-proof)
* [Pegar imágenes en Workfront desde el portapapeles](#paste-images-to-workfront-from-the-clipboard)
* [Mejoras del informe de utilización](#utilization-report-improvements)
* [Quitar el objeto de hora presupuestado de recurso de Workfront](#remove-the-resource-budgeted-hour-object-from-workfront)
* [Estadísticas de uso del informe](#report-usage-statistics)
* [Actualizaciones de gráfico Gantt](#gantt-chart-updates)
* [Nuevo Portfolio Optimizer](#new-portfolio-optimizer)
* [Opción de Ajuste de Fecha Presupuestaria en el Planificador de Recursos](#budget-date-adjustment-option-in-the-resource-planner)
* [Programación de recursos: Restringir asignaciones a usuarios según la pertenencia a grupos](#resource-scheduling-restrict-assignments-to-users-based-on-group-membership)
* [Horario de recursos: permitir asignaciones a usuarios independientemente del rol](#resource-scheduling-allow-assignments-to-users-regardless-of-role)
* [Compatibilidad con Emoji](#emoji-support)

## Mejoras de corrección en Workfront {#proofing-improvements-within-workfront}

Se han realizado las siguientes mejoras en la lista de documentos de Workfront: 

* [Ver progreso de revisión de la lista de documentos](#view-proof-progress-from-the-document-list)
* [Nueva opción para ver el resumen de impresión desde la lista de documentos](#new-option-to-view-the-print-summary-from-the-document-list)
* [Apariencia actualizada para generar o abrir la prueba desde la lista de documentos](#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list)
* [Varios vínculos eliminados de documentos en la lista de documentos](#various-links-removed-from-documents-on-the-document-list)
* [Ver nombres de archivo en pruebas combinadas](#view-file-names-on-combined-proofs)
* [Ver la fase activa actual de una prueba en la lista de documentos](#view-the-current-active-stage-of-a-proof-from-the-document-list)

### Ver progreso de revisión de la lista de documentos {#view-proof-progress-from-the-document-list}

Los indicadores de progreso de prueba ahora se muestran para todas las pruebas al ver la lista de documentos. (Esto incluye Enviados, Aperturas, Comentarios realizados y Decisión).

Antes de este cambio, tenía que seleccionar una prueba en la lista de documentos para ver el progreso de la prueba en el panel derecho. 

Para obtener más información, consulte [Progreso de prueba e información general de estado](../../../../review-and-approve-work/proofing/proofing-overview/view-progress-status-proof.md).

### Nueva opción para ver el resumen de impresión desde la lista de documentos {#new-option-to-view-the-print-summary-from-the-document-list}

Ahora puede ver el resumen de impresión de una prueba directamente desde la lista de documentos.

Antes de este cambio, solo podía ver el resumen de impresión desde el visor de pruebas. 

Para obtener más información sobre cómo ver el resumen de impresión desde la lista de documentos, consulte [Imprimir un resumen de prueba en Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md).

### Apariencia actualizada para generar o abrir la prueba desde la lista de documentos {#updated-look-and-feel-for-generating-or-opening-the-proof-from-the-document-list}

Ahora, al pasar el ratón por encima de un documento en la lista de documentos, se han actualizado las opciones para generar la prueba o abrirla. Estas opciones ahora son más prominentes y aparecen como botones.

Antes de este cambio, estas opciones estaban disponibles como vínculos debajo del nombre del documento.

Para obtener más información, consulte las secciones siguientes:

* .
* en .

### Varios vínculos eliminados de documentos en la lista de documentos {#various-links-removed-from-documents-on-the-document-list}

Las siguientes acciones ya no están disponibles como vínculos en documentos individuales dentro de la lista de documentos:

* Generar revisión
* Revisión
* Detalles
* Compartir
* Desproteger / Proteger

Las siguientes acciones están ahora disponibles como un botón en el documento dentro de la lista de documentos:

* Abrir revisión (disponible después de que se genere la revisión) 
* Generar revisión (disponible cuando la revisión aún no se ha generado)

Las siguientes acciones están ahora disponibles en el menú desplegable junto al botón Abrir prueba o Generar prueba:

* Detalles de la revisión
* Detalles del documento
* Imprimir resumen

Para obtener más información, consulte las secciones siguientes:

* .
* en .

### Ver nombres de archivo en pruebas combinadas {#view-file-names-on-combined-proofs}

Ahora puede ver los nombres de archivo individuales que conforman una prueba combinada. Esta información se muestra en la pestaña Detalles cuando se selecciona la prueba en la lista de documentos.

Para obtener más información, consulte Visualización de todos los archivos contenidos en una prueba combinada. 

### Ver la fase activa actual de una prueba en la lista de documentos {#view-the-current-active-stage-of-a-proof-from-the-document-list}

Ahora, al seleccionar una prueba en la lista de documentos, las fases activas actuales se muestran en la columna derecha de la pestaña Detalles. 

Para obtener más información, consulte [Visualización de las fases activas en una prueba](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/view-active-stages-proof.md).  

## Creación de pruebas en Workfront Proof: experiencia del usuario mejorada y funcionalidad adicional {#proof-creation-in-workfront-proof-improved-user-experience-and-additional-functionality}

Además de mejorar la experiencia del usuario al crear pruebas en Workfront Proof, ya están disponibles las siguientes funciones adicionales:

* Combine varias imágenes en una sola prueba.
* Prueba de sitios web en varias resoluciones (se pueden crear varias resoluciones como pruebas individuales o se pueden combinar en una sola prueba).
* Edite el nombre del archivo durante el proceso de carga.
* Incluya campos personalizados en el formulario de creación de prueba.
* Agregue un mensaje personalizado a las notificaciones de prueba por correo electrónico.
* Configuración de prueba adicional 
* Validación de errores en tiempo real al revisar una dirección URL (anteriormente, tenía que esperar varios minutos antes de que se mostrara un error)

>[!NOTE]
>
>Esta nueva página de creación de pruebas de Workfront Proof ahora coincide con la página de creación de pruebas que estuvo disponible recientemente al crear pruebas en Workfront. 

Para obtener más información, consulte  [Generar revisiones en Workfront Proof](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Mejoras de revisión en Workfront y Workfront Proof {#proofing-improvements-within-workfront-and-workfront-proof}

Los siguientes cambios se aplican cuando se agregan documentos a Workfront y a Workfront Proof:

* [Cambiar el tamaño de la lista de comentarios al revisar las pruebas](#resize-the-comment-list-when-reviewing-proofs)
* [Los Hipervínculos Están Activos Al Revisar Las Pruebas Estáticas](#hyperlinks-are-active-when-reviewing-static-proofs)
* [Mejoras Al Añadir Pruebas](#improvements-when-adding-proofs)

### Cambiar el tamaño de la lista de comentarios al revisar las pruebas {#resize-the-comment-list-when-reviewing-proofs}

Ahora puede cambiar el tamaño de la lista de comentarios al revisar las pruebas en el visor de pruebas.

Para obtener más información, consulte en .

### Los Hipervínculos Están Activos Al Revisar Las Pruebas Estáticas {#hyperlinks-are-active-when-reviewing-static-proofs}

Los hipervínculos ahora están activos al revisar una prueba estática en el visualizador de pruebas. Haga clic en un hipervínculo para ir a la página vinculada.

Esta funcionalidad se admite en cualquier tipo de archivo que contenga texto, como PDF, DOC, etc. No se admiten archivos de imagen.

### Mejoras Al Añadir Pruebas {#improvements-when-adding-proofs}

Las siguientes mejoras están disponibles cuando se agregan documentos para revisar. 

* La información de la lista Destinatarios ahora está disponible en una vista de tres columnas, lo que facilita la visualización y modificación de la información. 

  Anteriormente, la información se mostraba en una vista de una sola columna, lo que requería más clics cuando era necesario realizar cambios. 

  Para obtener más información, consulte en .

* Arrastre uno o varios destinatarios de una fase del flujo de trabajo a otra al utilizar el flujo de trabajo automatizado. Puede arrastrar directamente a un escenario o a un escenario del diagrama, ubicado en la parte superior de la página.

  Para obtener más información, consulte en .

* El diagrama de flujo de trabajo permanece visible en la parte superior de la página incluso al desplazarse. El diagrama está contraído de forma predeterminada; expanda el diagrama para ver el diagrama completo.

  Para obtener más información, consulte en .

* Al añadir una plantilla a un flujo de trabajo automatizado en una prueba, se muestra una animación de carga que indica que la plantilla se está cargando.

  Para obtener más información, consulte en .

* Las siguientes configuraciones se movieron de la sección Configuración de prueba a la sección Flujo de trabajo en la página Nueva prueba:

   * Responsable principal de la toma de decisiones
   * Requerir solo una decisión

## Aspecto actualizado con la integración de Basecamp en Workfront Proof {#updated-look-and-feel-with-basecamp-integration-in-workfront-proof}

Se ha actualizado el aspecto de la integración de Basecamp con Workfront Proof. La funcionalidad sigue siendo la misma.

## Pegar imágenes en Workfront desde el portapapeles {#paste-images-to-workfront-from-the-clipboard}

Ahora puede agregar archivos de imagen a Workfront pegando una imagen del portapapeles del sistema.

La capacidad de pegar desde el portapapeles se eliminó de Workfront en una versión anterior y se vuelve a incluir en esta versión. El nuevo método es más ágil e intuitivo.

Para obtener más información, consulte [Pegar imágenes desde el portapapeles](../../../../documents/managing-documents/paste-image-clipboard.md). 

## Mejoras del informe de utilización {#utilization-report-improvements}

El informe Utilización incluye las siguientes mejoras:

* Ver los ingresos en el informe de utilización de un proyecto

  Permite consultar los ingresos presupuestados, los ingresos planificados, los ingresos reales, la desviación presupuestada y la desviación planificada.

* Comparar ingresos con costos planificados y reales

  Permite ver el costo planificado o real junto con los ingresos planificados. También se muestra el margen (%) (el margen se calcula como Ingresos - Coste / Ingresos).

* Los ingresos se muestran al ver el gráfico.
* Los encabezados permanecen visibles al desplazarse.

  Ahora, al desplazarse por la información del informe Utilización, el encabezado situado en la parte superior del informe Utilización siempre está visible, lo que le permite comprender más fácilmente los datos del informe.

  Anteriormente, el encabezado de la parte superior del informe Utilización se desplazaba fuera de la vista al desplazarse.

* El informe de utilización de un proyecto individual se carga automáticamente

  Cuando se visualiza el informe Utilización de un proyecto, el informe se carga automáticamente.

  Antes de este cambio, tenía que hacer clic en &quot;Ejecutar&quot; antes de ejecutar el informe.

* Rendimiento mejorado

Para obtener más información sobre el informe Utilización, consulte [Descripción general del informe Utilización de los recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

## Quitar el objeto de hora presupuestado de recurso de Workfront {#remove-the-resource-budgeted-hour-object-from-workfront}

Para solucionar problemas de rendimiento, el campo Hora presupuestada de recurso se eliminó temporalmente de Workfront.

Como recordatorio, las horas presupuestadas de recurso son las horas presupuestadas para sus recursos o sus proyectos en el Planificador de recursos. Por el momento, ya no puede informar sobre este campo en la aplicación web o a través de la API. El campo se restablecerá en una versión futura, cuando se hayan resuelto los problemas de rendimiento.

Para obtener más información sobre cómo presupuestar horas en el Planificador de recursos, consulte [Resumen del Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md). 

## Estadísticas de uso del informe {#report-usage-statistics}

Ahora puede mostrar la siguiente información de uso de los informes de Workfront en una lista de informes:

* Última visualización por
* Fecha de última visualización
* 10 últimas personas que visualizaron
* Vistas de este mes/trimestre/año
* Vistas del último mes/trimestre/año
* Todas las vistas

Antes de esta actualización, la información de uso que se podía ver en los informes era limitada.

Para obtener más información sobre el uso de los informes, consulte [Ver uso del informe](../../../../reports-and-dashboards/reports/report-usage/view-report-usage.md)

## Programaciones administradas por administradores de grupo {#schedules-managed-by-group-administrators}

Como administrador de grupos, puede crear y editar programaciones asociadas a los grupos que administra, así como a sus subgrupos. Antes de este cambio, solo los administradores de Workfront podían crear y editar programaciones.

Para obtener más información sobre la administración de programaciones, consulte [Creación de una programación](../../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

## Actualizaciones de gráfico Gantt {#gantt-chart-updates}

El gráfico Gantt ahora se puede editar. Con el diagrama de Gantt, puede realizar las siguientes actualizaciones en sus tareas:

* Crear relaciones de predecesoras
* Editar duración de la tarea
* Actualizar el porcentaje completado de la tarea
* Aplicar nivelación de recursos

Antes de este cambio, sólo se podían quitar relaciones de predecesoras en el diagrama de Gantt y modificar tareas sólo en la lista de tareas.

Para obtener más información sobre el gráfico Gantt, consulte [Actualizar información en el gráfico Gantt de lista de tareas](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)

## Nuevo Portfolio Optimizer {#new-portfolio-optimizer}

El área de Portfolio Optimizer de Workfront ahora se actualiza con una nueva apariencia. La funcionalidad no ha cambiado.

Para obtener más información sobre Portfolio Optimizer, consulte [Información general de Portfolio Optimizer](../../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## Opción de Ajuste de Fecha Presupuestaria en el Planificador de Recursos {#budget-date-adjustment-option-in-the-resource-planner}

Se ha añadido una opción para darle una visibilidad rápida de los períodos de tiempo sin conflictos de presupuesto. Después de ver cuándo se producen los períodos de tiempo sin conflictos de presupuestos, puede mover manualmente las horas presupuestadas a esos períodos. Esto también ajusta las fechas presupuestadas de las horas. Antes de esta actualización, no era posible ver de un vistazo los conflictos presupuestarios de un proyecto.

Para obtener más información sobre el ajuste de fechas presupuestadas en el Planificador de recursos, consulte la sección &quot;Ajuste de Fechas de Presupuestación&quot; en el [Resumen del Planificador de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)

## Programación de recursos: Restringir asignaciones a usuarios según la pertenencia a grupos {#resource-scheduling-restrict-assignments-to-users-based-on-group-membership}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront con la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Descripción general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Al realizar asignaciones de usuarios en el área de Programación (como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de Programación&quot;), ahora puede configurar Workfront para que restrinja las asignaciones de tareas y problemas únicamente a los usuarios que sean miembros del grupo definido en el proyecto en el que se origina la tarea o el problema. 

Esto se aplica cuando se realizan asignaciones de las siguientes maneras:

* Al asignar un usuario a todas las tareas y problemas de una función específica, como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

  Antes de este cambio, una tarea o un problema siempre se podía asignar a cualquier usuario, independientemente de su pertenencia al grupo. 

* Al intercambiar asignaciones con otro usuario, como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

  Antes de este cambio, una tarea o un problema siempre se podía asignar a cualquier usuario, independientemente de su pertenencia al grupo. 

* Cuando se asigna manualmente una tarea o un problema desde la cronología de programación, como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

  Antes de este cambio, una tarea o un problema siempre se podía asignar a cualquier usuario, independientemente de su pertenencia al grupo. 

* Al permitir que Workfront asigne usuarios automáticamente, como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

  Antes de este cambio, Workfront asignaba tareas y problemas a los usuarios independientemente de su pertenencia al grupo.

Para obtener más información sobre la configuración de esta opción, consulte &quot;Introducción a la programación de recursos&quot;.

## Horario de recursos: permitir asignaciones a usuarios independientemente del rol {#resource-scheduling-allow-assignments-to-users-regardless-of-role}

Al realizar asignaciones de usuarios en el área de Programación (como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de Programación&quot;), ahora puede configurar Workfront para que permita que las tareas y los problemas se asignen a cualquier usuario, independientemente de si ese usuario tiene una función definida en su perfil de usuario que coincida con la asignación de funciones de la tarea o el problema que se le esté asignando.

Esto se aplica cuando se realizan asignaciones de las siguientes maneras:

* Al asignar un usuario a todas las tareas y problemas de una función específica, como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot; en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

  Antes de este cambio, la función principal del usuario que está asignando tenía que coincidir con la función ya definida en el campo Seleccionar función.

* Al intercambiar asignaciones con otro usuario, como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

  Antes de este cambio, la función principal del usuario que está asignando tenía que coincidir con la función ya definida en el campo Seleccionar función.

* Cuando se asigna manualmente una tarea o un problema desde la cronología de programación, como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;.

  Antes de este cambio, en la escala de tiempo de la programación solo se mostraban los usuarios cuya función coincidía con la función de la tarea o el problema que estaba asignando.

>[!NOTE]
>
>Esto no se aplica cuando se permite que Workfront asigne usuarios automáticamente, tal como se describe en &quot;Asignar manualmente tareas y problemas no asignados en las áreas de programación&quot;. Al asignar automáticamente usuarios, las tareas y los problemas solo se pueden asignar a usuarios con una función coincidente.

Para obtener más información sobre la configuración de esta opción, consulte &quot;Introducción a la programación de recursos&quot;.

## Compatibilidad con Emoji {#emoji-support}

Ahora puede establecer el tono de los comentarios y las actualizaciones que realice en Workfront insertando emojis. Los emojis añadidos a los comentarios realizados en la pestaña Actualizaciones también se muestran en la notificación de actualización por correo electrónico. 

Para obtener más información, consulte [Actualizar trabajo](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
