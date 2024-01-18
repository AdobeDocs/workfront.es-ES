---
title: 22.2 Mejoras de la gestión de recursos
description: 22.2 Mejoras de la gestión de recursos
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 22.2 Mejoras de la gestión de recursos

Esta página describe todas las mejoras de Administración de recursos realizadas con la versión 22.2 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción de

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 22.2, consulte [Información general de la versión 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Mejoras en la navegación del Distribuidor de cargas de trabajo

Para mejorar su experiencia al utilizar el Distribuidor de cargas de trabajo, hemos introducido las siguientes mejoras:

* Los botones Cancelar y Guardar al ajustar las asignaciones ahora son fijos, incluso cuando la tarea es más larga que el periodo de tiempo incluido en la pantalla o cuando se muestra el panel Resumen.
* El panel izquierdo que muestra los nombres de los usuarios y los elementos de trabajo ahora es fijo, para permitirle desplazarse horizontalmente durante períodos de tiempo más largos y seguir pudiendo leer los nombres de los elementos enumerados en el panel.
* Puede contraer y expandir todos los elementos enumerados en el panel izquierdo con un solo clic en lugar de en el nivel de usuario o proyecto.
* El panel izquierdo ahora también se puede cambiar de tamaño.
* Ahora hay un modo de pantalla completa para el Distribuidor de cargas de trabajo.

Para obtener más información sobre cómo navegar por el Distribuidor de cargas de trabajo, consulte [Navegación por el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Acceso a asignaciones avanzadas en el Distribuidor de cargas de trabajo

Para que la asignación de elementos de trabajo sea más fácil y precisa, ahora puede realizar asignaciones avanzadas cuando asigne elementos de trabajo manualmente en el Distribuidor de cargas de trabajo. Antes de esta mejora, podía acceder a Asignaciones avanzadas cuando editaba elementos, desde los encabezados de los elementos o en las listas.

Para obtener más información, consulte [Asignar trabajo manualmente mediante el Distribuidor de cargas de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nueva fórmula para calcular la disponibilidad del usuario cuando se selecciona la preferencia Horario predeterminado

Para proporcionar información más precisa en las herramientas de administración de recursos, hemos cambiado la fórmula que utiliza Workfront para calcular la disponibilidad del usuario cuando el administrador de Workfront selecciona El horario predeterminado en las preferencias de administración de recursos. Con la nueva actualización, Workfront utiliza la siguiente fórmula para calcular la disponibilidad del usuario:

Horas disponibles del usuario = (Horas programadas predeterminadas - Excepciones) &#42; FTE - Horas libres

Antes de esta actualización, Workfront utilizaba la siguiente fórmula para calcular la disponibilidad del usuario cuando se seleccionaba El horario predeterminado:

Horas disponibles del usuario = (Horas programadas predeterminadas - (Excepciones de horario + Horas libres)) &#42; Valor de FTE de usuario

Para obtener más información, consulte [Configurar preferencias de administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

