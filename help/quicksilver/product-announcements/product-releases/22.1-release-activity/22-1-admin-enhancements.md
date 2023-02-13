---
title: 22.1 Mejoras del administrador
description: 22.1 Mejoras del administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# 22.1 Mejoras del administrador

En esta página se describen todas las mejoras realizadas por el administrador con la versión 2.1 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 17 de enero de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 2.1, consulte [Resumen de la versión 2.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Descargas de documentos registradas en el área Actualizaciones

Para ayudar a los usuarios a rastrear las descargas de documentos que almacenan en Workfront, el sistema ahora registra una entrada en el área Actualizaciones de un documento cuando alguien lo descarga.

>[!NOTE]
>
>Se recomienda probar esta función en Vista previa en un documento recién cargado.

Para obtener información sobre cómo Workfront registra las actualizaciones automáticas de los objetos, consulte [Actualizaciones rastreadas por el sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Concesión de acceso a equipos mediante niveles de acceso

Una nueva sección del área Niveles de acceso le proporciona controles más granulares para administrar el acceso de los usuarios a los equipos. Ahora puede determinar quién puede crear, editar y ver equipos.

Esto no cambia el acceso existente de los usuarios a los equipos.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## La asignación de grupos ahora está disponible en modelos

Algunos modelos ahora incluyen grupos que puede personalizar antes de instalar el modelo. Puede asignar un grupo del modelo a un grupo existente en la instancia de Workfront o crear un grupo nuevo si es necesario.

Para obtener más información, consulte [Configuración de un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Actualizaciones de estilo en el área Forms personalizado

El área de Forms personalizado tiene un nuevo aspecto que lo actualiza con muchas otras áreas de la nueva experiencia de Workfront.

Para obtener información sobre cómo crear un formulario personalizado, consulte [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Muchas mejoras para crear campos personalizados calculados

La creación de campos personalizados calculados ahora es mucho más fácil con estas adiciones en el nuevo Editor de cálculos:

* Puede pasar el ratón sobre cualquier expresión del cálculo para mostrar información sobre ella, incluida una descripción, un ejemplo de cómo se puede utilizar y un vínculo a más información en un artículo de ayuda.
* Cada expresión que agregue tendrá un código de colores, según su tipo. Esto facilita la identificación de las expresiones y el reconocimiento inmediato de su tipo.
* Los números de línea ayudan a identificar y hacer referencia a funciones en un cálculo largo.
* Cuando empieza a escribir una expresión o un nombre de campo, aparece una lista de elementos disponibles para que pueda elegir el que desee. Y, cuando se escribe un paréntesis de apertura, el paréntesis de cierre se agrega automáticamente.
* Puede obtener una vista previa del resultado del cálculo utilizando un objeto existente sin salir del editor de cálculo.

Además, en el texto personalizable &quot;Instrucciones&quot; al pasar el ratón por encima de un campo personalizado calculado, puede mostrar u ocultar la fórmula del campo. Esto resulta útil si cree que los usuarios que rellenen el formulario personalizado no necesitan esa información.

Para obtener más información sobre la creación de un campo personalizado calculado, consulte [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Ver información del registro de auditoría sobre estados y empresas

Ahora puede solucionar con mayor facilidad los incidentes que impliquen estados y empresas consultando la información sobre ellos en el área Registros de auditoría de Configuración.

Por ejemplo:

* Puede averiguar quién cambió el nombre, bloqueó u ocultó un estado y cuándo lo hicieron.
* Puede averiguar quién eliminó a algunos miembros o funciones de trabajo de una empresa y cuándo lo hicieron.

Para obtener información sobre la visualización de la información del registro de auditoría, consulte [Ver y exportar registros de auditoría](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Planes de mapeo de la empresa y otras mejoras

Ya están disponibles las siguientes mejoras de modelos:

* Algunos modelos ahora incluyen empresas, que puede personalizar antes de instalar el modelo. Puede asignar una empresa del modelo a una empresa existente en la instancia de Workfront o crear una empresa nueva si es necesario.
* Ya está disponible un nuevo tipo de modelo, Estructura organizativa. Algunos modelos incluyen elementos de varios tipos (por ejemplo, plantilla de proyecto y estructura organizativa). Puede filtrar por tipo de modelo en la página de catálogo.
* Las secciones &quot;Preferencias de instalación&quot; y &quot;Propiedad de plantilla&quot; de la página de configuración se han combinado en &quot;Preferencias de plantilla&quot; para simplificar.

Para obtener más información, consulte [Configuración de un modelo](../../../administration-and-setup/blueprints/configure-template-package.md).

## Administre las membresías de la empresa con mayor facilidad

En el área Compañías, una barra de herramientas actualizada facilita la adición de usuarios de Workfront existentes a una empresa y la eliminación de miembros de la empresa.

Anteriormente, estas acciones solo estaban disponibles en el cuadro Editar empresa .

La barra de herramientas actualizada también contiene todas las acciones disponibles en la barra de herramientas anterior, como editar la información de perfil de usuario de los miembros y desactivarlos en el sistema.

Para obtener más información, consulte [Administración de suscripciones a la empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Seleccionar expresiones y campos en la nueva ventana de campo calculado

Seguimos facilitando la creación de un campo calculado en un formulario personalizado. Ahora, al hacer clic en Maximizar para abrir el nuevo Editor de cálculo, puede buscar y seleccionar las expresiones y los campos que necesita.

Para obtener más información, consulte [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Los grupos pueden configurar sus propias preferencias de horario y hora

>[!NOTE]
>
>Esta función estaba disponible inicialmente como parte de un lanzamiento por fases solo para clientes del clúster 4 como parte de la versión 21.4. Esta función estará disponible para todos los clústeres restantes de Producción el 8 de noviembre de 2021.

En una organización grande, es posible que algunos grupos necesiten configurar las preferencias de horas y horas de forma independiente para que se ajusten a sus flujos de trabajo únicos, en lugar de heredar las preferencias configuradas por un administrador a nivel del sistema. Ahora los administradores de Workfront pueden desbloquear un parte de horas y una preferencia de hora para todos los grupos del sistema para que puedan configurarlo por su cuenta.

Esta capacidad también se agregó recientemente para las preferencias de proyecto y para las preferencias de tarea y problema.

Para obtener información sobre cómo un administrador de Workfront desbloquea un parte de horas y una preferencia de hora, consulte la sección [Desbloquear preferencias de horas y horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) en el artículo [Configuración de las preferencias de horas y horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obtener información sobre cómo un administrador de grupo configura una tarea desbloqueada y las preferencias de problema para un grupo, consulte [Configuración de las preferencias de horas y horas de un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Seleccionar varias notificaciones que desee desbloquear o volver a bloquear para grupos

Ahora es más rápido y fácil desbloquear o volver a bloquear las notificaciones de correo electrónico para grupos. Ahora puede seleccionar varias notificaciones, comprobar las selecciones para asegurarse de que son correctas y luego hacer clic en el nuevo botón Desbloquear o Bloquear que aparece en la barra de herramientas.

Anteriormente, había que desbloquear y volver a bloquear las notificaciones de una en una. Actualmente, Workfront tiene 95 notificaciones, por lo que tardó un rato en hacerlo para todas o muchas de ellas.

Para obtener más información, consulte [Desbloquear o bloquear la configuración de las notificaciones de eventos para todos los grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Para administradores de grupos: Es más fácil seleccionar un grupo de reemplazo al eliminar un grupo

Al eliminar un grupo, dos mejoras en el cuadro Eliminar grupo facilitan la selección del grupo de reemplazo que desea conservar los usuarios, elementos de trabajo y subgrupos del grupo eliminado:

* Puede empezar a escribir el nombre del grupo para encontrarlo rápidamente. Anteriormente, solo había una lista desplegable que no podía escribir. Esto resultaba problemático para las organizaciones con muchos grupos porque había que desplazarse por la lista para encontrar el grupo que quería. Además, la lista desplegable tenía un límite de elementos, por lo que era posible que el grupo que quería no se mostrara.
* Puede utilizar el icono de información nueva para asegurarse de que está seleccionando el grupo de reemplazo que desea. Al pasar el ratón por encima del icono, se muestra una información sobre herramientas que enumera información sobre el grupo, como la jerarquía de grupos por encima de él y los nombres de sus administradores.

Para obtener más información, consulte [Eliminar un grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Área más grande para crear campos calculados

Ahora es más fácil crear campos calculados complejos en un formulario personalizado. Haga clic en el nuevo botón Maximizar para abrir una ventana de edición grande para crear el cálculo. Cuando haya terminado, haga clic en Minimizar para seguir trabajando en el formulario personalizado.

Para obtener más información, consulte [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Agregar formularios personalizados a grupos

Los formularios personalizados ahora se admiten para el objeto Group . Esto facilita a los grupos de su organización la captación y el uso compartido de información que satisfaga sus necesidades y flujos de trabajo específicos. Los usuarios pueden hacer lo siguiente para un grupo, igual que con otros objetos de Workfront:

* Crear un formulario personalizado
* Adjuntar un formulario personalizado
* Guardar datos de formulario personalizados
* Eliminación de un formulario personalizado
* Editar datos personalizados desde listas y, en la nueva experiencia de Workfront, desde la página Grupo

Para obtener información sobre los formularios personalizados, consulte [Formularios personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Cree aplicaciones OAuth2 para integrar aplicaciones con Workfront

Ahora puede integrar Workfront con otras aplicaciones para las que Workfront no ofrece una integración integrada. Al crear una aplicación OAuth2 para la aplicación con la que desea integrarse, puede permitir que dicha aplicación acceda a Workfront, al tiempo que sabe que sus datos están protegidos por el protocolo de autenticación OAuth2 seguro y estándar del sector.

Anteriormente, solo se podía integrar con otras aplicaciones mediante integraciones integradas, Workfront Fusion o la API de Workfront.

Para obtener más información, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Mejoras en la interfaz de texto en el área Compañías

En el área Empresas de Configuración, los nuevos mensajes de confirmación y los ligeros cambios de redacción facilitan la administración de las suscripciones a la empresa. Por ejemplo, el nombre de sección &quot;Personas&quot; en el panel izquierdo es ahora &quot;Miembros de la empresa&quot;.

Para obtener información sobre la administración de las suscripciones a la empresa, consulte [Administración de suscripciones a la empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
