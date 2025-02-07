---
title: 22.3 Mejoras del administrador
description: 22.3 Mejoras del administrador
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 95%

---

# 22.3 Mejoras del administrador

Esta página describe todas las mejoras realizadas por el administrador con la versión 22.3 en el entorno de vista previa. Estas mejoras estuvieron disponibles la semana del 11 de julio de 2022. Para obtener una lista de todos los cambios disponibles con la versión 22.3, consulte [Información general sobre la versión 22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integración de Adobe Workfront con JumpSeat

Ahora puede integrar JumpSeat en Workfront para crear una guía personalizada en el producto para sus usuarios. Debe tener una licencia empresarial de Adobe Workfront y una suscripción JumpSeat activa para habilitar la integración.

Para obtener más información, consulte [Configurar integración de JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## La configuración predeterminada de revisión se ha movido a Workfront

Ahora puede editar la siguiente configuración de pruebas dentro del área de configuración de Workfront:

* Configuración de revisión predeterminada

* Configuración de revisión de decisión

Para obtener más información, consulte [Configuración de valores predeterminados de prueba](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Usar estados desbloqueados en un proceso de aprobación

**Nota:** Se ha eliminado de la versión de producción 22.3. Está previsto que esta función se publique en Producción el 15 de septiembre de 2022.

Para darle más control sobre los procesos y estados de aprobación de su sistema, hemos creado un proceso de aprobación basado en un estado del sistema desbloqueado. Además, ahora puede desbloquear cualquier estado que ya se haya utilizado en un proceso de aprobación. 

Anteriormente, un estado del sistema utilizado en un proceso de aprobación tenía que estar bloqueado. De este modo, estaba disponible para todos los grupos, sin la posibilidad de eliminarlo o cambiarle el nombre, por lo que los administradores de grupos no podían optimizar la lista de estados de su grupo para adaptarla a sus necesidades específicas.

Para obtener más información, consulte los siguientes artículos:

* [Crear un proceso de aprobación para los elementos de trabajo](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Crear o editar un estado](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Estados de nivel del sistema bloqueados y desbloqueados](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Añadir un archivo PDF a un formulario personalizado

Seguimos trabajando para que los formularios personalizados sean más visuales e informativos, con nuevos widgets de recursos para añadir, como imágenes y vídeos. Ahora puede añadir un vínculo a un archivo PDF hacia un formulario personalizado. Cuando el formulario está adjunto a un objeto, los usuarios que trabajan con el objeto pueden ver e interactuar con el PDF desde el formulario.

## El editor de cálculo de campos de formulario personalizados muestra información de error

>[!NOTE]
>
>Esta función no está disponible temporalmente. Esta página se actualizará cuando la función esté disponible.

Editar cálculos para campos personalizados ahora es más fácil con información de error útil indicada directamente en el cálculo. Mientras crea un campo calculado en un formulario personalizado, los errores se resaltan en rosa. Cuando pasa el puntero encima de la parte resaltada, se muestra información del objeto para describir el problema.

## Personalización del encabezado del proyecto

Como administrador de Workfront o de grupos, ahora puede personalizar los campos que se muestran en el encabezado de un proyecto al utilizar una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Se eliminan los campos existentes del encabezado del proyecto.

* Añada campos nuevos de Información general del proyecto no editables. No puede añadir campos personalizados o campos que se puedan editar. Los campos editables que están actualmente en el encabezado del proyecto pueden seguir en el encabezado.

* El encabezado del objeto puede incluir hasta cinco campos.


Antes de esta versión, los campos en los encabezados de los objetos no se podían personalizar.

Para obtener más información, consulte [Personalización de los encabezados de los objetos mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Controlar la creación de un proyecto en blanco

Como administrador de sistemas o de grupos, ahora puede controlar si los usuarios pueden crear proyectos en blanco sin utilizar una plantilla. Hemos introducido una nueva configuración en el área Preferencias de proyecto, en Configuración, que le permite desactivar la creación de proyectos en blanco en las siguientes áreas:

* Desde la opción Nuevo proyecto en una lista de proyectos

* Cuando se convierte un problema en un proyecto desde la página del problema


La nueva configuración es &quot;Permitir a los usuarios crear proyectos sin utilizar una plantilla&quot; y está habilitada de forma predeterminada.

**Nota:** Los usuarios aún pueden convertir una tarea en un proyecto en blanco.

Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Desactivar un grupo de la página Grupos

Recientemente, hemos añadido la posibilidad de desactivar y reactivar grupos. Para que esa acción sea más rápida y sencilla, la hemos añadido a la página de un grupo. Ahora, después de hacer clic en el nombre de un grupo para ir a su página, puede seleccionar el icono del menú Más ![Menú principal](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) junto al nombre del grupo y, a continuación, seleccionar Desactivar o Reactivar.

Anteriormente, sólo se podía desactivar o reactivar un grupo mediante Está la casilla de verificación activa en la página Detalles.

Para obtener más información, consulte [Desactivar o reactivar un grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Añadir vídeos a formularios personalizados

Ahora puede proporcionar un nuevo modo de información, interés visual y creatividad a un formulario personalizado añadiendo un vídeo. Cuando el formulario está adjunto a un objeto, los usuarios que trabajen con el objeto pueden reproducir el vídeo en cualquier momento.

Anteriormente, solo se podían añadir campos basados en texto e imágenes a un formulario personalizado.

