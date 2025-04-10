---
title: Uso compartido de informes, paneles y calendarios
content-type: reference
product-area: user-management;reports;dashboards;calendars
navigation-topic: grant-and-request-access-to-objects
description: El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar informes, paneles y calendarios cuando asigna niveles de acceso. Para obtener más información sobre la concesión de acceso a informes, paneles y calendarios, consulte Concesión de acceso a informes, paneles y calendarios.
author: Alina
feature: Get Started with Workfront
exl-id: c2dac54b-6506-41b0-a7f2-6fafab12c2d1
source-git-commit: b8a2fea8c1eac376f49201dc840f7a4fcc67d759
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 100%

---

# Uso compartido de informes, paneles y calendarios

El administrador de Adobe Workfront concede a los usuarios acceso para ver o editar informes, paneles y calendarios cuando asigna niveles de acceso. Para obtener más información sobre cómo conceder acceso a informes, paneles y calendarios, vea [Concesión de acceso a informes, paneles y calendarios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Junto con el nivel de acceso que se concede a los usuarios, también puede darles permisos de Vista o Administración de informes, paneles o calendarios específicos a los que tiene acceso de Compartir. Para obtener información acerca de cómo conceder a los usuarios permisos de uso compartido en objetos, vea [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Los permisos son específicos de un elemento de Workfront y definen qué acciones se pueden realizar sobre ese elemento.

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los problemas, vea la sección [Informes](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Consideraciones sobre cómo compartir un informe, panel o calendario

Además de las consideraciones siguientes, consulte [Información general sobre los permisos de uso compartido en objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Un administrador de Workfront puede añadir o quitar permisos a cualquier elemento del sistema, para todos los usuarios, sin que tengan que ser el propietario de esos elementos.

* El creador de un informe, panel o calendario tiene permisos de Administración de forma predeterminada.
* Compartir informes, paneles y calendarios es similar a compartir cualquier otro objeto en Workfront.

  Para obtener más información sobre cómo compartir objetos en Workfront, vea [Uso compartido de un objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

  Consulte también los siguientes artículos para aprender a compartir informes, paneles y calendarios:

   * [Uso compartido de un informe en Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Uso compartido de un panel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Compartir un informe de calendario](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* Puede compartir informes y paneles de forma individual o masiva.

  Solo puede compartir calendarios de forma individual. No puede compartirlos por lotes.

* No puede compartir informes del sistema integrados. Solo puede compartir informes personalizados.

  Para obtener más información sobre cómo guardar un informe de sistema como un nuevo informe personalizado, vea [Creación de una copia de un informe](../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

* Puede conceder los siguientes permisos a informes, paneles y calendarios:

   * Ver
   * Administrar

* Cuando comparte un panel, los usuarios tienen permisos de Vista de forma predeterminada en todos los informes, calendarios y páginas externas del panel.
* Los usuarios con una licencia de solicitud no pueden ver un informe de todo el sistema. Un informe debe compartirse con los solicitantes de forma individual si necesitan verlo.
* Si un informe tiene una indicación y lo comparte de manera pública, los usuarios que accedan a este deben iniciar sesión en Workfront para poder ejecutar el informe con la indicación. Si no pueden iniciar sesión en Workfront, verán el informe sin la indicación aplicada.\
  Para obtener más información sobre las limitaciones al compartir informes con indicaciones, consulte la sección [Limitaciones del uso compartido de informes con indicaciones](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) en el artículo [Adición de una indicación a un informe](../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

* Puede quitar los permisos heredados de un informe o calendario.

  Para obtener más información acerca de cómo quitar permisos heredados de objetos, vea [Eliminación de permisos de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

* También puede compartir un informe o un calendario de forma pública o en todo el sistema.

  No puede compartir un panel de forma pública, pero sí en todo el sistema.

  >[!CAUTION]
  >
  >Se recomienda tener precaución al compartir con usuarios externos un objeto que contenga información confidencial. Esto les permite ver información sin ser usuarios de Workfront ni parte de su organización.
