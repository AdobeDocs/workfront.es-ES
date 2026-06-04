---
title: Mejoras en los informes del tercer trimestre de 2025
description: Mejoras del proyecto del tercer trimestre de 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/XN5rfSeje0azVxpC4uBSDn5mg2C9Oyik2awD5pQy3Jo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
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
