---
title: Mejoras del administrador en la versión 22.1
description: Mejoras del administrador en la versión 22.1
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
TQID: https://experienceleague.adobe.com/5OkRMNtGZPFq3UTOlmP9rUqvkdkxrB4Eo6Gh-culwZw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: a29813d3-f0cc-4b60-9396-13b558370803id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1466
ht-degree: 100%

---

# Mejoras del administrador en la versión 22.1

En esta página se describen todas las mejoras realizadas por el administrador con la versión 22.1 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 17 de enero de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.1, consulte [Información general sobre la versión 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Descargas de documentos registradas en el área de actualizaciones

Para ayudar a los usuarios a realizar un seguimiento de las descargas de documentos que se almacenan en Workfront, el sistema ya registra una entrada en el área de actualizaciones de los documentos cuando alguien los descarga.

>[!NOTE]
>
>Se recomienda probar esta función en Vista previa en un documento recién cargado.

Para obtener información sobre cómo Workfront registra las actualizaciones automáticas de los objetos, consulte [Actualizaciones con seguimiento del sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Concesión de acceso para los equipos que utilicen niveles de acceso

Una nueva sección en el área Niveles de acceso proporciona controles más granulares para administrar el acceso de los usuarios a los equipos. Ya es posible determinar quién puede crear, editar y ver equipos.

Esto no cambia el acceso existente de los usuarios a los equipos.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## La asignación de grupos ya está disponible en los modelos

Algunos modelos ya incluyen grupos, que se pueden personalizar antes de instalar el modelo. Asigne un grupo del modelo a un grupo existente en la instancia de Workfront o cree un grupo nuevo si fuera necesario.

Para obtener más información, consulte [Configurar un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Actualizaciones de estilo en el área Formularios personalizados

El área Formularios personalizados tiene una nueva apariencia que la pone al día respecto a muchas otras áreas de la nueva experiencia de Workfront.

## Muchas mejoras para la creación de campos personalizados calculados

La creación de campos personalizados calculados ahora es mucho más sencilla con estas adiciones en el nuevo Editor de cálculo:

* Pase el puntero por encima de cualquier expresión de cálculo para mostrar información sobre ella, incluyendo una descripción, un ejemplo de cómo se usa y un vínculo a más información en un artículo de ayuda.
* Cada expresión que añada estará codificada por colores, según su tipo. Esto facilita la detección de expresiones y el reconocimiento inmediato del tipo.
* Los números de línea ayudan a identificar y hacer referencia a funciones en cálculos largos.
* Al empezar a escribir una expresión o un nombre de campo, se muestra una lista de elementos disponibles para elegir el que se desee. Y al escribir un paréntesis de apertura, el paréntesis de cierre se añadirá automáticamente.
* Es posible obtener una vista previa del resultado del cálculo utilizando un objeto existente sin salir del editor de cálculo.

Además, en el texto personalizable “Instrucciones” que se muestra al pasar el puntero por encima de un campo personalizado calculado, es posible mostrar u ocultar la fórmula del campo. Esto resultará útil si se cree que los usuarios que rellenen el formulario personalizado no necesitarán esa información.

## Ver información de registro de auditoría sobre estados y compañías

Ya es posible solucionar más fácilmente los incidentes relacionados con estados y compañías, consultando información sobre ellos en el área Registros de auditoría, en Configuración.

Por ejemplo:

* Es posible saber quién cambió el nombre, bloqueó u ocultó un estado y cuándo lo hizo.
* Es posible averiguar quién eliminó algunos miembros o funciones de una compañía y cuándo se hizo.

Para obtener información acerca de cómo ver la información de registro de auditoría, consulte [Ver y exportar registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Modelos de asignación de compañías y otras mejoras

Ya están disponibles las siguientes mejoras de modelos:

* Algunos modelos ya incluyen compañías, que se pueden personalizar antes de instalar el modelo. Asigne una compañía del modelo a una compañía existente en la instancia de Workfront o cree una nueva si fuera necesario.
* Ya está disponible un nuevo tipo de modelo: estructura organizativa. Algunos modelos incluyen elementos de varios tipos (por ejemplo: plantilla de proyecto y estructura organizativa). Es posible filtrar por tipo de modelo en la página del catálogo.
* Las secciones “Instalar preferencias” y “Propiedad de la plantilla” de la página de configuración se combinaron en “Preferencias de plantilla” para una mayor simplicidad.

Para obtener más información, consulte [Configuración de modelos](../../../administration-and-setup/blueprints/configure-template-package.md).

## Administrar las suscripciones a compañías más fácilmente

En el área Compañías, una barra de herramientas actualizada facilita la adición de usuarios de Workfront existentes a una compañía y la eliminación de miembros de la misma.

Anteriormente, estas acciones solo estaban disponibles en el cuadro Editar compañía.

La barra de herramientas actualizada también contiene todas las acciones disponibles en la barra de herramientas anterior, como editar la información de perfil de usuario de los miembros y desactivarlos en el sistema.

Para obtener más información, consulte [Administrar suscripciones a compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Seleccionar expresiones y campos en la nueva ventana de campo calculado

Seguimos facilitando la creación de un campo calculado en un formulario personalizado. Ahora, al hacer clic en Maximizar para abrir el nuevo Editor de cálculos, puede buscar y seleccionar las expresiones y los campos que necesite.

## Los grupos pueden configurar sus propias preferencias de plantilla de horas y horas

>[!NOTE]
>
>Esta característica estaba disponible inicialmente como parte de un despliegue gradual solo para clientes del clúster 4 como parte de la versión 21.4. Esta característica estará disponible para todos los clústeres restantes de producción el 8 de noviembre de 2021.

En organizaciones grandes, es posible que algunos grupos necesiten configurar las preferencias de horas y de plantillas de horas de forma independiente para ajustarse a sus flujos de trabajo únicos, en lugar de heredar las preferencias configuradas por los administradores a nivel de sistema. Los administradores de Workfront ya pueden desbloquear preferencias de horas y plantillas de horas para todos los grupos del sistema y configurarlas ellos mismos.

Esta capacidad también se añadió recientemente a las preferencias del proyecto y a las preferencias de tareas y problemas.

Para obtener información sobre cómo un administrador de Workfront desbloquea una preferencia de plantilla de horas y horas, consulte la sección [Desbloquear preferencias de plantilla de horas y de horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) en el artículo [Configurar preferencias de plantilla de horas y de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obtener información sobre cómo un administrador de grupo configura las preferencias de tareas y problemas desbloqueados para un grupo, consulte [Configurar preferencias de plantilla de horas y de horas](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Seleccionar varias notificaciones que desee desbloquear o volver a bloquear para grupos

Ahora es más rápido y fácil desbloquear o volver a bloquear las notificaciones por correo electrónico para grupos. Ahora puede seleccionar varias notificaciones, comprobar las selecciones para asegurarse de que son correctas y, a continuación, hacer clic en el nuevo botón Desbloquear o Bloquear que se muestra en la barra de herramientas.

Anteriormente, tenía que desbloquear y volver a bloquear las notificaciones de una en una. Workfront tiene actualmente 95 notificaciones, por lo que este proceso tardaba un tiempo si había que hacerlo para todas ellas o muchas de ellas.

Para obtener más información, consulte [Desbloquear o bloquear la configuración de notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Para administradores de grupos: es más fácil seleccionar un grupo de reemplazo cuando se elimina un grupo

Al eliminar un grupo, dos mejoras en el cuadro Eliminar grupo facilitan la selección del grupo de reemplazo que desea para conservar los usuarios, elementos de trabajo y subgrupos del grupo eliminado:

* Puede empezar a escribir el nombre del grupo para encontrarlo rápidamente. Anteriormente, solo había una lista desplegable en la que no se podía escribir. Esto resultaba problemático para las organizaciones con muchos grupos, ya que había que desplazarse por la lista para encontrar el grupo deseado. Además, la lista desplegable tenía un límite de elementos, por lo que era posible que el grupo que quería no se mostrara.
* Puede utilizar el icono de información nueva para asegurarse de que está seleccionando el grupo de reemplazo que desea. Al pasar el puntero por encima del icono, se muestra información de objeto sobre el grupo, como la jerarquía de grupos que hay encima y los nombres de sus administradores.

Para obtener más información, consulte [Eliminar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Área más grande para crear campos calculados

Ahora es más fácil crear campos calculados complejos en un formulario personalizado. Haga clic en el nuevo botón Maximizar para abrir una ventana de edición grande para generar el cálculo. Cuando haya terminado, haga clic en Minimizar para continuar trabajando en el formulario personalizado.

## Añadir formularios personalizados a grupos

Ahora se admiten formularios personalizados para el objeto Group. Esto facilita a los grupos de su organización capturar y compartir información que satisfaga sus necesidades y flujos de trabajo específicos. Los usuarios pueden hacer lo siguiente para un grupo, igual que para otros objetos de Workfront:

* Crear un formulario personalizado
* Adjuntar un formulario personalizado
* Guardar datos de formularios personalizados
* Quitar un formulario personalizado
* Editar datos personalizados de listas y, en la nueva experiencia de Workfront, de la página Grupo

Para obtener información sobre formularios personalizados, consulte [Formularios personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Creación de aplicaciones OAuth2 para integrar aplicaciones con Workfront

Ahora puede integrar Workfront con otras aplicaciones para las que Workfront no ofrece una integración integrada. Al crear una aplicación OAuth2 para la aplicación con la que desea integrarse, puede permitir que esa aplicación acceda a Workfront, sabiendo al mismo tiempo que sus datos están protegidos por el protocolo de autenticación OAuth2 seguro y estándar del sector.

Anteriormente, solo se podía integrar con otras aplicaciones mediante integraciones integradas, Workfront Fusion o la API de Workfront.

Para obtener más información, consulte [Crear aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Mejoras en el texto de la interfaz en el área Compañías

En el área Compañías en Configuración, nuevos mensajes de confirmación y ligeros cambios en algunos términos facilitan la administración de miembros de la compañía. Por ejemplo, el nombre de sección &quot;Personas&quot; en el panel izquierdo es ahora &quot;Miembros de la compañía&quot;.

Para obtener información sobre la administración de suscripciones a compañías, consulte [Administración de suscripciones a compañías](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
