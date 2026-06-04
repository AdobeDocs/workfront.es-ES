---
title: Mejoras del administrador en la versión 22.4
description: Mejoras del administrador en la versión 22.4
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
TQID: https://experienceleague.adobe.com/d5r4VDW3ZD3sNx5s9Kj9V8PKt39fZNFtwfiAj6dzdzk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 881
ht-degree: 60%

---

# Mejoras del administrador en la versión 22.4

En esta página se describen todas las mejoras realizadas por el administrador con la versión 22.4 en el entorno de vista previa. Estas mejoras estarán disponibles la semana del 3 de octubre de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.4, consulte [Información general de la versión 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Usar estados desbloqueados en un proceso de aprobación

>[!NOTE]
>
>Esta función se introdujo por primera vez en el entorno de vista previa durante el periodo de tiempo de lanzamiento de la versión 22.3. Se lanzará al entorno de producción el 15 de septiembre de 2022.

Para darle más control sobre los procesos y estados de aprobación de su sistema, hemos creado un proceso de aprobación basado en un estado del sistema desbloqueado. Además, ahora puede desbloquear cualquier estado que ya se haya utilizado en un proceso de aprobación. Anteriormente, un estado del sistema utilizado en un proceso de aprobación tenía que estar bloqueado. De este modo, estaba disponible para todos los grupos, sin la posibilidad de eliminarlo o cambiarle el nombre, por lo que los administradores de grupos no podían optimizar la lista de estados de su grupo para adaptarla a sus necesidades específicas.

## El icono Modelos del menú principal ahora se controla mediante plantillas de diseño

Los administradores del sistema ahora pueden añadir o quitar el icono de modelos en el menú principal mediante la configuración de la plantilla de diseño. Esto ofrece un mayor control sobre quién puede examinar el catálogo de modelos.

El icono Modelos aparece en el menú principal cuando:

* No se ha asignado ninguna plantilla de diseño al usuario

* La plantilla de diseño del usuario tiene la opción Modelos en la lista Elementos activos

* La plantilla de diseño del usuario tiene la opción Modelos en la lista Elementos disponibles, el icono no aparece en el menú principal.

Las plantillas de diseño existentes incluyen automáticamente el icono Modelos y los administradores pueden eliminarlo de las plantillas de diseño para restringir la visibilidad del catálogo de Modelos. Las nuevas plantillas de diseño creadas después de la versión 22.4 incluirán el icono Modelos en la lista Elementos activos.

Para obtener más información, consulte [Configurar el acceso a modelos](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Vea un vídeo de demostración de esta función](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personalización del encabezado de un problema

Como administrador de Workfront o de grupos, ahora puede personalizar los campos que se muestran en el encabezado de un problema cuando utilice una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Quite o reorganice los campos existentes del encabezado del problema.

* Añada campos nuevos de información general del problema no editables. No puede añadir campos personalizados o campos que se puedan editar. También puede mostrar campos editables que estén actualmente en el encabezado del problema (por ejemplo, Estado o Porcentaje completado).

* El encabezado del problema puede incluir hasta cinco campos.

* Ahora puede agregar el campo &quot;Resuelto por&quot; al encabezado del problema. Cuando un objeto de resolución está asociado con el problema, el campo &quot;Resuelto por&quot; cambia a &quot;Resolviendo problema&quot;, &quot;Resolviendo tarea&quot; o &quot;Resolviendo proyecto&quot;, según el tipo de objeto asociado con el problema.

Antes de esta versión, solo se podían personalizar los encabezados de proyectos y tareas.



Para obtener más información, consulte [Personalización de los encabezados de los objetos mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Vea un vídeo de demostración de esta función](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personalización del encabezado de tarea

Como administrador de Workfront o de grupos, ahora puede personalizar los campos que se muestran en el encabezado de una tarea cuando utilice una plantilla de diseño.

Esta actualización incluye las siguientes mejoras:

* Elimine o reorganice los campos existentes del encabezado de la tarea.

* Agregue campos nuevos de Información general de la tarea no editables. No puede añadir campos personalizados o campos que se puedan editar. También puede mostrar campos editables que estén actualmente en el encabezado de la tarea (por ejemplo, Estado o Porcentaje completado).

* El encabezado de la tarea puede incluir hasta cinco campos.

Antes de esta versión, solo se podían personalizar los encabezados de proyecto.

Para obtener más información, vea [Personalizar encabezados de objeto mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Inclusión anticipada de funciones para las últimas funciones de los tableros

Estamos encantados de abrir nuevas funciones de tableros para la inclusión anticipada de funciones. Esta herramienta opcional está disponible para todas las organizaciones.

Solo un administrador de Workfront puede adherirse a las funciones anticipadas. Cuando el administrador incluye las funciones anticipadas, se incluye a todos los usuarios de la organización y las funciones adicionales se habilitan en el entorno de producción de Workfront.

Para obtener más información, consulte [Inclusión anticipada de funciones para tableros de Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## El editor de cálculo de campos de formulario personalizados muestra información de error

>[!NOTE]
>
>Esta función se introdujo por primera vez en el entorno de vista previa durante el periodo de tiempo de lanzamiento de la versión 22.3. Se lanza al entorno de producción con la versión 22.4.

Editar cálculos para campos personalizados ahora es más fácil con información de error útil indicada directamente en el cálculo. Mientras crea un campo calculado en un formulario personalizado, los errores se resaltan en rosa. Cuando pasa el puntero por encima de la parte resaltada, se muestra información del objeto para describir el problema.

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migración a la experiencia unificada de Adobe

NOTA: Esta migración se ha pospuesto hasta el primer y segundo trimestre de 2023. Se notificará a todos los clientes afectados en ese momento.

Si su organización se ha incorporado a Adobe Admin Console, la instancia de Workfront se migrará a Adobe Unified Experience con la versión 22.4.

La experiencia unificada de Adobe incluye lo siguiente:

* Un único inicio de sesión para todas las aplicaciones de Adobe mediante Adobe Experience Cloud

* Un “conmutador de organizaciones” para alternar entre organizaciones y entornos de Workfront

* Navegación con opciones para páginas de Workfront, preferencias de Adobe Experience Cloud y su perfil de Workfront

Para obtener más información, consulte [Experiencia unificada de Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Vea un vídeo de demostración de esta función.](https://video.tv.adobe.com/v/3412388/){target=_blank}
