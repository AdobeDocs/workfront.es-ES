---
title: 22.3 Mejoras del administrador
description: 22.3 Mejoras del administrador
author: Luke
draft: false
feature: Product Announcements
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 22.3 Mejoras del administrador

En esta página se describen todas las mejoras realizadas por el administrador con la versión 2.3 del entorno de vista previa. Estas mejoras están disponibles durante la semana del 11 de julio de 2022. Para obtener una lista de todos los cambios disponibles con la versión 2.3, consulte [Información general sobre la versión 22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrar Adobe Workfront con JumpSeat

Ahora puede integrar JumpSeat con Workfront para crear directrices personalizadas e integradas para sus usuarios. Debe tener una licencia de Adobe Workfront Enterprise y una suscripción JumpSeat activa para habilitar la integración.

Para obtener más información, consulte [Configuración de la integración de JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Probar la configuración predeterminada trasladada a Workfront

Ahora puede editar la siguiente configuración de prueba dentro del área de configuración de Workfront:

* Probar la configuración predeterminada

* Configuración de decisión de prueba

Para obtener más información, consulte [Configuración de los ajustes de prueba predeterminados](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Usar estados desbloqueados en un proceso de aprobación

**Nota:** Eliminada de la versión de producción 2.3. Esta función se lanzará a Producción el 15 de septiembre de 2022.

Para darle más control sobre los procesos y estados de aprobación en su sistema, hemos hecho posible crear un proceso de aprobación basado en un estado del sistema desbloqueado. Además, ahora puede desbloquear cualquier estado que ya se haya utilizado en un proceso de aprobación.

Anteriormente, un estado de sistema utilizado en un proceso de aprobación tenía que estar bloqueado. Esto hizo que estuviera disponible para todos los grupos (sin la posibilidad de eliminarlo o cambiarle el nombre), de modo que los administradores de los grupos no podían racionalizar la lista de estados de sus grupos para adaptarla a sus necesidades específicas.

Para obtener más información, consulte los siguientes artículos:

* [Creación de un proceso de aprobación para elementos de trabajo](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Crear o editar un estado](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Estados de nivel de sistema bloqueados y desbloqueados](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Agregar un archivo PDF a un formulario personalizado

Seguimos ayudando a que los formularios personalizados sean más visuales e informativos con los nuevos widgets de recursos que puede agregar, como imágenes y vídeos. Ahora puede agregar un vínculo a un archivo de PDF a un formulario personalizado. Cuando el formulario está adjunto a un objeto, los usuarios que trabajan con él pueden ver e interactuar con el PDF desde el formulario.

Para obtener más información, consulte [Agregar o editar una imagen u otro widget de recursos en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## El editor de cálculo de campos de formulario personalizado muestra información de error

>[!NOTE]
>
>Esta función no está disponible temporalmente. Esta página se actualizará cuando la función esté disponible.

La edición de cálculos para campos personalizados ahora es más sencilla, ya que la información de error útil se indica directamente en el cálculo. Mientras crea un campo calculado en un formulario personalizado, los errores se resaltan en rosa. Cuando pasa el ratón por encima de la parte resaltada, aparece una información sobre herramientas para describir cuál es el problema.

Para obtener más información, consulte [Agregar datos calculados a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Personalización del encabezado del proyecto

Como administrador de Workfront o de grupos, ahora puede personalizar los campos que se muestran en el encabezado de un proyecto al utilizar una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Elimine los campos existentes del encabezado del proyecto.

* Agregue campos de Información general del proyecto nuevos y no editables. No se pueden agregar campos personalizados ni campos que se puedan editar. Los campos editables que están actualmente en el encabezado del proyecto pueden permanecer en el encabezado.

* El encabezado del objeto puede incluir hasta cinco campos.


Antes de esta versión, los campos de los encabezados de objeto no se podían personalizar.

Para obtener más información, consulte [Personalización de encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Control de la creación de un proyecto en blanco

Como administrador de sistemas o grupos, ahora puede controlar si los usuarios pueden crear proyectos en blanco sin usar una plantilla. Hemos introducido una nueva configuración en el área Preferencias del proyecto de configuración que le permite deshabilitar la creación de proyectos en blanco en las siguientes áreas:

* Desde la opción Nuevo proyecto en una lista de proyectos

* Al convertir un problema en un proyecto desde la página de problemas


El nuevo ajuste es &quot;Permitir que los usuarios creen proyectos sin usar una plantilla&quot; y está habilitado de forma predeterminada.

**Nota:** Los usuarios aún pueden convertir una tarea en un proyecto en blanco.

Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Desactivar un grupo desde la página Grupos

Recientemente, hemos agregado la capacidad de desactivar y reactivar grupos. Para que esa acción sea más rápida y fácil, la hemos agregado a la página de un grupo. Ahora, después de hacer clic en el nombre de un grupo para ir a su página, puede seleccionar el menú Más ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) junto al nombre del grupo, seleccione Desactivar o Reactivar.

Anteriormente, solo se podía desactivar o reactivar un grupo mediante la casilla de verificación Está activo en la página Detalles.

Para obtener más información, consulte [Desactivar o reactivar un grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Añadir vídeos a formularios personalizados

Ahora puede proporcionar un nuevo modo de información, interés visual y creatividad a un formulario personalizado añadiendo un vídeo. Cuando el formulario está adjunto a un objeto, los usuarios que trabajan con él pueden reproducir el vídeo en cualquier momento.

Anteriormente, solo se podían agregar campos e imágenes basados en texto a un formulario personalizado.

Para obtener más información, consulte [Agregar o editar una imagen o un widget de recursos de vídeo en un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

