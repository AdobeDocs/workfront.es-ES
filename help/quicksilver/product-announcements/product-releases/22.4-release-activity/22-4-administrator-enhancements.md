---
title: 22.4 Mejoras del administrador
description: 22.4 Mejoras del administrador
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 22.4 Mejoras del administrador

Esta página describe todas las mejoras realizadas por el administrador con la versión 22.4 en el entorno de vista previa. Estas mejoras estarán disponibles la semana del 3 de octubre de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.4, consulte [Descripción general de la versión 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Uso de estados desbloqueados en procesos de aprobación

>[!NOTE]
>
>Esta función se introdujo por primera vez en el entorno de vista previa durante el periodo de tiempo de lanzamiento de la versión 22.3. Se lanzará al entorno de producción el 15 de septiembre de 2022.

Para darle más control sobre los procesos y estados de aprobación de su sistema, hemos hecho posible crear un proceso de aprobación basado en un estado de sistema desbloqueado. Además, ahora puede desbloquear cualquier estado que ya se esté utilizando en un proceso de aprobación. Anteriormente, un estado del sistema utilizado en un proceso de aprobación tenía que estar bloqueado. Esto lo hizo disponible para todos los grupos, sin la posibilidad de eliminarlo o cambiarle el nombre, por lo que los administradores de grupos no pudieron optimizar la lista de estados de su grupo para adaptarla a sus necesidades específicas.

## El icono Modelos del menú principal ahora se controla mediante plantillas de diseño

Los administradores del sistema ahora pueden añadir o quitar el icono Modelos en el menú principal mediante la configuración de la plantilla de diseño. Esto proporciona un mayor control sobre quién puede examinar el catálogo de modelos.

El icono Modelos aparece en el menú principal cuando:

* No se ha asignado ninguna plantilla de diseño al usuario

* La plantilla de diseño del usuario tiene la opción Modelos en la lista Elementos activos

* La plantilla de diseño del usuario tiene la opción Modelos en la lista Elementos disponibles, el icono no aparece en el menú principal.

Las plantillas de diseño existentes incluyen automáticamente el icono Modelos y los administradores pueden eliminarlo de las plantillas de diseño para restringir la visibilidad del catálogo de Modelos. Las nuevas plantillas de diseño creadas después de la versión 22.4 incluirán el icono Modelos en la lista Elementos activos.

Para obtener más información, consulte [Configurar el acceso a modelos](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Ver una demostración en vídeo de esta característica](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personalizar encabezado de problema

Como administrador de Workfront o de un grupo, ahora puede personalizar los campos que se muestran en el encabezado de un problema al utilizar una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Elimine o reorganice los campos existentes del encabezado del problema.

* Agregar campos nuevos de información general de problema no editables. No puede agregar campos personalizados o campos que se puedan editar. También puede mostrar campos editables que estén actualmente en el encabezado del problema (por ejemplo, Estado o Porcentaje completado).

* El encabezado del problema puede incluir hasta cinco campos.

* Ahora puede agregar el campo &quot;Resuelto por&quot; al encabezado del problema. Cuando un objeto de resolución está asociado con el problema, el campo &quot;Resuelto por&quot; cambia a &quot;Resolviendo problema&quot;, &quot;Resolviendo tarea&quot; o &quot;Resolviendo proyecto&quot;, según el tipo de objeto asociado con el problema.

Antes de esta versión, solo se podían personalizar los encabezados de proyecto y tarea.



Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Ver una demostración en vídeo de esta característica](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personalización del encabezado de tarea

Como administrador de Workfront o de grupos, ahora puede personalizar los campos que se muestran en el encabezado de una tarea al utilizar una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Elimine o reorganice los campos existentes del encabezado de la tarea.

* Agregue campos nuevos de Información general de la tarea no editables. No puede agregar campos personalizados o campos que se puedan editar. También puede mostrar campos editables que estén actualmente en el encabezado de la tarea (por ejemplo, Estado o Porcentaje completado).

* El encabezado de la tarea puede incluir hasta cinco campos.

Antes de esta versión, solo se podían personalizar los encabezados de proyecto.

Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Ver una demostración en vídeo de esta característica.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Inclusión anticipada de funciones para las últimas funciones de los tableros

Estamos encantados de abrir nuevas funciones de tableros para la inclusión temprana de funcionalidades. Esta herramienta opcional está disponible para todas las organizaciones.

Solo un administrador de Workfront puede adherirse a las primeras funciones. Cuando el administrador se incluye en las funciones iniciales, se incluye a todos los usuarios de la organización y las funciones adicionales se habilitan en el entorno de producción de Workfront.

Para obtener más información, consulte [Inclusión anticipada de funciones para tableros de Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Ver una demostración en vídeo de esta característica.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## El editor de cálculo de campos de formulario personalizados muestra información de error

>[!NOTE]
>
>Esta función se introdujo por primera vez en el entorno de vista previa durante el periodo de tiempo de lanzamiento de la versión 22.3. Se lanza al entorno de producción con la versión 22.4.

Editar cálculos para campos personalizados ahora es más fácil con información de error útil indicada directamente en el cálculo. Mientras crea un campo calculado en un formulario personalizado, los errores se resaltan en rosa. Cuando pasa el ratón por encima de la parte resaltada, se muestra información del objeto para describir el problema.

Para obtener más información, consulte [Agregar datos calculados a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[Ver una demostración en vídeo de esta característica.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migración a la experiencia unificada de Adobe

NOTA: Esta migración se ha pospuesto hasta el primer y segundo trimestre de 2023. Se notificará a todos los clientes afectados en ese momento.

Si su organización se ha incorporado a Adobe Admin Console, la instancia de Workfront se migrará a la experiencia unificada de Adobe con la versión 22.4.

La experiencia unificada de Adobe incluye lo siguiente:

* Un solo inicio de sesión para todas las aplicaciones de Adobe a través de Adobe Experience Cloud

* Un &quot;conmutador de organización&quot; para alternar entre organizaciones y entornos de Workfront.

* Navegación con opciones para páginas de Workfront, preferencias de Adobe Experience Cloud y su perfil de Workfront

Para obtener más información, consulte [Experiencia unificada de Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Ver una demostración en vídeo de esta característica.](https://video.tv.adobe.com/v/3412388/){target=_blank}
