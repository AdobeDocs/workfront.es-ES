---
title: Mejoras en los informes del tercer trimestre de 2025
description: Mejoras del proyecto del tercer trimestre de 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 25%

---

# Mejoras en los informes del tercer trimestre de 2025

Esta página describe todas las mejoras de creación de informes realizadas con la versión del tercer trimestre de 2025 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2025, consulte [Información general de la versión del tercer trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Los comodines del usuario ya no devuelven resultados con un valor nulo al filtrar

>[!NOTE]
>
>* Vista previa: 30 de abril de 2025
>* Versión rápida de producción: 15 de mayo de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Hemos actualizado el comportamiento de los comodines del usuario para excluir el valor nulo al filtrar un informe. Este cambio ayuda al filtro a producir resultados más precisos, en lugar de devolver resultados que no tienen un usuario configurado correctamente (un resultado nulo).

Anteriormente, cuando un comodín de usuario producía un valor nulo, un informe mostraba todos los registros que también tenían un valor nulo.

Este cambio se aplica a los siguientes filtros comodín:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

