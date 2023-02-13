---
title: 21.4 Mejoras del administrador
description: 21.4 Mejoras del administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1882'
ht-degree: 0%

---

# 21.4 Mejoras del administrador

En esta página se describen todas las mejoras realizadas por el administrador con la versión 21.4 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción en la semana del 4 de octubre de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.4, consulte [Resumen de la versión 21.4](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## Para administradores: Ver qué grupos están asociados a un proceso de aprobación

Para ayudarle a averiguar qué grupos están asociados a los procesos de aprobación en su sistema, hemos añadido una columna Nombre de grupo a la vista Estándar en la página Aprobaciones de Configuración. Ahora puede ver esta información sin tener que crear una vista personalizada.

Para obtener información sobre los procesos de aprobación, consulte [Información general del proceso de aprobación](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Para obtener información sobre la administración de procesos de aprobación de grupos, consulte [Procesos de aprobación a nivel de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Novedades para administradores: Los grupos pueden configurar sus propias preferencias de horario y hora

>[!NOTE]
>
>Inicialmente, en Producción, esta funcionalidad estará disponible como parte de un despliegue por fases solo para los clientes del Cluster 4. Esta nota se actualizará a medida que la funcionalidad esté disponible para otros clústeres.

En una organización grande, es posible que algunos grupos necesiten configurar las preferencias de horas y horas de forma independiente para que se ajusten a sus flujos de trabajo únicos, en lugar de heredar las preferencias configuradas por un administrador a nivel del sistema. Ahora los administradores de Workfront pueden desbloquear un parte de horas y una preferencia de hora para todos los grupos del sistema para que puedan configurarlo por su cuenta.

Esta capacidad también se agregó recientemente para las preferencias de proyecto y para las preferencias de tarea y problema.

Para obtener información sobre cómo un administrador de Workfront desbloquea un parte de horas y una preferencia de hora, consulte la sección [Desbloquear preferencias de horas y horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) en el artículo [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obtener información sobre cómo un administrador de grupo configura una tarea desbloqueada y las preferencias de problema para un grupo, consulte [Configuración de las preferencias de horas y horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Novedades para administradores de Workfront: Configurar plantillas de diseño para usuarios aprovisionados automáticamente en la nueva experiencia de Workfront

Ahora puede configurar las plantillas de diseño en la nueva experiencia de Workfront para los usuarios aprovisionados automáticamente. En el menú desplegable Atributo de usuario de Workfront, donde asigna atributos de usuario (Configuración > Sistema > Inicio de sesión único), ahora hay disponible un nuevo elemento de menú &quot;Plantilla de diseño NWE&quot; para realizar esta configuración. Anteriormente, solo se podían configurar plantillas de diseño para usuarios aprovisionados automáticamente en Workfront Classic.

Para obtener instrucciones sobre la asignación de atributos de usuario, consulte [Asignación de atributos de usuario y provisión automática de nuevos usuarios](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## El nuevo campo muestra los grupos a los que pertenecen los usuarios

Ahora es fácil averiguar a qué grupos pertenecen sus usuarios. En un informe o vista que enumera a los usuarios, puede crear una columna utilizando el nuevo campo Otros grupos . Este campo enumera los grupos a los que pertenece cada usuario.

Para obtener información sobre el uso de informes y vistas, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) y [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## La página de detalles de modelos ahora muestra una imagen

La página de detalles de cada modelo ahora muestra una imagen de la plantilla de proyecto que se instala con el modelo. La imagen proporciona una vista previa del contenido del modelo para que sepa lo que está a punto de instalar. Si lo desea, puede previsualizar la imagen completa en el navegador o descargar la imagen.

Para obtener más información, consulte [Información general sobre modelos](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Preferencias de modelos para nuevas cuestiones

Ya hay disponibles nuevas preferencias de problemas para algunos modelos. Se instalan de forma predeterminada, pero puede desactivar la instalación de las preferencias al configurar los detalles de instalación.

Las preferencias incluyen grupos de temas de cola, temas de cola y reglas de enrutamiento para recopilar la información correcta cuando se envía un problema o una solicitud, y enviar el problema o la solicitud al rol o equipo de trabajo correcto. El uso de las preferencias ayuda a crear coherencia en la forma en que se capturan nuevos problemas o solicitudes en los proyectos.

Tenga en cuenta que al utilizar estas preferencias, los proyectos creados a partir de la plantilla no se convierten en colas de solicitud.

Para obtener más información, consulte [Configuración de un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Novedades para administradores de grupos: Ver y administrar los elementos recientemente eliminados y restaurados de un grupo

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Seguimos facilitando la administración de sus grupos y objetos asociados en un solo lugar. Ahora puede ver y trabajar con los elementos recientemente eliminados y restaurados de un grupo del área Grupos. Esto evita tener que ir al área Eliminada recientemente o Restaurada recientemente en Configuración para administrar esos elementos. Y mantiene la lista de elementos de grupo con los que está trabajando separados de los otros elementos eliminados y restaurados del sistema.

Para obtener más información, consulte [Ver y administrar los elementos eliminados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) y [Ver y administrar los elementos restaurados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Novedades para administradores de grupos: Las preferencias de grupo ahora afectan a las plantillas de grupo

Ahora es más fácil asegurarse de que las plantillas de proyecto de su grupo satisfacen las necesidades de su grupo. Cuando asigna una nueva plantilla de proyecto a un grupo en el momento de crearla, la plantilla hereda la siguiente configuración de las preferencias de proyecto y tarea del grupo:

* Método de índice de rendimiento
* Tipo de condición
* Programar desde
* Tiempo de espera del usuario
* Tipo de actualización
* Acceso a la configuración de la sección

Cuando crea una nueva tarea de plantilla dentro de una plantilla de proyecto asociada a un grupo, la tarea de plantilla hereda la siguiente configuración de las preferencias de tareas del grupo:

* Tipo de duración
* Tipo de ingresos
* Tipo de costo

Anteriormente, las plantillas de proyecto y las tareas de plantilla de proyecto heredaban esta configuración de las preferencias de proyecto y tarea establecidas a nivel del sistema.

Si crea una plantilla o una tarea de plantilla sin un grupo (por ejemplo, desde la página de plantillas principal), la configuración anterior se hereda de las preferencias de tarea y proyecto del sistema. Sin embargo, si posteriormente asigna un grupo a la plantilla o a la tarea de plantilla, las preferencias del grupo no lo afectan.

Para obtener más información, consulte la sección Aplicación de las preferencias a plantillas y tareas de plantilla en el artículo [Creación y modificación de las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Novedades para administradores: Descubra qué formularios personalizados utilizan un campo personalizado

Ahora es más fácil cambiar un campo personalizado en un formulario personalizado. Con un solo clic en el formulario personalizado, puede encontrar cualquier otro formulario personalizado que también esté utilizando el campo . Es importante evaluar si estos formularios necesitarán ajustes para seguir funcionando correctamente después de realizar el cambio.

Para obtener más información, consulte [Ver todos los formularios personalizados que utilizan un widget o campo personalizado en particular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Novedades para administradores de grupos: Bloquear y desbloquear proyectos, tareas y preferencias de problemas para un grupo

Ahora puede asegurarse de que todos los subgrupos debajo de su grupo utilizan la misma configuración de preferencias o puede permitirles configurar una configuración de preferencias para sus flujos de trabajo únicos.

* Una vez que un administrador de Workfront desbloquea una preferencia a nivel de sistema, puede configurarla y luego bloquearla para todos los subgrupos debajo del grupo. Aunque aún puede volver a configurar la preferencia bloqueada, los administradores de subgrupos inferiores no pueden hacerlo para sus grupos.

   Por el contrario, puede desbloquear una preferencia para su grupo. Esto permite que los administradores de subgrupos lo configuren para las necesidades únicas de sus usuarios en cuanto a proyectos, tareas o flujos de trabajo de problemas.

   Para obtener más información, consulte [Bloquear o desbloquear un proyecto, tarea o preferencia de problemas para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Si es administrador de Workfront, no necesita ir al área Grupos para configurar las preferencias de un subgrupo. Desde las preferencias principales del proyecto Preferencias, Tareas y problemas o las preferencias de hojas de horas y horas, puede utilizar el cuadro de búsqueda situado en la parte superior de la página para encontrar el subgrupo y configurar sus preferencias.

   Para obtener más información, consulte [Configuración de las preferencias de un proyecto para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Configuración de las preferencias de tarea y problema para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Novedades para administradores de grupos: Crear y editar plantillas desde el área Grupos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Workfront.

Seguimos facilitando la administración de los grupos y sus objetos asociados en un solo lugar. Ahora puede ver y trabajar con las plantillas de un grupo desde el área Grupos de Configuración. Esto evita tener que ir al área Plantillas para administrar las plantillas de un grupo. Y mantiene la lista de plantillas de grupo en las que está trabajando separadas de las otras del sistema.

Para obtener más información, consulte [Creación y modificación de las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Introduzca y guarde información en un formulario personalizado adjunto a la vez

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora es más fácil proporcionar información en la sección Detalles de un objeto: Escriba y guarde información en un único campo personalizado o área expandible (como Información general y Finanzas), aunque los campos requeridos en otros formularios personalizados del objeto aún no estén rellenados.

Anteriormente, cuando se introducía información en un formulario personalizado o área ampliable para un objeto, todos los formularios personalizados adjuntos al objeto se ponían en modo de edición y todos los campos requeridos se debían completar antes de poder guardar los cambios. Este era un problema si no podía completar un campo obligatorio porque estaba destinado a otro usuario.

Si desea editar todos los formularios personalizados y áreas ampliables en la sección Detalles de un objeto, puede hacer clic en Editar todo en el nuevo menú Edición que hemos agregado al icono Editar. O bien, en el mismo menú, puede hacer clic en un nombre para desplazarse hasta el formulario o la sección personalizados en los que desee realizar cambios

>[!NOTE]
>
>Esta función se publicó originalmente en Preview con la versión 21.3.

Con el fin de facilitar a todos los niveles de una organización la gestión y el control de sus flujos de trabajo de forma independiente, se ha introducido la capacidad de crear y administrar estados para subgrupos. Ahora, desde la sección Grupos de Configuración, puede hacer lo siguiente para los grupos que administra en cualquier nivel:

* Crear, editar, eliminar y ocultar un estado para un grupo
* Bloquee un estado para cualquier grupo para que todos los subgrupos inferiores puedan utilizarlo de la misma manera
* Desbloquear un estado para cualquier grupo para que los administradores de subgrupos inferiores puedan personalizarlo para satisfacer sus necesidades específicas
* Establecer un estado de grupo como estado predeterminado
* Reordenar y ocultar la visualización de estados de grupo en objetos

Los administradores de Workfront también pueden hacer lo siguiente (para todos los grupos).

Anteriormente, esta funcionalidad solo estaba disponible para grupos de nivel superior.

Para obtener más información, consulte [Administrar estados de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Novedades para administradores de Workfront: Migración de plantillas de diseño de Workfront Classic a la nueva experiencia de Workfront por su cuenta

>[!NOTE]
>
>Esta función se publicó en el entorno de vista previa el 1 de julio de 2021. Se lanzará al entorno Producción el 15 de julio de 2021.

Para ayudarle a administrar las plantillas de diseño mientras los usuarios cambian a utilizar la nueva experiencia de Workfront, hemos creado un botón que puede utilizar para migrar las plantillas de diseño de Workfront Classic a la nueva experiencia sin depender del servicio de asistencia al cliente de Workfront.

Anteriormente, solo el Servicio de atención al cliente de Workfront podía migrar las plantillas de diseño de Workfront Classic a la nueva experiencia de Workfront.

## Al asociar una plantilla con un grupo, seleccione un proceso de aprobación de grupo en Detalles de cola y Temas de cola

Se ha añadido una nueva opción al proceso de asociar una plantilla con un grupo. Ahora puede seleccionar procesos de aprobación específicos del grupo para problemas en los Detalles de cola de la plantilla o en uno de sus Temas de cola.

En la versión 21.3, cuando se ha agregado la capacidad de asociar una plantilla de grupo a un grupo, se puede seleccionar un proceso de aprobación específico del grupo en la plantilla, pero no se puede hacer en los Detalles de cola o Temas de cola de la plantilla.

Para obtener más información, consulte [Asociar un proceso de aprobación nuevo o existente al trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
