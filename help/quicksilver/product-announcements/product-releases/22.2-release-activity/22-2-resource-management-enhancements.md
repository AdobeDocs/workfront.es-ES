---
title: 22.2 Mejoras en la administración de recursos
description: 22.2 Mejoras en la administración de recursos
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
TQID: https://experienceleague.adobe.com/X2dBmB8Qyiwg9hM60af6GRBDGT4KkH6Jjs2A-S-TWVg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 86%

---

# 22.2 Mejoras en la administración de recursos

Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 22.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.2, consulte [Información general sobre la versión 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Mejoras en la navegación del Distribuidor de cargas de trabajo

Para mejorar la experiencia al utilizar el Distribuidor de cargas de trabajo, se introdujeron las siguientes mejoras:

* Los botones Cancelar y Guardar al ajustar las asignaciones ya son fijos, incluso cuando la tarea sea más larga que el periodo de tiempo incluido en la pantalla o cuando se muestre en el panel Resumen.
* El panel izquierdo que muestra los nombres de los usuarios y los elementos de trabajo ya es fijo para permitir desplazarse horizontalmente durante períodos de tiempo más largos y seguir pudiendo leer los nombres de los elementos enumerados en el panel.
* Es posible contraer y expandir todos los elementos enumerados en el panel izquierdo con un solo clic en lugar de en el nivel de usuario o proyecto.
* El panel izquierdo ya se puede cambiar de tamaño también.
* Ya hay un modo de pantalla completa para el Distribuidor de cargas de trabajo.

Para obtener más información sobre cómo navegar por el Distribuidor de cargas de trabajo, consulte [Navegar por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Acceso a asignaciones avanzadas en el Distribuidor de cargas de trabajo

Para que la asignación de elementos de trabajo sea más fácil y precisa, ya es posible realizar asignaciones avanzadas al asignar elementos de trabajo manualmente en el Distribuidor de cargas de trabajo. Antes de esta mejora, era posible acceder a las asignaciones avanzadas al editar elementos, desde los encabezados de los elementos o en las listas.

Para obtener más información, consulte [Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nueva fórmula para calcular la disponibilidad del usuario cuando se selecciona la preferencia Horario predeterminado

Para proporcionar información más precisa en las herramientas de administración de recursos, se cambió la fórmula que utiliza Workfront para calcular la disponibilidad del usuario cuando el administrador de Workfront selecciona El horario predeterminado en las preferencias de administración de recursos. Con la nueva actualización, Workfront utiliza la siguiente fórmula para calcular la disponibilidad del usuario:

Horas disponibles del usuario = (Horas programadas predeterminadas - Excepciones) &#42; FTE - Horas de descanso

Antes de esta actualización, Workfront utilizaba la siguiente fórmula para calcular la disponibilidad del usuario cuando se seleccionaba El horario predeterminado:

Horas disponibles del usuario = (Horas programadas predeterminadas - (Excepciones de horario + Horas libres)) &#42; Valor de FTE del usuario

Para obtener más información, consulte [Configurar las preferencias de administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

