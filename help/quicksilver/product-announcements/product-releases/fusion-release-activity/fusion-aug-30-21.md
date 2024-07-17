---
title: 'Actividad de la versión de Workfront Fusion: &nbsp;Semana del 30 de agosto de 2021'
description: 'Actividad de la versión de Workfront Fusion: &nbsp;Semana del 30 de agosto de 2021'
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: Semana del 30 de agosto de 2021

Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 30 de agosto de 2021.

Para obtener una lista de todos los cambios recientes, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obtener una lista de las correcciones de errores recientes en Workfront Fusion, consulte la página [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) y busque cualquier actualización denominada Actualización de mantenimiento de Workfront Fusion.

## Filtrar eventos que almacenan en déclencheur el módulo Workfront > Ver eventos

1. Configure un filtro personalizado para los eventos que entran en déclencheur con el módulo Workfront > Ver eventos

   Para reducir el número de ejecuciones de escenarios innecesarias, hemos actualizado el módulo Workfront > Ver registros para habilitar el filtrado de eventos. Ahora, puede establecer un filtro cuando cree un webhook. Esto permite que el escenario entre en déclencheur únicamente cuando el evento cumpla determinados criterios.

   El filtro de eventos ofrece actualmente las siguientes operaciones:

   * Equal: Almacene en Déclencheur un escenario solo cuando un evento coincida con las condiciones del filtro. Por ejemplo, puede configurar un déclencheur que almacene en caché un escenario solo si el evento se produce en un proyecto específico.
   * Not Equal: Almacena en Déclencheur un escenario solo si un evento no coincide con las condiciones del filtro. Por ejemplo, puede crear un filtro que almacene en déclencheur un escenario solo si el problema en el que se produce un evento no tiene el estado Cerrado.

   Anteriormente, el módulo Observar registros recuperaba todos los registros. Los usuarios solo podían filtrar configurando filtros más adelante en el escenario.

   Para aprovechar el filtrado de eventos, cree un nuevo webhook en el módulo Ver eventos. Actualmente no es posible editar los webhooks existentes para incluir esta funcionalidad. Le recomendamos encarecidamente que cree nuevos webhooks utilizando filtros de evento para sus escenarios existentes.

1. Filtrar los eventos activados por la conexión actual.

   Para que tus webhooks sean más fáciles de configurar para el módulo Workfront > Ver eventos, hemos incluido el filtro de eventos más común. Ahora, el gancho web tiene la opción de filtrar cualquier cambio realizado por módulos usando la conexión especificada para el módulo Watch events. En otras palabras, con este filtro habilitado, cualquier cambio realizado por el usuario de Workfront asociado con esa conexión no puede almacenar el déclencheur en el escenario.

   Anteriormente, este filtro no estaba disponible. Por lo tanto, era más fácil para los cambios realizados en los módulos de Workfront almacenar en déclencheur los escenarios que contenían esos módulos, lo que provocaba que los escenarios se almacenaran en déclencheur en un bucle infinito.

Para obtener más información sobre los filtros de eventos en el módulo Workfront > Ver eventos, consulte [módulos de Adobe Workfront](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

