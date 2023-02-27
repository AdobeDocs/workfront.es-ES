---
title: Actividad de la versión de Workfront Fusion:&nbsp;semana del 30 de agosto de 2021
description: Actividad de la versión de Workfront Fusion:&nbsp;semana del 30 de agosto de 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: semana del 30 de agosto de 2021

En esta página se describen todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 30 de agosto de 2021.

Para obtener una lista de todos los cambios recientes, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obtener una lista de las correcciones de errores recientes en Workfront Fusion, consulte la [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) y compruebe si hay actualizaciones etiquetadas como Actualización de mantenimiento de Workfront Fusion.

## Filtre los eventos de déclencheur del módulo Workfront > Watch events

1. Configure un filtro personalizado para los eventos de déclencheur en el módulo Workfront > Watch events

   Para reducir el número de ejecuciones de escenarios innecesarias, se ha actualizado el módulo Workfront > Watch records para habilitar el filtrado de eventos. Ahora, puede establecer un filtro cuando cree un weblink. Esto permite que el escenario tenga déclencheur únicamente cuando el evento cumple determinados criterios.

   El filtro de eventos ofrece actualmente las siguientes operaciones:

   * Igual: Déclencheur un escenario solo cuando un evento coincide con las condiciones del filtro. Por ejemplo, puede configurar un filtro que almacene en déclencheur un escenario solo si el evento se produce en un proyecto específico.
   * Distinto a: Déclencheur un escenario solo si un evento no coincide con las condiciones del filtro. Por ejemplo, puede crear un filtro que almacene en déclencheur un escenario solo si el problema en el que se produce un evento no tiene el estado Cerrado.

   Anteriormente, el módulo Watch records recuperaba todos los registros. Los usuarios solo podían filtrar configurando filtros más adelante en el escenario.

   Para aprovechar el filtrado de eventos, cree un nuevo vínculo web en el módulo Watch events . Actualmente no es posible editar los vínculos web existentes para incluir esta funcionalidad. Le recomendamos encarecidamente que cree nuevos enlaces web utilizando filtros de evento para los escenarios existentes.

1. Filtrar eventos activados por la conexión actual.

   Para facilitar la configuración de los enlaces web para el módulo Workfront > Watch events , hemos incluido el filtro de eventos más común. Ahora, el enlace web tiene la opción de filtrar cualquier cambio realizado por módulos usando la conexión especificada para el módulo Watch events. En otras palabras, con este filtro habilitado, cualquier cambio realizado por el usuario de Workfront asociado con esa conexión no puede almacenar en déclencheur el escenario.

   Anteriormente, este filtro no estaba disponible. Por lo tanto, fue más fácil para los cambios realizados en los módulos de Workfront almacenar en déclencheur escenarios que contenían esos módulos, causando potencialmente que los escenarios se déclencheur en un bucle infinito.

Para obtener más información sobre los filtros de evento en el módulo Workfront > Watch events , consulte [Módulos de Adobe Workfront](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

