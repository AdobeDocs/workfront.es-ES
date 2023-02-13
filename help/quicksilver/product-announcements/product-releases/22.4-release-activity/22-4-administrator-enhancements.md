---
title: 22.4 Mejoras del administrador
description: 22.4 Mejoras del administrador
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 80fa784e15c3b4a927ee8ba2d18a80a2d84f4a91
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4 Mejoras del administrador

En esta página se describen todas las mejoras realizadas por el administrador con la versión 2.4 del entorno de vista previa. Estas mejoras estarán disponibles la semana del 3 de octubre de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 2.4, consulte [Resumen de la versión 2.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Usar estados desbloqueados en un proceso de aprobación

>[!NOTE]
>
>Esta función se introdujo por primera vez en el entorno de vista previa durante el lapso de tiempo de la versión 2.3. Se lanza a Producción el 15 de septiembre de 2022.

Para darle más control sobre los procesos y estados de aprobación en su sistema, hemos hecho posible crear un proceso de aprobación basado en un estado del sistema desbloqueado. Además, ahora puede desbloquear cualquier estado que ya se haya utilizado en un proceso de aprobación. Anteriormente, un estado de sistema utilizado en un proceso de aprobación tenía que estar bloqueado. Esto hizo que estuviera disponible para todos los grupos (sin la posibilidad de eliminarlo o cambiarle el nombre), de modo que los administradores de los grupos no podían racionalizar la lista de estados de sus grupos para adaptarla a sus necesidades específicas.

## El icono de modelos del menú principal ahora se controla mediante plantillas de diseño

Los administradores del sistema ahora pueden agregar o quitar el icono Blueprints del menú principal mediante la configuración de la plantilla de diseño. Esto proporciona bueno control sobre quién puede examinar el catálogo de modelos.

El icono Modelos aparece en el menú principal cuando:

* El usuario no tiene ninguna plantilla de diseño asignada

* La plantilla de diseño del usuario tiene la opción Planos de la lista Elementos activos

* La plantilla de diseño del usuario tiene la opción Modelos de la lista Elementos disponibles , el icono no aparece en el menú principal.

Las plantillas de diseño existentes incluyen automáticamente el icono Blueprints y los administradores pueden eliminar el icono de las plantillas de diseño para restringir la visibilidad del catálogo de modelos. Las nuevas plantillas de diseño creadas después de la versión 2.4 incluirán el icono Modelos en la lista Elementos activos .

Para obtener más información, consulte [Configuración del acceso a modelos](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personalización del encabezado del problema

Como administrador de Workfront o de grupos, ahora puede personalizar los campos que aparecen en el encabezado de un problema al utilizar una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Elimine o reorganice los campos existentes del encabezado del problema.

* Agregue nuevos campos de Información general de problemas no editables. No se pueden agregar campos personalizados ni campos que se puedan editar. También puede mostrar campos editables que estén actualmente en el encabezado del problema (por ejemplo, Estado o Porcentaje completado).

* El encabezado del problema puede incluir hasta cinco campos.

* Ahora puede agregar el campo &quot;Resuelto por&quot; al encabezado del problema. Cuando un objeto de resolución está asociado al problema, el campo &quot;Resuelto por&quot; cambia a &quot;Solución de problema&quot;, &quot;Tarea resuelta&quot; o &quot;Proyecto resuelto&quot;, según el tipo de objeto asociado al problema.

Antes de esta versión, solo se podían personalizar los encabezados de proyecto y tarea.



Para obtener más información, consulte [Personalización de encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Ver una demostración en vídeo de esta función](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personalización del encabezado de la tarea

Como administrador de Workfront o de grupos, ahora puede personalizar los campos que se muestran en el encabezado de una tarea al utilizar una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Elimine o reorganice los campos existentes del encabezado de la tarea.

* Agregue nuevos campos Información general de tareas no editables. No se pueden agregar campos personalizados ni campos que se puedan editar. También puede mostrar campos editables que se encuentren actualmente en el encabezado de la tarea (por ejemplo, Estado o Porcentaje completado).

* El encabezado de la tarea puede incluir hasta cinco campos.

Antes de esta versión, solo se podían personalizar los encabezados de proyecto.

Para obtener más información, consulte [Personalización de encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Vea una demostración en vídeo de esta función.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Inclusión anticipada para las últimas funciones de los tableros

Estamos encantados de abrir nuevas funciones de tableros para la inclusión anticipada de funciones. Esta herramienta opcional está disponible para todas las organizaciones.

Solo los administradores de Workfront pueden incluirse en las funciones anteriores. Cuando el administrador elige las funciones iniciales, todos los usuarios de la organización se incluyen y las funciones adicionales se habilitan en el entorno de producción de Workfront.

Para obtener más información, consulte [Inclusión anticipada de funciones para placas Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Vea una demostración en vídeo de esta función.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## El editor de cálculo de campos de formulario personalizado muestra información de error

>[!NOTE]
>
>Esta función se introdujo por primera vez en el entorno de vista previa durante el lapso de tiempo de la versión 2.3. Se lanza a Producción con la versión 22.4.

La edición de cálculos para campos personalizados ahora es más sencilla, ya que la información de error útil se indica directamente en el cálculo. Mientras crea un campo calculado en un formulario personalizado, los errores se resaltan en rosa. Cuando pasa el ratón por encima de la parte resaltada, aparece una información sobre herramientas para describir cuál es el problema.

Para obtener más información, consulte [Agregar datos calculados a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[Vea una demostración en vídeo de esta función.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migración a la experiencia unificada de Adobe

NOTA: Esta migración se ha pospuesto hasta el primer trimestre de 2023. A cualquier cliente afectado se le notificará en ese momento.

Si su organización se ha incorporado a Adobe Admin Console, la instancia de Workfront se migrará a la Experiencia unificada de Adobe con la versión 22.4.

La experiencia unificada de Adobe incluye:

* Un inicio de sesión único para todas las aplicaciones de Adobe a través de Adobe Experience Cloud

* Un &quot;conmutador de organización&quot; para moverse entre las organizaciones y los entornos de Workfront

* Navegación con opciones para páginas de Workfront, preferencias de Adobe Experience Cloud y su perfil de Workfront

Para obtener más información, consulte [Experiencia unificada de Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Vea una demostración en vídeo de esta función.](https://video.tv.adobe.com/v/3412388/){target=_blank}
