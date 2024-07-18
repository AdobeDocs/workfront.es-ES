---
title: 22.3 Mejoras del administrador
description: 22.3 Mejoras del administrador
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 0%

---

# 22.3 Mejoras del administrador

Esta página describe todas las mejoras realizadas por el administrador con la versión 22.3 en el entorno de vista previa. Estas mejoras estuvieron disponibles la semana del 11 de julio de 2022. Para obtener una lista de todos los cambios disponibles con la versión 22.3, consulte [Información general sobre la versión 22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integración de Adobe Workfront con JumpSeat

Ahora puede integrar JumpSeat con Workfront para crear orientación personalizada en el producto para sus usuarios. Debe tener una licencia empresarial de Adobe Workfront y una suscripción JumpSeat activa para habilitar la integración.

Para obtener más información, consulte [Configuración de la integración de JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## La configuración predeterminada de revisión se movió a Workfront

Ahora puede editar la siguiente configuración de revisión dentro del área de configuración de Workfront:

* Configuración predeterminada de revisión

* Configuración de decisión de revisión

Para obtener más información, consulte [Configurar opciones predeterminadas de revisión](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Uso de estados desbloqueados en procesos de aprobación

**Nota:** se eliminó de la versión de producción 22.3. Está previsto que esta función se publique en Production el 15 de septiembre de 2022.

Para darle más control sobre los procesos y estados de aprobación de su sistema, hemos hecho posible crear un proceso de aprobación basado en un estado de sistema desbloqueado. Además, ahora puede desbloquear cualquier estado que ya se esté utilizando en un proceso de aprobación.

Anteriormente, un estado del sistema utilizado en un proceso de aprobación tenía que estar bloqueado. Esto lo hizo disponible para todos los grupos, sin la posibilidad de eliminarlo o cambiarle el nombre, por lo que los administradores de grupos no pudieron optimizar la lista de estados de su grupo para adaptarla a sus necesidades específicas.

Para obtener más información, consulte los siguientes artículos:

* [Crear un proceso de aprobación para elementos de trabajo](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Creación o edición de un estado](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Estados bloqueados y desbloqueados en el nivel del sistema](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Agregar un archivo de PDF a un formulario personalizado

Seguimos ayudando a que los formularios personalizados sean más visuales e informativos con los nuevos widgets de recursos que puede agregar, como imágenes y vídeos. Ahora puede agregar un vínculo a un archivo de PDF a un formulario personalizado. Cuando el formulario está adjunto a un objeto, los usuarios que trabajan con el objeto pueden ver e interactuar con el PDF desde el formulario.

## El editor de cálculo de campos de formulario personalizados muestra información de error

>[!NOTE]
>
>Esta función no está disponible temporalmente. Esta página se actualizará cuando la función esté disponible.

Editar cálculos para campos personalizados ahora es más fácil con información de error útil indicada directamente en el cálculo. Mientras crea un campo calculado en un formulario personalizado, los errores se resaltan en rosa. Cuando pasa el ratón por encima de la parte resaltada, se muestra información del objeto para describir el problema.

## Personalización del encabezado del proyecto

Como administrador de Workfront o de grupos, ahora puede personalizar los campos que se muestran en el encabezado de un proyecto al utilizar una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Elimine los campos existentes del encabezado del proyecto.

* Agregue campos nuevos de Información general del proyecto no editables. No puede agregar campos personalizados o campos que se puedan editar. Los campos editables que están actualmente en el encabezado del proyecto pueden permanecer en el encabezado.

* El encabezado del objeto puede incluir hasta cinco campos.


Antes de esta versión, los campos de los encabezados de objeto no se podían personalizar.

Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Controlar la creación de un proyecto en blanco

Como administrador de sistemas o de grupos, ahora puede controlar si los usuarios pueden crear proyectos en blanco sin utilizar una plantilla. Hemos introducido una nueva configuración en el área de Preferencias de proyecto de Configuración que le permite desactivar la creación de proyectos en blanco en las siguientes áreas:

* Desde la opción Nuevo proyecto en una lista de proyectos

* Cuando se convierte un problema en un proyecto desde la página del problema


La nueva configuración es &quot;Permitir a los usuarios crear proyectos sin utilizar una plantilla&quot; y está habilitada de forma predeterminada.

**Nota:** Los usuarios aún pueden convertir una tarea en un proyecto en blanco.

Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Desactivar un grupo de la página Grupos

Recientemente, hemos agregado la capacidad de desactivar y reactivar grupos. Para que esa acción sea más rápida y sencilla, la hemos agregado a la página de un grupo. Ahora, después de hacer clic en el nombre de un grupo para ir a su página, puede seleccionar el menú Más ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) junto al nombre del grupo y, a continuación, seleccionar Desactivar o Reactivar.

Anteriormente, sólo se podía desactivar o reactivar un grupo mediante la casilla de verificación Está activo en la página Detalles.

Para obtener más información, vea [Desactivar o reactivar un grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Agregar vídeos a formularios personalizados

Ahora puede proporcionar un nuevo modo de información, interés visual y creatividad a un formulario personalizado agregando un vídeo. Cuando el formulario está adjunto a un objeto, los usuarios que trabajen con el objeto pueden reproducir el vídeo en cualquier momento.

Anteriormente, solo se podían agregar campos basados en texto e imágenes a un formulario personalizado.

