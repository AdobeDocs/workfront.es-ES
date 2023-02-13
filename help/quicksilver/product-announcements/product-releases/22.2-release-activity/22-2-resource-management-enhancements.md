---
title: 22.2 Mejoras en la gestión de recursos
description: 22.2 Mejoras en la gestión de recursos
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 22.2 Mejoras en la gestión de recursos

En esta página se describen todas las mejoras realizadas en la administración de recursos con la versión 2.2 del entorno de vista previa. Estas mejoras estarán disponibles en el entorno Producción

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

la semana del 4 de abril de 2022.

Para obtener una lista de todos los cambios disponibles con la versión 2.2, consulte [Resumen de la versión 2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Mejoras en la navegación del equilibrador de carga de trabajo

Para mejorar su experiencia al utilizar el equilibrador de carga de trabajo, hemos introducido las siguientes mejoras:

* Los botones Cancelar y Guardar al ajustar asignaciones ahora son fijos, incluso cuando la tarea es más larga que el periodo de tiempo incluido en la pantalla o cuando se muestra el panel Resumen.
* El panel izquierdo que muestra los nombres de los usuarios y los elementos de trabajo es ahora fijo, para permitirle desplazarse horizontalmente durante períodos de tiempo más largos y poder seguir leyendo los nombres de los elementos enumerados en el panel.
* Puede contraer y expandir todos los elementos enumerados en el panel izquierdo con un clic en lugar de en el nivel de usuario o proyecto.
* Ahora también se puede cambiar el tamaño del panel izquierdo.
* Ahora hay un modo de pantalla completa para el equilibrador de carga de trabajo.

Para obtener más información sobre cómo navegar por el equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Acceso a asignaciones avanzadas en el equilibrador de carga de trabajo

Para que la asignación de elementos de trabajo sea más fácil y precisa, ahora puede hacer asignaciones avanzadas cuando asigna elementos de trabajo manualmente en el equilibrador de carga de trabajo. Antes de esta mejora, podía acceder a Asignaciones avanzadas al editar elementos, desde los encabezados de los elementos o en listas.

Para obtener más información, consulte [Asignar trabajo manualmente mediante el equilibrador de carga de trabajo](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nueva fórmula para calcular la disponibilidad del usuario cuando se selecciona la preferencia Programación predeterminada

Para proporcionar información más precisa en las herramientas de administración de recursos, hemos cambiado la fórmula que utiliza Workfront para calcular la disponibilidad del usuario cuando el administrador de Workfront selecciona La programación predeterminada en las preferencias de administración de recursos. Con la nueva actualización, Workfront utiliza la siguiente fórmula para calcular la disponibilidad del usuario:

Horas disponibles del usuario = (Horas de programación predeterminadas - Excepciones) &#42; FTE - Horas de inactividad

Antes de esta actualización, Workfront utilizaba la siguiente fórmula para calcular la disponibilidad del usuario cuando se seleccionaba La programación predeterminada :

Horas disponibles del usuario = (Horas de programación predeterminadas - (Excepciones de programación + Horas de descanso)) &#42; Valor FTE del usuario

Para obtener más información, consulte [Configurar las preferencias de Administración de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

