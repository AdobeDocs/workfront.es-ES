---
title: Mejoras del administrador del cuarto trimestre de 2026
description: Mejoras del administrador del cuarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: c3dc1aa9e48d45d2546561c2ac9412b008258e2d
workflow-type: tm+mt
source-wordcount: '1267'
ht-degree: 1%

---

# Mejoras del administrador del cuarto trimestre de 2026

Esta página describe las mejoras realizadas por el administrador con la versión del cuarto trimestre de 2026 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del cuarto trimestre de 2026, consulte [Información general de la versión del cuarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

<!--

## Interface improvements to the Actions list

>[!NOTE]
>
>Preview: August 20, 2026
>Production fast release: September 17, 2026
>Production for everyone: October 15, 2026

The Actions list in the Update Feeds section of the Setup area has an updated look and feel.

The following enhancements are included:

* We removed the Save and Cancel buttons.
* The Track column now appears in the last position.
* We removed the confirmation message that previously displayed when you saved changes in this area.

For information, see [Configure system updates](/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

-->

## Establezca un nivel de acceso predeterminado para los usuarios aprovisionados en Adobe Admin Console

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede establecer un nivel de acceso predeterminado para los usuarios que se aprovisionan en Workfront a través de Adobe Admin Console. Un administrador de Workfront puede configurar este valor predeterminado en Preferencias del sistema.

Anteriormente, Workfront asignaba al usuario un nivel de acceso de colaborador o solicitante.

Para obtener más información, consulte [Configurar las preferencias del sistema](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Semanas personalizadas además de trimestres personalizados para clientes de Workfront Planning

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Si su organización ha adquirido un paquete de Planning, además de un paquete de flujo de trabajo, ahora puede configurar semanas personalizadas del mismo modo que lo hace con un administrador de Workfront.

Las semanas personalizadas no son visibles en Workfront. Solo están visibles en la vista de cronología de Workfront Planning.

Para obtener más información, consulte [Habilitar trimestres personalizados](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md).

## Reordenar aplicaciones personalizadas en el menú principal

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Al trabajar en una plantilla de diseño, ahora puede cambiar la posición de las aplicaciones personalizadas para que estén en cualquier orden con las opciones de menú predeterminadas de Workfront. Esto le permite colocar cada aplicación en el lugar más relevante.

Anteriormente, las aplicaciones personalizadas siempre eran los últimos elementos en las opciones del menú principal de la plantilla de diseño y no se podían cambiar de posición.

Para obtener más información sobre cómo agregar aplicaciones personalizadas al menú principal, vea [Personalizar el menú principal con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

## Compatibilidad con archivos grandes para integraciones de documentos personalizadas

>[!NOTE]
>
>Vista previa: 3 de septiembre de 2026
>Versión rápida de producción: 17 de septiembre de 2026
>Producción para todos: 15 de octubre de 2026

Las integraciones de documentos personalizadas ahora admiten cargas fraccionadas para archivos grandes. Cuando se habilita, los archivos de más de 25 MB se dividen en fragmentos más pequeños y se cargan en paralelo, lo que hace que las cargas de archivos grandes sean más rápidas y fiables. Los administradores pueden activar esta opción y establecer el tamaño máximo de fragmento (hasta 100 MB) por integración.

Para obtener más información, consulte [Configurar integraciones de documentos](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md).

## Los administradores de grupo pueden administrar perfiles empresariales

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Los administradores de grupos ahora pueden crear, editar y eliminar perfiles empresariales para los grupos que administran, sin necesidad de acceso de administrador del sistema. Esto proporciona a las organizaciones más flexibilidad para delegar la administración del perfil empresarial en el nivel de grupo.

Para obtener más información, vea [Ver y administrar perfiles de negocio](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-business-profiles.md).

## Compatibilidad con plantillas de diseño para vistas en listas mejoradas

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Ahora se admiten vistas para listas mejoradas en el sistema a través de una plantilla de diseño. Puede ocultar las vistas del sistema existentes, asignar una vista específica como vista predeterminada y agregar una vista personalizada a la lista de vistas del sistema.

Algunos ejemplos de listas mejoradas en la plantilla de diseño son **Todas las solicitudes** y **Asignaciones avanzadas**. Una lista mejorada tiene la etiqueta &quot;Nueva experiencia&quot; junto a las vistas.

Para obtener más información, consulte [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Edición masiva de campos de búsqueda externos

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Los cuadros de diálogo de edición masiva ahora permiten editar campos de búsqueda externos. Anteriormente esto no era posible.

En situaciones en las que un campo de búsqueda depende de otro campo de búsqueda, el campo con la dependencia no se puede editar de forma masiva a menos que el primer campo sea el mismo para todos los objetos que se están editando.

Por ejemplo, una lista de países depende de la selección realizada para una región. Si la región de un proyecto es Asia y la de otro es Europa y edita ambos proyectos en lote, el campo País no estará disponible porque las regiones no coinciden. Si edita la región para que sea la misma en ambos proyectos, también puede seleccionar un país para utilizarlo en ambos.

Para obtener información sobre los campos de búsqueda externos, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-external-lookup-fields).

## Lógica avanzada admitida en la vista previa del diseñador de formularios personalizados

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

El modo de vista previa del diseñador de formularios personalizado ahora admite opciones de lógica avanzadas, incluida la lógica de visualización avanzada, la lógica de valor predeterminada, la lógica de validación, la lógica de formato y la lógica de editabilidad. Puede probar las fórmulas lógicas en la vista previa del formulario y ajustarlas según sea necesario en el generador de lógicas. También puede seleccionar un objeto de prueba (proyecto, tarea, problema, etc.) para obtener una vista previa del formulario con datos contextuales reales.

Anteriormente, solo se admitían las opciones básicas de visualización y lógica de omisión en el modo de vista previa.

Tenga en cuenta que estos tipos lógicos solo están disponibles para organizaciones en los paquetes Workflow Prime o Ultimate: visualización avanzada, valor predeterminado, formato condicional y editabilidad.

Para obtener más información, consulte [Agregar reglas lógicas a formularios y campos personalizados](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) y [Organizar y previsualizar un formulario](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Seguimiento de cambios para revisión y aprobación unificadas

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

La página Historial de cambios de Workfront ahora captura la actividad en los flujos de trabajo unificados de revisión y aprobación, lo que proporciona a los administradores un registro de control completo para los eventos de ciclo vital de revisión y documento.

Ahora se realiza un seguimiento de las acciones de aprobación, fase y participante. Estas acciones pueden incluir:

* Toma de una decisión de aprobación en el visor Frame.io
* Creación o eliminación de una aprobación
* Actualizar un documento, como cambiarle el nombre, moverlo o eliminarlo

Cada entrada incluye los campos rastreados estándar: fecha y hora, operación, nombre de usuario (o &quot;generado por el sistema&quot;) y nombre de objeto. Se capturan las actividades de MCP, incluido qué LLM (como Claude) realizó la actualización. No se incluyen los comentarios del visor de Frame.io.

Para obtener más información, vea [Ver y administrar el historial de cambios](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Defina una aplicación personalizada como una página de aterrizaje en la plantilla de diseño

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Ahora puede establecer una aplicación personalizada como página de aterrizaje en una plantilla de diseño. Las aplicaciones personalizadas que ya se han añadido al menú principal están disponibles para su uso como página de aterrizaje.

Las aplicaciones personalizadas deben crearse por separado antes de que estén disponibles como opciones del menú principal o de la página de aterrizaje.

Para obtener más información, consulte [Personalizar la página de aterrizaje con una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md) y [Crear aplicaciones personalizadas para Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

## Configurar campos rastreados en el historial de cambios

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

Puede agregar campos que desee rastrear para un tipo concreto de objeto a través de Workfront. Cuando los usuarios cambian información en ese campo, el sistema registra la información sobre el cambio como una entrada en el historial de cambios.

Anteriormente, la pantalla Configuración para definir los campos rastreados era de solo vista.

Para obtener más información, consulte [Configurar campos para realizar un seguimiento en el historial de cambios](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

## Acceso administrativo al historial de cambios agregado a los niveles de acceso

>[!NOTE]
>
>Vista previa: 30 de julio de 2026
>Versión rápida de producción: 13 de agosto de 2026
>Producción para todos: 15 de octubre de 2026

En el nivel de acceso Estándar, ahora puede definir si los usuarios con ese nivel deben tener acceso a la lista Historial de cambios. La opción **Cambiar historial** está disponible en la sección **Permitir acceso administrativo para** en el nivel de acceso.

Para obtener más información, consulte [Conceder acceso administrativo a los usuarios a ciertas áreas](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md) y [Ver y administrar el historial de cambios](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).


