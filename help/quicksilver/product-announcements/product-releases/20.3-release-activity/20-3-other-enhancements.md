---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: Otras mejoras de la versión 20.3
description: En esta página se describen todas las demás mejoras realizadas con la versión 20.3 en el entorno Producción. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 10 de agosto de 2020.
author: Luke
feature: Product Announcements
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 0%

---

# Otras mejoras de la versión 20.3

En esta página se describen todas las demás mejoras realizadas con la versión 20.3 en el entorno Producción. Estas mejoras estaban disponibles en el entorno Producción durante la semana del 10 de agosto de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 20.3, consulte [Información general sobre la versión 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Compartir un calendario con un vínculo privado

Para aliviar la carga de compartir calendarios en Workfront, puede compartir un vínculo privado que lleve a los usuarios directamente al calendario. El calendario debe compartirse con el usuario, que debe iniciar sesión para verlo.

Anteriormente, se podía compartir una URL pública que no requería un inicio de sesión para visualizarla.

Para obtener más información, consulte [Compartir un informe de calendario](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Nueva área Borradores al crear solicitudes

Para proporcionar una mayor flexibilidad al trabajar con solicitudes, Workfront ahora guarda automáticamente todas las solicitudes que cree como borrador en el nuevo área Borradores . Si no dispone de toda la información necesaria para completar la nueva solicitud, puede dejarla como borrador, volver a ella y terminarla más tarde. Workfront guarda una solicitud por tema de cola en el nuevo área Borradores . Los borradores de solicitudes se pueden guardar durante el tiempo que los necesite hasta que esté listo para completarlos y enviarlos. También puede quitar o cambiar la posición del área Borradores del panel izquierdo mediante una plantilla de diseño.

Para obtener más información sobre la creación de solicitudes, consulte [Crear y enviar solicitudes de Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Para la versión de vista previa, si tiene una plantilla de diseño personalizada asignada, deberá agregar el área Borradores de las solicitudes modificando la plantilla de diseño.

## Expandir o contraer elementos en el parte de horas

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Para facilitar la administración de partes de horas con varios elementos, ahora puede expandir o contraer todos los elementos con solo hacer clic en un botón.

Anteriormente, había que hacer clic en cada elemento individualmente.

Para obtener más información, consulte [Tiempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Omitir fechas reales en calendarios de Workfront

>[!NOTE]
>
>Esta función se publicó en el entorno de vista previa el 5 de junio de 2020. Estará disponible en el entorno Producción el 19 de junio de 2020.

Para darle más control sobre cómo se muestran los objetos en los informes de calendario, puede optar por ignorar las fechas reales incluso cuando estén disponibles.

Anteriormente, el calendario utilizaba automáticamente las fechas reales una vez que estaban disponibles.

Para obtener más información, consulte [Información general sobre los informes del calendario](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Usar campos de fecha personalizados en informes de calendario

>[!NOTE]
>
>Esta función se publicó en el entorno de vista previa el 29 de mayo de 2020. Estará disponible en el entorno Producción el 12 de junio de 2020.

Para ayudarle a visualizar y administrar mejor su trabajo diario con calendarios, los campos de fecha personalizados ya están disponibles como opción de fecha.

Anteriormente, solo se podía administrar el calendario con fechas planificadas y proyectadas cuando las fechas reales no estaban disponibles.

Para obtener más información, consulte [Usar campos de fecha personalizados en un informe de calendario](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (o si utiliza Workfront Classic, consulte [Usar campos de fecha personalizados en un informe de calendario](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US)).

## Cambios en el correo electrónico

**Cambios en el correo electrónico de salida:** Todos los correos electrónicos de Workfront provienen de notifications@my.workfront.com. Esto incluye alertas automatizadas y comunicación entre usuarios.

Anteriormente, los administradores del sistema podían añadir una dirección de correo electrónico personalizada en el área Configuración del correo electrónico .

**Cambios en la respuesta POP de correo electrónico entrante:** Los administradores del sistema ya no tendrán la capacidad de configurar un servidor de correo electrónico POP personalizado para las respuestas de correo electrónico entrantes a las notificaciones.

Para obtener más información, consulte [Cambios en el correo electrónico de respuesta POP y de suplantación de correo electrónico](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## Correo identificado de DomainKeys (DKIM) ahora se incluye en los correos electrónicos salientes de Workfront

Se incluirá una técnica de autenticación por correo electrónico (DKIM) en todos los correos electrónicos salientes. Esta firma DKIM no es visible para el usuario final, pero permite la validación a nivel de servidor y refuerza nuestro marco de autenticación existente.

## Actualizaciones de la inscripción en la nueva experiencia de Workfront

Para que la inscripción de usuarios en la nueva experiencia de Workfront sea más manejable, los administradores de grupos ahora tienen acceso para inscribir y cancelar la inscripción de usuarios que pertenecen a los grupos que administran.

Ahora también hay un vínculo de detalles del usuario que muestra la siguiente información del usuario:

* Nombre
* Función del trabajo
* Dirección de correo electrónico
* Imagen de perfil

## Novedades para administradores: Brand Workfront para grupos, equipos, funciones de trabajo y usuarios específicos

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

Ahora puede utilizar una plantilla de diseño para cambiar los logotipos en el área de navegación superior y en el menú principal para grupos específicos, equipos, funciones de trabajo y usuarios que tengan su propia marca.

Para obtener más información, consulte [Marca la instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Los administradores de grupo pueden crear y administrar procesos de aprobación

Para permitir una mayor autonomía y control de los flujos de trabajo de sus grupos, un administrador de grupo ahora puede acceder al área Proceso de aprobación en Configuración y crear y editar procesos de aprobación para un grupo que administra. Estos procesos de aprobación se basan en los estados de ese grupo.

Para garantizar que los administradores de grupo no editen involuntariamente los procesos de aprobación que se utilizan en todo el sistema o que otros grupos los crean, solo pueden acceder a los procesos de aprobación asociados a los grupos que administran.

Para obtener más información, consulte [Creación de un proceso de aprobación para elementos de trabajo](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Para administradores: La página Nuevos grupos facilita la creación y administración de grupos

Los administradores de grupos pueden administrar los grupos más fácilmente ahora que todo lo que necesitan está en la nueva página Grupos . Ya no es necesario navegar entre varios cuadros de superposición y páginas de configuración para crear y modificar grupos.

Aquí están los aspectos más destacados:

* Detalles del grupo: Vea y edite información básica sobre el grupo, como el nombre del grupo, la descripción, los nombres de los administradores del grupo y si el grupo es público o privado.
* Lista de miembros del grupo: Vea todos los miembros del grupo y utilice la nueva barra de herramientas para agregar, quitar, exportar, activar y desactivar suscripciones rápidamente. También puede editar los perfiles de los miembros y enviarles comentarios de actualización.
* Campo Administrador de grupo en el encabezado: Cuando visualice un grupo que administra, asigne o quite la asignación rápidamente de un miembro del grupo como administrador del grupo. También puede hacerlo en la lista de miembros del grupo utilizando la nueva columna Función del grupo .
* Lista de subgrupos: Ver, editar, copiar, exportar y eliminar los subgrupos en un grupo que administra.
* Lista de estados: Vea y administre los estados de su grupo.

Para obtener más información, consulte [Crear un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Novedades para administradores: Crear hasta 14 niveles de subgrupos

Con el fin de facilitar la organización de los grupos de Workfront para que coincidan con la jerarquía de su organización, hemos aumentado los niveles de subgrupos que puede crear en un grupo de 3 a 14.

Para obtener más información, consulte [Información general sobre grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Novedades para administradores: Nueva barra lateral de configuración

>[!NOTE]
>
>Esta función solo está disponible en la nueva experiencia de Adobe Workfront

La barra lateral izquierda en Configuración es ahora más rápida y fácil de usar y aprovecha el diseño y la funcionalidad básicos que ya conoce. Junto con una apariencia más moderna, aquí está lo que más es nuevo:

* Un nuevo fondo blanquecino en la barra lateral facilita la diferenciación del resto del área de configuración.
* Los iconos de la barra lateral son un poco más grandes y algunos se han rediseñado para sugerir con mayor claridad lo que hace la opción.
* Un espacio vertical más amplio entre los elementos de la barra lateral facilita su lectura.
* Puede contraer la barra lateral cuando necesite espacio en el área principal para ver y hacer más, como ver columnas adicionales. Y puede volver a expandir la barra lateral cuando necesite ver los nombres de las funciones.
* Mientras la barra lateral está contraída, solo verá los iconos de cada función. Para ver los subelementos debajo de un elemento principal de la barra lateral, pase el ratón sobre su icono para mostrarlos en un menú flotante. Por ejemplo, pase el ratón sobre el icono Procesos para mostrar un menú que contiene Aprobaciones y Rutas de hitos.
* Puede acceder a las dos opciones Inicio rápido (Importar datos y Exportar datos) un clic más rápido. Se han desplazado de Sistema para mostrarse en el nivel principal de la barra lateral.

Para obtener información sobre cómo utilizar el área de configuración, consulte [Administración y configuración](../../../administration-and-setup/administration-and-setup.md).

## Incluir número de clúster en el área Información del cliente

Como administrador de Workfront, ahora puede encontrar fácilmente el número de clúster dentro de Workfront, sin tener que dedicar más tiempo y esfuerzo a obtenerlo de nuestro equipo de asistencia. Hemos agregado un campo Configuración de clúster en el área Información del cliente de Configuración.

Para obtener información sobre el área Información del cliente, consulte [Configurar información básica para el sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Codificación Base64 para suscripciones de eventos

El campo base64Encoding es un campo opcional que se utiliza para habilitar la codificación Base64 de las cargas de suscripción de eventos. Si se realiza una solicitud utilizando el campo base64Encoding establecido en true, los objetos newState y oldState de la carga útil se envían como cadenas de codificación Base64. Esta función puede resultar útil si la red está configurada de forma que no permita caracteres especiales en Suscripciones de eventos.

Para obtener más información, consulte [API de suscripción de evento](../../../wf-api/general/event-subs-api.md).

## Se ha eliminado la capacidad de crear suscripciones de eventos duplicadas

Para evitar el envío de mensajes duplicados, ya no se pueden crear suscripciones duplicadas. Además, se han eliminado todas las suscripciones duplicadas creadas anteriormente.

Para obtener más información, consulte [Preguntas más frecuentes: Suscripciones a eventos](../../../wf-api/general/event-subs-faq.md).
