---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Acceso a objetos y áreas por tipo de licencia (heredada)
description: En la siguiente tabla se indica el nivel más alto de acceso (Editar o Ver) que cada una de las licencias de Adobe Workfront permite para los objetos y áreas en Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
TQID: https://experienceleague.adobe.com/UV5Oh-MjdnrGMJv62onf7uC8sFcbsyyQiAoJsxK9NFk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: d3382524-5489-431b-bde9-271ab257bc37id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 482
ht-degree: 73%

---

# Acceso a objetos y áreas por tipo de licencia (heredada)

<!-- Audited: 11/2025 -->

>[!NOTE]
>
>La información de este artículo hace referencia a los niveles de acceso heredados. Para obtener información acerca de los niveles de acceso actuales, consulte [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

En la siguiente tabla se indica el nivel más alto de acceso (Editar o Ver) que cada una de las licencias de Adobe Workfront permite para los objetos y áreas en Workfront.

* Ver: el usuario puede revisar y compartir elementos.
* Editar: el usuario puede crear, editar, eliminar y compartir elementos.

  >[!NOTE]
  >
  >Cuando otro usuario comparte un objeto, dicho usuario puede especificar permisos que limiten su capacidad para editarlo. Para obtener más información sobre los nuevos tipos de licencia, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

  >[!NOTE]
  >
  >Este artículo contiene información sobre el acceso a objetos para los tipos de licencia heredados. Para obtener información sobre los nuevos tipos de licencia, consulte [Información general sobre los nuevos niveles de acceso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) y [Información general sobre las nuevas licencias](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

|   | Plan | Trabajo | Revisar | Solicitud | Externo |
|---|---|---|---|---|---|
| Proyectos | Editar | Editar (sin permisos de creación) | Ver | Ver (solo la página Detalles) | Sin acceso |
| Tareas | Editar | Editar | Ver | Ver | Sin acceso |
| Problemas | Editar | Editar | Editar | Editar | Sin acceso |
| Portafolios | Editar | Ver | Ver | Sin acceso | Sin acceso |
| Programas | Editar | Ver | Ver | Sin acceso | Sin acceso |
| Informes, paneles de control y calendarios | Editar | Ver | Ver | Vista&#42; | Ver (solo para calendarios, sin permisos de uso compartido) |
| Filtros, vistas y agrupaciones | Editar | Editar | Editar | Editar | Sin acceso |
| Documentos | Editar | Editar | Editar | Editar | Ver (sin permisos de uso compartido) |
| Usuarios | Editar | Ver | Ver | Ver | Ver |
| Equipos | Editar | Editar | Ver | Ver | Sin acceso |
| Plantillas | Editar | Sin acceso | Sin acceso | Sin acceso | Sin acceso |
| Datos financieros | Editar | Ver (solo el área Finanzas en Detalles del proyecto) | Ver | Sin acceso | Sin acceso |
| Administración de recursos | Editar | Ver | Ver | Sin acceso | Sin acceso |
| Planificador de escenarios | Editar | Editar | Editar | Sin acceso | Sin acceso |
| Workfront Goals | Editar | Editar | Editar | Editar | Sin acceso |

&#42; Los usuarios con una licencia de solicitud solo pueden ver los informes, tableros y calendarios que se han compartido con ellos.

>[!NOTE]
>
>Los usuarios con una licencia de revisión o de solicitud tienen capacidades de uso compartido limitadas. Para obtener más información, consulte [Información general sobre las licencias](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Los usuarios externos no pueden buscar elementos en Workfront. Pueden ver documentos y calendarios que se comparten específicamente con ellos. También pueden ver los usuarios que comparten elementos con ellos.

Puede encontrar información detallada sobre lo que permiten los niveles de acceso para cada objeto y área en los siguientes artículos:

* [Conceder acceso a los proyectos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Conceder acceso a los problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Conceder acceso a los documentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Conceder acceso a los portafolios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Conceder acceso a los programas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Conceder acceso a informes, paneles de control y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Conceder acceso a los equipos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Conceder acceso a las plantillas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Conceder acceso a Administración de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Conceder acceso al Planificador de escenarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Conceder acceso a Adobe Workfront Goals](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
