---
title: Mejoras de informes del tercer trimestre de 2025
description: Mejoras del proyecto del tercer trimestre de 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 17%

---

# Mejoras de informes del tercer trimestre de 2025

Esta página describe todas las mejoras de los informes realizadas con la versión del tercer trimestre de 2025 en el entorno de previsualización. Estas mejoras estarán disponibles en el entorno de producción, como se ha indicado.

Para obtener una lista de todos los cambios disponibles en este punto del ciclo de la versión del tercer trimestre de 2025, consulte [Información general de la versión del tercer trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Seguridad de entrega de informes mejorada

* Vista previa: viernes, 26 de junio de 2025
* Producción: Implementación gradual desde el 26 de junio de 2025 hasta el 9 de julio de 2025

Hemos mejorado la entrega de informes programados para garantizar que las notificaciones de Workfront solo se envíen a los dominios de correo electrónico aprobados en la lista de permitidos.

Anteriormente, si su organización había definido una limitación en qué dominios de correo electrónico se incluían las notificaciones de Workfront, ejecutaríamos una comprobación en la lista de permitidos a medida que se añadían correos electrónicos.

Ahora, también realizamos una comprobación a medida que se envía el correo electrónico para garantizar que la dirección de correo electrónico introducida cumpla con la lista de permitidos de correo electrónico. Esta comprobación mejorada se aplica tanto a las direcciones de correo electrónico asociadas a los usuarios como a los correos electrónicos ad hoc añadidos a la lista de destinatarios del informe.

Para obtener más información, consulte [Programar la entrega automática de informes](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


## Los comodines de usuario ya no devuelven resultados con un valor nulo al filtrar

>[!NOTE]
>
>* Vista previa: 30 de abril de 2025
>* Versión rápida de producción: viernes, 15 de mayo de 2025
>* Producción para todos los clientes: 17 de julio de 2025

Hemos actualizado el comportamiento de los caracteres comodín de usuario para excluir el valor nulo al filtrar un informe. Este cambio ayuda al filtro a producir resultados más precisos, en lugar de devolver resultados que no tienen un usuario configurado correctamente (un resultado nulo).

Anteriormente, cuando un comodín de usuario generaba un valor nulo, un informe mostraba todos los registros que también tenían un valor nulo.

Este cambio se aplica a los siguientes filtros de comodines:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
