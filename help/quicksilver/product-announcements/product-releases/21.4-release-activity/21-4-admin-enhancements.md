---
title: 21.4 Mejoras del administrador
description: 21.4 Mejoras del administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: fc85b4c2-4a76-4226-9120-11635b03aa4e
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# 21.4 Mejoras del administrador

Esta página describe todas las mejoras realizadas por el administrador con la versión 21.4 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 4 de octubre de 2021.

Para ver una lista de todos los cambios disponibles con la versión 21.4, consulte [21.4 Información general de la versión](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Para administradores: ver qué grupos están asociados con un proceso de aprobación

Para ayudarle a averiguar qué grupos están asociados con los procesos de aprobación de su sistema, hemos agregado una columna Nombre de grupo a la vista Estándar en la página Aprobaciones de Configuración. Ahora puede ver esta información sin tener que crear una vista personalizada.

Para obtener información sobre los procesos de aprobación, consulte [Resumen del proceso de aprobación](../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Para obtener información sobre la administración de procesos de aprobación de grupos, consulte [Procesos de aprobación de nivel de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Nuevo para administradores: los grupos pueden configurar sus propias preferencias de horas y hojas de horas

>[!NOTE]
>
>Inicialmente, en el entorno de producción, esta funcionalidad estará disponible como parte de un despliegue gradual solo para los clientes del clúster 4. Esta nota se actualizará a medida que la funcionalidad esté disponible para otros clústeres.

En una organización grande, es posible que algunos grupos necesiten configurar las preferencias de horas y de plantillas de horas de forma independiente para ajustarse a sus flujos de trabajo únicos, en lugar de heredar las preferencias configuradas por un administrador a nivel de sistema. Ahora los administradores de Workfront pueden desbloquear una plantilla de horas y una preferencia de horas para todos los grupos del sistema y así poder configurarlas ellos mismos.

Esta capacidad también se ha agregado recientemente para preferencias de proyecto y para preferencias de tarea y problema.

Para obtener información sobre cómo un administrador de Workfront desbloquea una plantilla de horas y preferencias de hora, consulte la sección [Desbloquear hoja de horas y preferencias de horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) en el artículo [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obtener información sobre cómo un administrador de grupo configura las preferencias de tareas y problemas desbloqueados para un grupo, consulte [Configurar las preferencias de horas y hojas de horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Nuevo para administradores de Workfront: configuración de plantillas de diseño para usuarios con aprovisionamiento automático en la nueva experiencia de Workfront

Ahora puede configurar las plantillas de diseño en la nueva experiencia de Workfront para los usuarios que se aprovisionan automáticamente. En el menú desplegable Atributo de usuario de Workfront, donde se asignan los atributos de usuario (Configuración > Sistema > Inicio de sesión único), ahora hay disponible un nuevo elemento de menú &quot;Nueva plantilla de diseño&quot; para realizar esta configuración. Anteriormente, solo se podían configurar plantillas de diseño para usuarios con aprovisionamiento automático en Workfront Classic.

Para obtener instrucciones sobre la asignación de atributos de usuario, consulte [Asignar atributos de usuario y aprovisionar automáticamente nuevos usuarios](../../../administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## El nuevo campo muestra los grupos a los que pertenecen los usuarios

Ahora es fácil averiguar a qué grupos pertenecen sus usuarios. En un informe o vista que enumera usuarios, puede crear una columna con el nuevo campo Otros grupos. Este campo enumera los grupos a los que pertenece cada usuario.

Para obtener información sobre el uso de informes y vistas, consulte [Creación de un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) y [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## La página de detalles de modelos ahora muestra una imagen

La página de detalles de cada modelo ahora muestra una imagen de la plantilla de proyecto que se instala con el modelo. La imagen proporciona una vista previa del contenido del modelo para que sepa lo que va a instalar. Si lo desea, puede previsualizar la imagen completa en el explorador o descargar la imagen.

Para obtener más información, consulte [Información general de modelos](../../../administration-and-setup/blueprints/blueprints-overview.md).

![](assets/blueprint-detailspage.png)

## Preferencias de modelos para nuevos problemas

Ya están disponibles las nuevas preferencias de problema para algunos modelos. Se instalan de forma predeterminada, pero puede excluirse de la instalación de las preferencias al configurar los detalles de instalación.

Las preferencias incluyen grupos de temas de colas, temas de colas y reglas de enrutamiento para recopilar la información correcta cuando se envía un problema o una solicitud, y enviar el problema o la solicitud al rol o equipo correcto. El uso de las preferencias ayuda a crear coherencia en la forma en que se capturan los nuevos problemas o solicitudes en los proyectos.

Tenga en cuenta que el uso de estas preferencias no convierte los proyectos creados a partir de la plantilla en colas de solicitudes.

Para obtener más información, consulte [Configurar un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Nuevo para administradores de grupos: vea y administre los elementos eliminados y restaurados recientemente de un grupo

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Seguimos facilitando la administración de sus grupos y sus objetos asociados en un solo lugar. Ahora puede ver y trabajar con los elementos recientemente eliminados y restaurados de un grupo desde el área de Grupos. Esto evita tener que ir al área Eliminados recientemente o Restaurados recientemente en la Configuración para administrar esos elementos. Además, mantiene la lista de los elementos del grupo con los que está trabajando separada de los demás elementos eliminados y restaurados del sistema.

Para obtener más información, consulte [Ver y administrar los elementos eliminados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) y [Ver y administrar los elementos restaurados recientemente de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).

## Nuevo para administradores de grupos: Las preferencias de grupo ahora afectan a las plantillas de grupo

Ahora es más fácil asegurarse de que las plantillas de proyecto del grupo satisfacen las necesidades del grupo. Cuando asigna una nueva plantilla de proyecto a un grupo en el momento en que lo crea, la plantilla hereda la siguiente configuración de las preferencias de proyecto y tarea del grupo:

* Método de índice de rendimiento
* Tipo de condición
* Programar desde
* Tiempo libre del usuario
* Tipo de actualización
* Configuración de sección de acceso

Cuando se crea una nueva tarea de plantilla dentro de una plantilla de proyecto asociada a un grupo, la tarea de plantilla hereda la siguiente configuración de las preferencias de tarea del grupo:

* Tipo de duración
* Tipo de ingresos
* Tipo de costo

Anteriormente, las plantillas de proyecto y las tareas de plantilla de proyecto heredaban esta configuración de las preferencias de proyecto y tarea establecidas en el sistema.

Si crea una plantilla o tarea de plantilla sin un grupo (por ejemplo, desde la página principal Plantillas), la configuración anterior se hereda de las preferencias de proyecto y tarea de nivel del sistema. Sin embargo, si posteriormente asigna un grupo a la plantilla o tarea de plantilla, las preferencias del grupo no le afectan.

Para obtener más información, vea la sección Cómo se aplican las preferencias a las plantillas y tareas de plantilla en el artículo [Crear y modificar las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Nuevo para administradores: Descubra qué formularios personalizados utilizan un campo personalizado

Ahora es más fácil cambiar un campo personalizado en un formulario personalizado. Con un solo clic en el formulario personalizado, puede obtener información sobre cualquier otro formulario personalizado que también utilice el campo. Es importante evaluar si esos formularios necesitarán ajustes para seguir funcionando correctamente después de realizar el cambio.

Para obtener más información, consulte [Ver todos los formularios personalizados que utilizan un campo o widget personalizado en particular](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md).

## Novedades para los administradores de grupos: bloquear y desbloquear preferencias de proyectos, tareas y problemas de un grupo

Ahora puede asegurarse de que todos los miembros de los subgrupos debajo de su grupo estén utilizando la misma configuración de preferencias o puede permitirles configurar una configuración de preferencias para sus flujos de trabajo únicos.

* Una vez que un administrador de Workfront desbloquea una preferencia en el sistema, puede configurarla y bloquearla para todos los subgrupos por debajo del grupo. Aunque todavía puede volver a configurar la preferencia bloqueada, los administradores de subgrupos inferiores no pueden hacerlo para sus grupos.

  Por el contrario, puede desbloquear una preferencia para su grupo. Esto permite a los administradores de subgrupos configurarlo para el proyecto, la tarea o el flujo de trabajo de problemas únicos de sus usuarios.

  Para obtener más información, consulte [Bloquear o desbloquear una preferencia de proyecto, tarea o problema para subgrupos](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md).

* Si es administrador de Workfront, no es necesario que vaya al área de Grupos para configurar las preferencias de un subgrupo. En el área principal Preferencias de proyecto, Preferencias de tareas y problemas o Preferencias de horas y hojas de horas, puede usar el cuadro de búsqueda en la parte superior de la página para buscar el subgrupo y configurar sus preferencias.

  Para obtener más información, consulte [Configurar las preferencias de proyecto de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) y [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Nuevo para administradores de grupos: cree y edite plantillas desde el área de Grupos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Workfront.

Seguimos facilitando la administración de sus grupos y sus objetos asociados en un solo lugar. Ahora puede ver y trabajar con las plantillas de un grupo desde el área Grupos en Configuración. Esto evita tener que ir al área Plantillas para administrar las plantillas de un grupo. Y mantiene la lista de plantillas de grupo en las que está trabajando separada de las demás en todo el sistema.

Para obtener más información, consulte [Crear y modificar las plantillas de proyecto de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md).

## Introduzca y guarde información en un formulario personalizado adjunto a la vez

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront.

Ahora es más fácil proporcionar información en la sección Detalles de un objeto: escriba y guarde información en un único campo personalizado o área expansible (como Información general y Finanzas), incluso si los campos obligatorios de otros formularios personalizados del objeto aún no están rellenados.

Anteriormente, cuando se especificaba información en un formulario personalizado o área expansible para un objeto, todos los formularios personalizados adjuntos al objeto entraban en modo de edición y todos sus campos obligatorios debían rellenarse antes de poder guardar los cambios. Este problema se producía si no se podía completar un campo obligatorio porque estaba destinado a otro usuario.

Si desea editar todos los formularios personalizados y las áreas ampliables de la sección Detalles de un objeto, puede hacer clic en Editar todo en el nuevo menú Edición que hemos agregado al icono Editar. O bien, en el mismo menú, puede hacer clic en un nombre para desplazarse hasta el formulario o la sección personalizados donde desee realizar los cambios

>[!NOTE]
>
>Esta función se publicó originalmente en Vista previa con la versión 21.3.

Para facilitar a todos los niveles de una organización la administración y el control de sus flujos de trabajo de forma independiente, hemos introducido la capacidad de crear y administrar estados para subgrupos. Ahora, desde la sección Grupos en Configuración, puede hacer lo siguiente para los grupos que administre en cualquier nivel:

* Crear, editar, eliminar y ocultar un estado para un grupo
* Bloquee un estado para cualquier grupo de modo que todos los subgrupos inferiores debajo de él puedan utilizarlo de la misma manera
* Desbloquee un estado para cualquier grupo para que los administradores de subgrupos inferiores puedan personalizarlo para satisfacer sus necesidades únicas
* Establecer un estado de grupo como estado predeterminado
* Reordenar y ocultar la visualización de estados de grupo en objetos

Los administradores de Workfront también pueden hacer estas cosas (para todos los grupos).

Anteriormente, esta funcionalidad solo estaba disponible para grupos de nivel superior.

Para obtener más información, consulte [Administrar estados de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md).

## Nuevo para administradores de Workfront: Migre las plantillas de diseño de Workfront Classic a la nueva experiencia de Workfront por su cuenta

>[!NOTE]
>
>Esta función se publicó en el entorno de vista previa el 1 de julio de 2021. Se lanzará al entorno de producción el 15 de julio de 2021.

Para ayudarle a administrar las plantillas de diseño mientras sus usuarios cambian a la nueva experiencia de Workfront, hemos creado un botón que puede utilizar para migrar las plantillas de diseño de Workfront Classic a la nueva experiencia sin depender de la asistencia al cliente de Workfront.

Anteriormente, solo la Asistencia al cliente de Workfront podía migrar las plantillas de diseño de Workfront Classic a la nueva experiencia de Workfront.

## Al asociar una plantilla a un grupo, seleccione un proceso de aprobación de grupo en Detalles de cola y Temas de cola

Se ha añadido una nueva opción al proceso de asociar una plantilla con un grupo. Ahora puede seleccionar procesos de aprobación específicos del grupo para problemas en los Detalles de cola de la plantilla o en uno de sus Temas de cola.

En la versión 21.3, cuando añadimos la capacidad de asociar una plantilla de grupo con un grupo, se podía seleccionar un proceso de aprobación específico de grupo en la plantilla, pero no se podía hacer en los Detalles de cola o en los Temas de cola de la plantilla.

Para obtener más información, consulte [Asociar un proceso de aprobación nuevo o existente con el trabajo](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
