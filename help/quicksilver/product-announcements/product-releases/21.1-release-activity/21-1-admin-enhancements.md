---
content-type: release-notes
keywords: notas,trimestral,actualizar
navigation-topic: product-releases
title: 21.1 Mejoras del administrador
description: Esta página describe todas las mejoras realizadas por el administrador con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 15 de febrero de 2021.
author: Luke
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 4048f8b5-70e2-4d63-ae64-a4fbf91a57df
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# 21.1 Mejoras del administrador

Esta página describe todas las mejoras realizadas por el administrador con la versión 21.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción el 15 de febrero de 2021.

Para obtener una lista de todos los cambios disponibles con la versión 21.1, consulte [Información general sobre la versión 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Introducir nueva configuración de nivel de acceso para copiar proyectos

Para darle más control, como administrador del sistema, sobre lo que los planificadores pueden hacer con un proyecto, hemos hecho que el acceso de edición a proyectos en el nivel de acceso sea más granular, al introducir una nueva configuración que le permite habilitar o deshabilitar su capacidad para copiar proyectos. Antes de este cambio, cuando habilitaba el acceso de los usuarios a Editar proyectos, automáticamente tenían acceso para copiarlos. Con la nueva función, puede otorgar acceso a alguien para editar proyectos sin tener necesariamente acceso para copiarlos deshabilitando la nueva configuración Copiar.

Si los usuarios tenían acceso a Editar proyectos en su nivel de acceso antes de este cambio, automáticamente tendrán esta configuración habilitada cuando se publique esta función.

Para obtener información sobre el nivel de acceso del plan, consulte [Conceder acceso a proyectos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Para obtener información sobre cómo copiar un proyecto, vea [Copiar un proyecto](../../../manage-work/projects/manage-projects/copy-project.md).

Esta característica ahora se incluye en [Aspectos básicos del administrador en la nueva experiencia de Workfront, Parte 1: Organización del usuario](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) ruta de aprendizaje en Workfront One.

## En un formulario personalizado de un objeto, seleccione todos los elementos en un campo desplegable de selección múltiple

>[!NOTE]
>
>Esta funcionalidad no está disponible actualmente al enviar una nueva solicitud.

En la página Detalles de un objeto, cuando rellene un campo desplegable de selección múltiple en un formulario personalizado, puede hacer clic en Seleccionar todo si necesita seleccionar todas las opciones disponibles.

Para obtener información sobre cómo editar datos en un formulario personalizado, consulte [Editar información en campos de formulario personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Volver a calcular todos los campos de formulario personalizados de un objeto

Ahora es más fácil asegurarse de que todos los datos de los campos personalizados calculados estén actualizados para un objeto. La nueva opción de menú Recalcular expresiones permite volver a calcular rápidamente todos los datos de estos campos.

Esto resulta especialmente útil después de que alguien edite datos en otro objeto al que se hace referencia mediante un campo personalizado calculado en el objeto.

Anteriormente, los usuarios tenían que usar soluciones alternativas para asegurarse de que todos los datos de los campos personalizados calculados estuvieran actualizados. Por ejemplo, editaron el objeto junto con otros objetos para utilizar la opción de recálculo que está disponible para la edición masiva.

Para obtener más información, consulte [Editar información en campos de formulario personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Desbloquear las preferencias de tareas y problemas para los administradores de grupos

>[!NOTE]
>
>Hasta el 24 de junio de 2021, esto estaba disponible como parte de un despliegue gradual solo para clientes que tengan la capacidad de desbloquear las preferencias de proyecto para grupos. Ahora está disponible para todos los clientes.

Los administradores de Adobe Workfront ahora pueden dar más autonomía a los administradores de grupos desbloqueando las preferencias de tareas y problemas individuales. Cuando una preferencia está desbloqueada, los administradores de grupos pueden configurarla para que sus grupos sirvan a las necesidades únicas y a los procesos internos de cada grupo.

Para obtener más información, consulte [Configurar las preferencias de tareas y problemas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

Esta característica ahora se incluye en [Aspectos básicos del administrador en la nueva experiencia de Workfront, Parte 2: Configuración del proyecto](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-1-project-workfl-MCTBVZ3Q3J5RHNLIPPZPFSQRLKUY) ruta de aprendizaje en Workfront One.

## Configurar por separado el nivel de acceso para portafolios y programas

Ahora es más fácil administrar el acceso de los usuarios a portafolios y programas porque puede establecer la configuración de su nivel de acceso por separado.

Anteriormente, se combinaba la configuración del nivel de acceso para portafolios y programas. Esto significaba que no se podía establecer la configuración de acceso para los programas sin configurarlos de la misma manera para los portafolios, y lo mismo ocurría al revés.

Para obtener información acerca de cómo configurar un nivel de acceso, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Para obtener información acerca de la configuración de acceso que puede configurar para programas y portafolios, vea [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Esta característica ahora se incluye en [Aspectos básicos del administrador en la nueva experiencia de Workfront, Parte 1: Organización del usuario](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) ruta de aprendizaje en Workfront One.

## Seleccionar todas las casillas de verificación de una serie al editar información en un formulario personalizado

>[!NOTE]
>
>Esta funcionalidad no está disponible actualmente al enviar una nueva solicitud.

En la página Detalles de un objeto, cuando rellene un campo Formulario personalizado que contenga casillas de verificación, puede hacer clic en Seleccionar todo si necesita seleccionar todas las casillas de verificación disponibles.

Esta opción solo se muestra si el campo contiene más de dos casillas de verificación.

Para obtener más información, consulte [Editar información en campos de formulario personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

## Configuración de la lista de permitidos de correo electrónico de Workfront

Para proteger mejor sus datos, ahora puede utilizar una lista de permitidos de dominio de correo electrónico para lo siguiente:

* Controlar adónde pueden ir los correos electrónicos de Workfront si contienen informes o documentos almacenados en Workfront
* Los dominios de control de correo electrónico pueden estar en la dirección de correo electrónico que los usuarios pueden especificar en su perfil de usuario

Por ejemplo, si desea proteger datos confidenciales, como un informe que enumere los clientes en riesgo, puede incluir solo el dominio o los dominios de correo electrónico internos en la lista de permitidos de correo electrónico. De este modo, los usuarios no podrán enviar dicho informe (ni ningún otro informe de Workfront) a una dirección de correo electrónico externa.

Para obtener más información, consulte la sección [Configuración de la lista de permitidos del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md#configur) en el artículo [Configuración de la lista de permitidos del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Asignar un administrador de grupo para un subgrupo

Para facilitar el funcionamiento independiente de los niveles de su organización, se ha añadido la capacidad de asignar un administrador de grupo a un subgrupo. Ahora puede asegurarse de delegar la administración de subgrupos a las personas adecuadas.

Anteriormente, solo un grupo de nivel superior podía tener Administradores de grupo y estos administradores administraban todos los subgrupos debajo del grupo de nivel superior.

Para obtener más información, consulte la sección [Administradores de grupos para subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md#for) en el artículo [Información general sobre subgrupos](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

Esta característica ahora se incluye en [Aspectos básicos del administrador en la nueva experiencia de Workfront, Parte 1: Organización del usuario](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) ruta de aprendizaje en Workfront One.

## Configuración de notificaciones de eventos para grupos

>[!NOTE]
>
>Disponible como parte de un despliegue gradual, solo para clientes que tengan la capacidad de desbloquear las preferencias de proyecto de los grupos. Esto incluye a todos los clientes de los clústeres 4 y 6 y a un pequeño número de clientes de otros clústeres. Esta nota se actualizará a medida que la funcionalidad esté disponible para más clústeres.

Los administradores de Workfront ahora pueden dar más autonomía a los administradores de grupos, ya que les permite configurar notificaciones de eventos para sus grupos de nivel superior. Los subgrupos heredan las configuraciones de notificación de eventos de su grupo principal superior.

Anteriormente, solo un administrador de Workfront podía configurar las notificaciones de eventos en el sistema, lo que significa que todos los grupos tenían que utilizar el mismo conjunto de notificaciones de eventos.

Para obtener más información, consulte los siguientes artículos:

* [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)
* [Visualización y configuración de notificaciones de eventos para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)

Esta característica ahora se incluye en [Aspectos básicos del administrador en la nueva experiencia de Workfront, Parte 1: Organización del usuario](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-MCUPSLH2M2WBDTFI2VKSRE2BRGKY) ruta de aprendizaje en Workfront One.

Esta característica ahora se incluye en [Notificaciones por correo electrónico y en la aplicación en la nueva ruta de aprendizaje de la experiencia Workfront](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-MCDSDH3SRJ4ZGTJF5NJI64F4TW2U) en Workfront One.

## Trabajar con proyectos de grupo y procesos de aprobación en el área de Grupos

Si es administrador de grupos, es fácil ver y trabajar con los proyectos y procesos de aprobación de su grupo ahora que están enumerados en el área de Grupos. Desde la página principal de un grupo, puede:

* Haga clic en Proyectos en el menú de la izquierda para ver los proyectos del grupo y crear otros nuevos para el grupo. Si se ha compartido un proyecto seleccionado con usted, puede utilizar los botones de la barra de herramientas para editarlo, exportarlo, copiarlo o eliminarlo.

  Para obtener más información, vea [Crear y modificar proyectos de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

* Haga clic en Aprobaciones en el menú de la izquierda para ver y administrar todos los procesos de aprobación asociados con el grupo.

  Para obtener más información, consulte [Procesos de aprobación de nivel de grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

Esta funcionalidad también está disponible para los administradores de Workfront.

## Ver el número de licencias utilizadas y asignadas en un grupo

Para determinar cómo se distribuyen las licencias, ahora puede ver el número de licencias que se usan en un grupo y en los subgrupos que haya debajo de él.

Si administra un grupo de nivel superior, puede ver tanto el número de licencias que se usan en un grupo (y sus subgrupos) como el número máximo de licencias asignadas para el grupo.

Para obtener más información, consulte [Ver el número de licencias asignadas y utilizadas en un grupo en la nueva experiencia de Adobe Workfront](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

