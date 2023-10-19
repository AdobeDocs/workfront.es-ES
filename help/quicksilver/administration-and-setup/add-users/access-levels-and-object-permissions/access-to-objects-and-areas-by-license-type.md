---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Acceso a objetos y áreas por tipo de licencia
description: La siguiente tabla indica el nivel más alto de acceso (Editar o Ver) que cada una de las licencias de Adobe Workfront permite para los objetos y áreas en Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 20%

---

# Acceso a objetos y áreas por tipo de licencia

La siguiente tabla indica el nivel más alto de acceso (Editar o Ver) que cada una de las licencias de Adobe Workfront permite para los objetos y áreas en Workfront.

* **Ver**: el usuario puede revisar y compartir elementos.
* **Editar**: el usuario puede crear, editar, eliminar y compartir elementos.

  >[!NOTE]
  >
  >Cuando otro usuario comparte un objeto, el que comparte puede especificar permisos que limiten su capacidad para editarlo. Para obtener más información, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | Plan | Trabajo | Revisar | Solicitud | Externo |
|---|---|---|---|---|---|
| Proyectos | Editar | Editar (sin permisos de creación) | Vista | Ver (solo la página Detalles) | Sin acceso |
| Tareas | Editar | Editar | Vista | Vista | Vista |
| Problemas | Editar | Editar | Editar | Editar | Sin acceso |
| Portafolios | Editar | Vista | Vista | Sin acceso | Sin acceso |
| Programas | Editar | Vista | Vista | Sin acceso | Sin acceso |
| Informes, tableros y calendarios | Editar | Vista | Vista | Vista&#42; | Ver (solo para calendarios, sin permisos de uso compartido) |
| Filtros, vistas y agrupaciones | Editar | Editar | Editar | Editar | Sin acceso |
| Documentos | Editar | Editar | Editar | Editar | Ver (sin permisos de uso compartido) |
| Usuarios | Editar | Vista | Vista | Vista | Vista |
| Equipos | Editar | Editar | Vista | Vista | Sin acceso |
| Plantillas | Editar | Sin acceso | Sin acceso | Sin acceso | Sin acceso |
| Datos financieros | Editar | Ver (solo el área Finanzas en Detalles del proyecto) | Vista | Sin acceso | Sin acceso |
| Administración de recursos | Editar | Vista | Vista | Sin acceso | Sin acceso |
| Planificador de escenarios | Editar | Editar | Editar | Sin acceso | Sin acceso |
| Workfront Goals | Editar | Editar | Editar | Editar | Sin acceso |

&#42; Los usuarios con una licencia de solicitud solo pueden ver los informes, tableros y calendarios que se han compartido con ellos.

>[!NOTE]
>
>Los usuarios con una licencia de revisión o de solicitud tienen capacidades de uso compartido limitadas. Para obtener más información, consulte [Resumen de licencias de Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Los usuarios externos no pueden buscar elementos en Workfront. Pueden ver documentos y calendarios que se comparten específicamente con ellos. También pueden ver los usuarios que comparten elementos con ellos.

Puede encontrar información detallada sobre lo que permiten los niveles de acceso para cada objeto y área en los siguientes artículos:

* [Concesión de acceso a proyectos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Conceder acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Conceder acceso a los problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Conceder acceso a documentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Conceder acceso a portafolios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Concesión de acceso a los programas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Concesión de acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Conceder acceso a los equipos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Concesión de acceso a las plantillas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Concesión de acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Conceder acceso a Administración de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Conceder acceso al Scenario Planner](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Concesión de acceso a Adobe Workfront Goals](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
