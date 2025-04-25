---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 otras mejoras
description: En esta página se describen todas las demás mejoras realizadas en la versión 20.3 del entorno de producción. Estas mejoras estuvieron disponibles en el entorno de producción la semana del 10 de agosto de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 48%

---

# 20.3 otras mejoras

En esta página se describen todas las demás mejoras realizadas en la versión 20.3 del entorno de producción. Estas mejoras estuvieron disponibles en el entorno de producción la semana del 10 de agosto de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.3, consulte [Información general de la versión 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Compartir un calendario con un vínculo privado

Para aliviar la carga que supone compartir calendarios en Workfront, puede compartir un vínculo privado que lleva a los usuarios directamente al calendario. El calendario debe compartirse con el usuario y este tiene que iniciar sesión para verlo.

Anteriormente, se podía compartir una dirección URL pública que no requería iniciar la sesión para verla.

Para obtener más información, vea [Compartir un informe de calendario](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Área de nuevos borradores al crear solicitudes

Para ofrecerle una mayor flexibilidad a la hora de trabajar con solicitudes, Workfront guarda ahora automáticamente todas las solicitudes que crea como borrador en la nueva área Borradores. Si no tiene toda la información necesaria para completar la nueva solicitud, puede dejarla como borrador, volver a ella y terminarla más tarde. Workfront guarda una solicitud por tema de la cola en la nueva área Borradores. Las solicitudes de borrador se pueden guardar durante el tiempo que las necesite hasta que esté listo para completarlas y enviarlas. También puede quitar o cambiar la posición del área Borradores del panel izquierdo mediante una plantilla de diseño.

Para obtener más información sobre la creación de solicitudes, consulte [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Para la versión Vista previa, si tiene asignada una plantilla de diseño personalizada, deberá añadir el área Borradores de las solicitudes modificando la plantilla de diseño.

## Expandir o contraer elementos en la hoja de horas

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Para ayudarle a administrar fácilmente las plantillas de horas con varios elementos, ahora puede expandir o contraer todos los elementos con solo hacer clic en un botón.

Anteriormente, tenía que hacer clic en cada elemento individualmente.

Para obtener más información, consulte [Registrar tiempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Omitir fechas reales en calendarios de Workfront

>[!NOTE]
>
>Esta función se publicó en el entorno de vista previa el 5 de junio de 2020. Estará disponible en el entorno de producción el 19 de junio de 2020.

Para controlar mejor cómo se muestran los objetos en los informes del calendario, puede optar por omitir las fechas reales incluso cuando estén disponibles.

Anteriormente, el calendario utilizaba automáticamente las fechas reales una vez que estaban disponibles.

Para obtener más información, consulte [Resumen de informes del calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Usar campos de fecha personalizados en informes de calendario

>[!NOTE]
>
>Esta función se publicó en el entorno de vista previa el 29 de mayo de 2020. Estará disponible en el entorno de producción el 12 de junio de 2020.

Para ayudarle a visualizar y administrar mejor su trabajo diario con los calendarios, los campos de fecha personalizados ahora están disponibles como una opción de fecha.

Anteriormente, el calendario solo se podía administrar con fechas proyectadas y planificadas cuando las fechas reales no estaban disponibles.

Para obtener más información, consulte [Usar campos de fecha personalizados en un informe de calendario](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (o si usa Workfront Classic, vea [Usar campos de fecha personalizados en un informe de calendario](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

## Cambios de correo electrónico

**Cambios en el correo electrónico saliente:** Todo el correo electrónico de Workfront provendrá de notifications@my.workfront.com. Esto incluye alertas automatizadas y comunicación entre usuarios.

Anteriormente, los administradores del sistema podían agregar una dirección de correo electrónico personalizada en el área Configuración de correo electrónico.

**Cambios en la respuesta POP de correo electrónico entrante:** Los administradores del sistema ya no podrán configurar un servidor de correo electrónico POP personalizado para las respuestas de correo electrónico entrantes a las notificaciones.

Para obtener más información, consulte [suplantación de correo electrónico y cambios en el correo electrónico de respuesta POP](https://experienceleague.adobe.com/en/docs/workfront/using/home).

## DomainKeys Identified Mail (DKIM) ahora se incluye en los correos electrónicos salientes de Workfront

Se incluirá una técnica de autenticación de correo electrónico (DKIM) en todos los correos electrónicos salientes. Esta firma DKIM no es visible para el usuario final, pero permite la validación en el nivel de servidor y refuerza el marco de autenticación existente.

## Actualizaciones para inscribirse en la nueva experiencia de Workfront

Para que la inscripción de usuarios en la nueva experiencia de Workfront sea más manejable, los administradores de grupos ahora tienen acceso para inscribir y dar de baja a usuarios que pertenecen a los grupos que administran.

Ahora también hay un vínculo de Detalles del usuario que muestra la siguiente información del usuario:

* Nombre
* Función
* Dirección de correo electrónico
* Imagen de perfil

## Nuevo para administradores: Brand Workfront para grupos, equipos, roles y usuarios específicos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Ahora puede utilizar una plantilla de diseño para cambiar los logotipos en el área de navegación superior y en el menú principal para grupos, equipos, funciones y usuarios específicos que tengan su propia marca.

Para obtener más información, consulte [Crear una marca para su instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Los administradores de grupo pueden crear y administrar procesos de aprobación

Para permitir una mayor autonomía y control de los flujos de trabajo de sus grupos, un administrador de grupos ahora puede acceder al área Proceso de aprobación en Configuración y crear y editar los procesos de aprobación para un grupo que administra. Estos procesos de aprobación se basan en los estados de ese grupo.

Para garantizar que los administradores de grupo no editen de forma involuntaria los procesos de aprobación que se utilizan en todo el sistema o que crean otros grupos, solo pueden acceder a los procesos de aprobación asociados con los grupos que administran.

Para obtener más información, consulte [Crear un proceso de aprobación de elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Para administradores: la página Nuevos grupos facilita la creación y administración de grupos

Los administradores de grupos pueden administrar grupos más fácilmente ahora que todo lo que necesitan está en la nueva página Grupos. Ya no es necesario desplazarse entre los distintos cuadros de superposición y las páginas de configuración para crear y modificar grupos.

Estos son los aspectos destacados:

* Detalles del grupo: vea y edite información básica sobre el grupo, como su nombre, descripción, nombres de administradores del grupo y si el grupo es público o privado.
* Lista de miembros del grupo: vea todos los miembros del grupo y utilice la nueva barra de herramientas para agregar, quitar, exportar, activar y desactivar pertenencias rápidamente. También puede editar los perfiles de los miembros y enviarles comentarios de actualización.
* Campo Administrador de grupos en la cabecera: Cuando visualice un grupo que gestione, asigne o anule rápidamente la asignación de un miembro del grupo como administrador del grupo. También puede hacerlo en la lista de miembros del grupo mediante la nueva columna Función del grupo.
* Lista de subgrupos: vea, edite, copie, exporte y elimine los subgrupos de un grupo que administre.
* Lista de estados: vea y administre los estados de su grupo.

Para obtener más información, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Nuevo para administradores: crear hasta 14 niveles de subgrupos.

Para facilitar la organización de los grupos de Workfront de modo que coincidan con la jerarquía de la organización, hemos aumentado los niveles de subgrupos que puede crear dentro de un grupo de 3 a 14.

Para obtener más información, consulte [Información general sobre los grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Nuevo para administradores: nueva barra lateral de configuración

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

La barra lateral izquierda de la Configuración ahora es más rápida y fácil de usar y aprovecha el diseño y la funcionalidad básicos que ya conoce. Además de un aspecto más moderno, esto es lo que hay de nuevo:

* Un nuevo fondo en blanco roto en la barra lateral facilita la diferenciación del resto del área de configuración.
* Los iconos de la barra lateral son un poco más grandes y algunos se han rediseñado para sugerir con mayor claridad lo que hace la opción.
* Un espacio más vertical entre los elementos de la barra lateral facilita su lectura.
* Puede contraer la barra lateral cuando necesite espacio en el área principal para ver y hacer más, como ver columnas adicionales. Y puede expandir la barra lateral nuevamente cuando necesite ver los nombres de las características.
* Mientras la barra lateral está contraída, solo verá los iconos de cada función. Para ver los subelementos debajo de un elemento de la barra lateral principal, pase el ratón sobre su icono para mostrarlos en un menú flotante. Por ejemplo, pase el ratón sobre el icono Procesos para mostrar un menú que contenga Aprobaciones y Rutas de hitos.
* Puede acceder a las dos opciones de Kick-Starts (Importar datos y Exportar datos) con un clic más rápido. Se han movido desde Sistema para mostrarse en el nivel principal de la barra lateral.

Para obtener información sobre cómo usar el área de configuración, consulte [Administración y configuración](../../../administration-and-setup/administration-and-setup.md).

## Incluir número de clúster en el área Información del cliente

Como administrador de Workfront, ahora puede encontrar fácilmente el número de clúster dentro de Workfront sin tener que dedicar tiempo ni esfuerzo adicionales a obtenerlo de nuestro equipo de soporte. Hemos añadido un campo Configuración de clúster en el área Información del cliente de Configuración.

Para obtener información acerca del área Información del cliente, vea [Configurar información básica para el sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Codificación Base64 para suscripciones a eventos

El campo base64Encoding es un campo opcional que se utiliza para habilitar la codificación Base64 de las cargas útiles de suscripción a eventos. Si se realiza una solicitud utilizando el campo base64Encoding establecido en true, los objetos newState y oldState de la carga útil se ofrecen como cadenas de codificación en Base64. Esta función puede resultar útil si la red está configurada de tal manera que no permite caracteres especiales en las suscripciones a eventos.

Para obtener más información, consulte [API de suscripción a evento](../../../wf-api/general/event-subs-api.md).

## Se ha eliminado la capacidad de crear suscripciones de eventos duplicadas

Para evitar la entrega de mensajes duplicados, ya no puede crear suscripciones duplicadas. Además, se han eliminado todas las suscripciones duplicadas creadas anteriormente.

Para obtener más información, consulte [Preguntas más frecuentes - Suscripciones de eventos](../../../wf-api/general/event-subs-faq.md).
