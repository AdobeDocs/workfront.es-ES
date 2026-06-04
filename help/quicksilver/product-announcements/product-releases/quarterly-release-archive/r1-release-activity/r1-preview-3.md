---
content-type: release-notes
navigation-topic: product-releases-archive
title: Vista previa 3 de R1
description: Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión R1.3. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 1 de febrero de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
TQID: https://experienceleague.adobe.com/--RlYylhPcyb6lNrf8RuuC-87lrw88NlAms6EfmGRWo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1353
ht-degree: 100%

---

# Vista previa 3 de R1

Esta página describe todos los cambios disponibles en el entorno de vista previa con la versión R1.3. La funcionalidad de esta página estaba disponible en el entorno de vista previa el 1 de febrero de 2017.

Para obtener una lista de todos los cambios realizados en R1, consulte [Información general de la actividad de la versión R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Método mejorado para vincular archivos externos

La opción para vincular documentos desde una fuente externa (como Google Drive, Box, Dropbox, etc.) ahora se encuentra en una ubicación más destacada del área Documentos. 

Además, la acción de autorizar a un proveedor de documentos antes de vincular archivos de dicho proveedor por primera vez es ahora más intuitiva (es simplemente un paso adicional al vincular archivos de un proveedor externo).

Antes de realizar estos cambios, la opción para vincular archivos desde una fuente externa se encontraba en el cuadro de diálogo Añadir documentos dentro del área Documentos. Antes de vincular un documento desde una fuente externa por primera vez, el usuario que lo vinculaba tenía que autorizar al proveedor de documentos en el área de Configuración.

Para obtener más información, consulte [Vincular documentos desde aplicaciones externas](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Calendario de trabajo en curso del equipo actualizado

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront en la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

El Calendario de trabajo en curso disponible para los equipos contiene ahora funcionalidades adicionales y una apariencia actualizada. El Calendario de trabajo en curso funciona ahora de forma similar a la herramienta de horario de recursos de los proyectos.

El Calendario de trabajo en curso actualizado de los equipos incluye las siguientes mejoras:

* Vea los usuarios alfabéticamente o agrupados por función.
* Filtre la cronología de programación por prioridades de proyecto, estado y proyectos individuales. También puede filtrar la cronología de programación por funciones y usuarios. (El área Filtro incluye menos opciones que al programar recursos para proyectos).
* Incluya problemas en la cronología de programación.
* Muestre las asignaciones de usuarios y modifique el número de horas que se asignan a los usuarios a determinadas tareas y problemas cada día.
* Vea los indicadores que muestran cuándo se asignan excesivamente los usuarios en un día determinado.
* Configure si el trabajo completado se muestra en la cronología de la programación.

Diferencias con respecto a la herramienta de programación de recursos al programar recursos para proyectos:

* Todos los integrantes del equipo se muestran en el Calendario de trabajo en curso del equipo.\
  Al programar recursos para proyectos, solo se muestran los usuarios que tienen una función asociada que coincida con una función de una o varias tareas del área No asignada.
* La herramienta de intercambio no está disponible y no se incluye en el Calendario de trabajo en curso del equipo.
* Cualquier miembro del equipo puede realizar cambios en el Calendario de trabajo en curso.\
  Al programar recursos para proyectos, solamente los administradores de recursos pueden tomar decisiones de asignación de recursos para el proyecto.
* Los problemas se muestran de forma predeterminada en el Calendario de trabajo en curso del equipo.\
  Al programar recursos para proyectos, los problemas no se muestran de forma predeterminada.

Para obtener más información sobre el uso del Calendario de trabajo en curso del equipo actualizado, consulte “Horario de recursos”.

## Mejoras en el horario de los recursos

La cronología de programación incluye las siguientes mejoras:

* “Utilizar el filtro para controlar qué usuarios se muestran en la cronología de programación”
* “Los usuarios permanecen en la cronología después de que se les asigne una tarea”

### Utilizar el filtro para controlar qué usuarios se muestran en la cronología de programación {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>Las herramientas de programación de recursos han quedado obsoletas y se han eliminado de Workfront en la versión 23.1. Para obtener información sobre la programación de recursos mediante el Distribuidor de cargas de trabajo, consulte [Información general del Distribuidor de cargas de trabajo](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

El filtro se puede utilizar ahora para controlar qué usuarios se muestran en la cronología de la programación, además de qué tareas y problemas se muestran en el área sin asignar. Cuando se seleccionan usuarios en el filtro, solo se muestran los usuarios seleccionados, independientemente de si tienen una asignación de función que coincida con la asignación de función de las tareas del área Sin asignar. También se muestran todas las tareas asignadas actualmente a ese usuario.

Antes de este cambio, el filtro controlaba solamente qué tareas y problemas se mostraban en el área Sin asignar. Los usuarios se mostraban en la cronología de la programación solo si el usuario coincidía con la asignación de funciones de una tarea en el área Sin asignar.

Para obtener más información sobre el uso del filtro para controlar lo que se muestra en la cronología de programación, consulte “Filtrar información en el área de programación” y “Asignar manualmente tareas y problemas no asignados en las áreas de programación”.

### Los usuarios permanecen en la cronología después de que se les asigne una tarea {#users-remain-on-the-timeline-after-being-assigned-a-task}

Los usuarios permanecen en la cronología de la programación una vez que se les asigna una tarea o un problema, aunque no queden tareas o problemas con una asignación de función coincidente. Esto le permite realizar los cambios necesarios después de asignar los usuarios.

Antes de este cambio, los usuarios desaparecían de la cronología de la programación inmediatamente después de que se les asignara una tarea o un problema si no quedaban en el área Sin asignar con una asignación de función coincidente.

Para obtener más información, consulte “Asignar manualmente tareas y problemas no asignados en las áreas de programación”.

## Personalizar la terminología de Workfront cambiando el nombre de los objetos

Ahora puede personalizar la terminología de Workfront cambiando los nombres de ciertos objetos.\
Con una plantilla de diseño, ahora puede cambiar los nombres de los siguientes objetos de trabajo para que coincidan con las necesidades de su organización:

* Portafolio
* Programa
* Proyecto
* Tarea
* Problema

Por ejemplo, si en su organización trabaja con campañas en lugar de con proyectos, puede reemplazar el nombre del objeto “Proyecto” por “Campaña”.

Cuando se realiza este reemplazo, el nombre actualizado de los objetos se muestra en las siguientes áreas de la aplicación:

* Barra de navegación global
* Todas las fichas
* Todos los menús 
* Generador de informes y elementos de creación de informes (vistas, filtros y agrupaciones)
* Botones Guardar
* Archivos exportados
* Correos electrónicos

Las áreas siguientes no muestran el nombre actualizado de los objetos:

* Estimaciones de recursos
* Administrador del presupuesto de recursos
* Planificador de capacidades
* Cuadrícula de recursos
* Generador de equipos
* Optimizador de portafolios 
* Aplicaciones móviles
* Complemento de Outlook

Para obtener más información sobre cómo personalizar la terminología de Workfront con una plantilla de diseño, consulte la sección “Personalización de la terminología” en “Creación y administración de plantillas de diseño” y la sección “Explicación de las implicaciones de la personalización de nombres de objetos” en [Comprender los objetos de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Incluir fechas de inicio y de finalización de la aprobación en los informes

Ahora puede incluir los siguientes campos al crear o modificar informes:

* Fecha de inicio de la ruta de aprobación
* Fecha de finalización de la ruta de aprobación

Estos campos le permiten obtener información sobre cuándo se inició la ruta de aprobación actual o la más reciente y cuándo se marcó como completa.

Para obtener más información sobre estos campos, consulte [Glosario de terminología de Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Para obtener más información sobre las rutas de aprobación, cómo se crean y desencadenan y la función que sirven en procesos de aprobación, consulte [Crear un proceso de aprobación para elementos de trabajo](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Los siguientes campos se han eliminado de Workfront y ya no pueden incluirse en los informes (estos campos proporcionaban información sobre el proyecto en lugar de sobre las aprobaciones en sí, y a menudo se utilizaban indebidamente):

* Fecha de inicio planificada de las aprobaciones
* Fecha proyectada de inicio de la aprobación
* Fecha estimada de inicio de la aprobación

## Nuevas opciones de resumen de correo electrónico para “Solicitudes que he realizado”

La opción de entrega de resumen diario se ha añadido al área “Solicitudes que he realizado” de la configuración de Notificaciones.

Para obtener más información, consulte [Modificar sus propias notificaciones por correo electrónico](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad. Esto es necesario porque la zona protegida de previsualización borra las direcciones de correo electrónico de todos los usuarios.

## Apariencia actualizada de las notificaciones por correo electrónico de aprobación de documentos

La apariencia de la notificación de “Aprobación del documento” se ha actualizado con una nueva IU:

Para obtener más información sobre las notificaciones por correo electrónico, consulte [Notificaciones de Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Recuerde actualizar la dirección de correo electrónico asociada a su cuenta para poder probar esta funcionalidad. Esto es necesario porque la zona protegida de previsualización borra las direcciones de correo electrónico de todos los usuarios.

## Mejoras en la vista de hito

La vista de hito que está disponible cuando se visualiza una lista de proyectos o un informe de proyectos ahora contiene las siguientes mejoras:

* Las fechas planificadas son editables
* Se muestra el porcentaje completado de proyectos y tareas

Antes de este cambio, para editar las fechas o ver el porcentaje completado, tenía que ir a cada tarea.

Para obtener más información, consulte [Usar la vista de hito](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
