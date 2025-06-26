---
title: Mejoras en los informes del tercer trimestre de 2025
description: Mejoras del proyecto del tercer trimestre de 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 15%

---

# Mejoras en los informes del tercer trimestre de 2025

Esta página describe todas las mejoras de creación de informes realizadas con la versión del tercer trimestre de 2025 en el entorno de vista previa. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2025, consulte [Información general de la versión del tercer trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Seguridad de entrega de informes mejorada

* Vista previa: viernes, 26 de junio de 2025
* Producción: Despliegue gradual del 26 de junio de 2025 al 9 de julio de 2025

Se ha mejorado la entrega de informes programados para garantizar que las notificaciones de Workfront solo se envíen a dominios de correo electrónico aprobados en la lista de permitidos.

Anteriormente, si su organización había definido una limitación en los dominios de correo electrónico para las notificaciones de Workfront, ejecutábamos una comprobación con la lista de permitidos a medida que se añadían correos electrónicos.

Ahora, también comprobamos si el correo electrónico se envía para garantizar que la dirección de correo electrónico introducida cumpla con la lista de permitidos de correo electrónico. Esta comprobación mejorada se aplica tanto a las direcciones de correo electrónico asociadas con los usuarios como a los correos electrónicos ad hoc añadidos a la lista de destinatarios del informe.

Para obtener más información, consulte [Programar una entrega automática de informes](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


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
