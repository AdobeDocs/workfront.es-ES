---
title: 22.1 Mejoras del administrador
description: 22.1 Mejoras del administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1452'
ht-degree: 0%

---

# 22.1 Mejoras del administrador

Esta página describe todas las mejoras realizadas por el administrador con la versión 22.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción de

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 17 de enero de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.1, consulte [Información general sobre la versión 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Descargas de documentos registradas en el área de Actualizaciones

Para ayudar a los usuarios a realizar un seguimiento de las descargas de documentos que almacenan en Workfront, el sistema registra ahora una entrada en el área de Actualizaciones de un documento cuando alguien lo descarga.

>[!NOTE]
>
>Se recomienda probar esta función en Vista previa en un documento recién cargado.

Para obtener información sobre cómo Workfront registra las actualizaciones automáticas de los objetos, consulte [Actualizaciones con seguimiento del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Conceder acceso a los equipos que utilizan niveles de acceso

Una nueva sección en el área de Niveles de acceso le proporciona controles más granulares para administrar el acceso de los usuarios a los equipos. Ahora puede determinar quién puede crear, editar y ver equipos.

Esto no cambia el acceso existente de los usuarios a los equipos.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## La asignación de grupos ya está disponible en los modelos

Algunos modelos ahora incluyen grupos, que puede personalizar antes de instalar el modelo. Puede asignar un grupo del modelo a un grupo existente en la instancia de Workfront o crear un grupo nuevo si es necesario.

Para obtener más información, consulte [Configurar un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Actualizaciones de estilo en el área de Forms personalizado

El área de Forms personalizado tiene un nuevo aspecto que la pone al día con muchas otras áreas de la nueva experiencia de Workfront.

## Muchas mejoras para crear campos personalizados calculados

Crear campos personalizados calculados ahora es mucho más fácil con estas adiciones en el nuevo Editor de cálculos:

* Puede situarse sobre cualquier expresión del cálculo para mostrar información sobre ella, incluida una descripción, un ejemplo de cómo se puede utilizar y un vínculo a más información en un artículo de ayuda.
* Cada expresión que agregue estará codificada por colores, según su tipo. Esto facilita la detección de expresiones y el reconocimiento inmediato de su tipo.
* Los números de línea ayudan a identificar y hacer referencia a funciones en un cálculo largo.
* Cuando empieza a escribir una expresión o un nombre de campo, se muestra una lista de elementos disponibles para que pueda elegir el que desee. Y, al escribir un paréntesis de apertura, el paréntesis de cierre se agrega automáticamente.
* Puede obtener una vista previa del resultado del cálculo utilizando un objeto existente sin salir del editor de cálculos.

Además, en el texto &quot;Instrucciones&quot; personalizable que pasa por encima de un campo personalizado calculado, puede mostrar u ocultar la fórmula del campo. Esto resulta útil si cree que los usuarios que rellenen el formulario personalizado no necesitarán esa información.

## Ver información de registro de auditoría sobre estados y compañías

Ahora puede solucionar más fácilmente los incidentes que implican estados y compañías consultando información sobre ellos en el área Registros de auditoría en Configuración.

Por ejemplo:

* Puede averiguar quién cambió el nombre, bloqueó u ocultó un estado y cuándo lo hizo.
* Puede averiguar quién eliminó algunos miembros o roles de trabajo de una compañía y cuándo lo hicieron.

Para obtener información acerca de cómo ver la información del registro de auditoría, vea [Ver y exportar registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Modelos de asignación de empresas y otras mejoras

Ya están disponibles las siguientes mejoras de modelos:

* Algunos modelos ahora incluyen compañías que puede personalizar antes de instalar el modelo. Puede asignar una compañía del modelo a una compañía existente en la instancia de Workfront o crear una nueva si es necesario.
* Ya está disponible un nuevo tipo de modelo, Estructura organizativa. Algunos modelos incluyen elementos de varios tipos (por ejemplo, plantilla de proyecto y estructura organizativa). Puede filtrar por tipo de modelo en la página del catálogo.
* Las secciones &quot;Instalar preferencias&quot; y &quot;Propiedad de la plantilla&quot; de la página de configuración se han combinado en &quot;Preferencias de plantilla&quot; para simplificar.

Para obtener más información, consulte [Configurar un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Administrar las suscripciones a compañías más fácilmente

En el área Compañías, una barra de herramientas actualizada facilita la adición de usuarios de Workfront existentes a una compañía y la eliminación de miembros de la compañía.

Anteriormente, estas acciones solo estaban disponibles en el cuadro Editar compañía.

La barra de herramientas actualizada también contiene todas las acciones disponibles en la barra de herramientas anterior, como editar la información de perfil de usuario de los miembros y desactivarlos en el sistema.

Para obtener más información, consulte [Administrar suscripciones a compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Seleccione expresiones y campos en la nueva ventana de campo calculado

Seguimos facilitando la creación de un campo calculado en un formulario personalizado. Ahora, al hacer clic en Maximizar para abrir el nuevo Editor de cálculos, puede buscar y seleccionar las expresiones y los campos que necesite.

## Los grupos pueden configurar sus propias preferencias de horas y hojas de horas

>[!NOTE]
>
>Esta característica estaba disponible inicialmente como parte de un despliegue gradual solo para clientes del clúster 4 como parte de la versión 21.4. Esta función estará disponible para todos los clústeres restantes de Producción el 8 de noviembre de 2021.

En una organización grande, es posible que algunos grupos necesiten configurar las preferencias de horas y de plantillas de horas de forma independiente para ajustarse a sus flujos de trabajo únicos, en lugar de heredar las preferencias configuradas por un administrador a nivel de sistema. Ahora los administradores de Workfront pueden desbloquear una plantilla de horas y una preferencia de horas para todos los grupos del sistema y así poder configurarlas ellos mismos.

Esta capacidad también se ha agregado recientemente para preferencias de proyecto y para preferencias de tarea y problema.

Para obtener información sobre cómo un administrador de Workfront desbloquea una hoja de horas y preferencias de horas, consulte la sección [Desbloquear hoja de horas y preferencias de horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) en el artículo [Configurar preferencias de horas y hojas de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obtener información sobre cómo un administrador de grupo configura las preferencias de tareas y problemas desbloqueados para un grupo, consulte [Configurar las preferencias de horas y hojas de horas para un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Seleccione varias notificaciones que desee desbloquear o volver a bloquear para grupos

Ahora es más rápido y fácil desbloquear o volver a bloquear las notificaciones por correo electrónico para los grupos. Ahora puede seleccionar varias notificaciones, comprobar las selecciones para asegurarse de que son correctas y, a continuación, hacer clic en el nuevo botón Desbloquear o Bloquear que se muestra en la barra de herramientas.

Anteriormente, tenía que desbloquear y volver a bloquear las notificaciones de una en una. Workfront tiene actualmente 95 notificaciones, por lo que tardó un tiempo si tenía que hacerlo para todas o muchas de ellas.

Para obtener más información, consulte [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Para administradores de grupos: es más fácil seleccionar un grupo de reemplazo cuando se elimina un grupo

Al eliminar un grupo, dos mejoras en el cuadro Eliminar grupo facilitan la selección del grupo de reemplazo que desea que conserve los usuarios, elementos de trabajo y subgrupos del grupo eliminado:

* Puede empezar a escribir el nombre del grupo para encontrarlo rápidamente. Anteriormente, solo había una lista desplegable en la que no se podía escribir. Esto resultaba problemático para las organizaciones con muchos grupos, ya que había que desplazarse por la lista para encontrar el grupo deseado. Además, la lista desplegable tenía un límite de elementos, por lo que era posible que el grupo que quería no se mostrara.
* Puede utilizar el icono de información nueva para asegurarse de que está seleccionando el grupo de sustitución que desea. Al pasar el ratón por encima del icono, se muestra información de objeto sobre el grupo, como la jerarquía de grupos que hay encima y los nombres de sus administradores.

Para obtener más información, vea [Eliminar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Área más grande para crear campos calculados

Ahora es más fácil crear campos calculados complejos en un formulario personalizado. Haga clic en el nuevo botón Maximizar para abrir una ventana de edición grande y generar el cálculo. Cuando haya terminado, haga clic en Minimizar para continuar trabajando en el formulario personalizado.

## Agregar formularios personalizados a grupos

Ahora se admiten formularios personalizados para el objeto Group. Esto facilita a los grupos de su organización la captura y el uso compartido de información que satisface sus necesidades y flujos de trabajo específicos. Los usuarios pueden hacer lo siguiente para un grupo, igual que para otros objetos de Workfront:

* Creación de un formulario personalizado
* Adjuntar un formulario personalizado
* Guardar datos de formulario personalizados
* Eliminación de un formulario personalizado
* Edite datos personalizados de listas y, en la nueva experiencia de Workfront, de la página Grupo

Para obtener información sobre formularios personalizados, consulte [Formularios personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Creación de aplicaciones de OAuth2 para integrar aplicaciones con Workfront

Ahora puede integrar Workfront con otras aplicaciones para las que Workfront no ofrece una integración integrada. Al crear una aplicación OAuth2 para la aplicación con la que desea integrar, puede permitir que esa aplicación acceda a Workfront, sabiendo al mismo tiempo que sus datos están protegidos por el protocolo de autenticación OAuth2 seguro y estándar del sector.

Anteriormente, solo se podía integrar con otras aplicaciones mediante integraciones integradas, Workfront Fusion o la API de Workfront.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Mejoras en el texto de la interfaz en el área Compañías

En el área Compañías de la Configuración, los nuevos mensajes de confirmación y los ligeros cambios de redacción facilitan la administración de las suscripciones a la empresa. Por ejemplo, el nombre de sección &quot;Personas&quot; en el panel izquierdo es ahora &quot;Miembros de la compañía&quot;.

Para obtener información sobre cómo administrar las suscripciones a compañías, consulte [Administrar suscripciones a compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
