---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Acceso a objetos y áreas por parte de las nuevas licencias
description: La siguiente tabla indica el nivel de acceso más alto (Editar o Ver) que cada una de las licencias de Adobe Workfront permite para los objetos y las áreas de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 17%

---

# Acceso a objetos y áreas por parte de las nuevas licencias

La siguiente tabla indica el nivel de acceso más alto (Editar o Ver) que cada una de las licencias de Adobe Workfront permite para los objetos y las áreas de Workfront.

* **Ver**: El usuario puede revisar y compartir artículos.
* **Editar**: El usuario puede crear, editar, eliminar y compartir elementos.

   >[!NOTE]
   >
   >Cuando otro usuario comparte un objeto, el usuario que comparte puede especificar permisos que limiten su capacidad para editarlo. Para obtener más información, consulte [Información general sobre cómo compartir permisos en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Estándar</td>
        <td>Ligero</td>
        <td>Colaborador</td>
        <td>Externo</td>
    </tr>
    <tr>
        <td>Proyectos</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Ver (solo la página Detalles)</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Tareas</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Vista</td>
        <td>Vista</td>
    </tr>
    <tr>
        <td>Problemas</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Portafolios</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Programas</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Informes, tableros y calendarios</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Vista*</td>
        <td>Ver (solo para calendarios, sin permisos de uso compartido)</td>
    </tr>
    <tr>
        <td>Filtros, vistas y agrupaciones</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Documentos</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Ver (sin permisos de uso compartido)</td>
    </tr>
    <tr>
        <td>Usuarios</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Vista</td>
        <td>Vista</td>
    </tr>
    <tr>
        <td>Equipos</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Vista</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Plantillas</td>
        <td>Editar</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Datos financieros</td>
        <td>Editar</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Administración de recursos</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Planificador de escenarios</td>
        <td>Editar</td>
        <td>Vista</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Workfront Goals</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Editar</td>
        <td>Sin acceso</td>
    </tr>
</table>

&#42; Los usuarios con una licencia de colaborador solo pueden ver los informes, tableros y calendarios que se han compartido con ellos.

>[!NOTE]
>
>Los usuarios con una licencia Light o una licencia de colaborador tienen capacidades de uso compartido limitadas. Para obtener más información, consulte [Información general sobre licencias](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>Los usuarios externos no pueden buscar elementos en Workfront. Pueden ver documentos y calendarios que se han compartido específicamente con ellos. También pueden ver los usuarios que comparten artículos con ellos.

Puede encontrar información detallada sobre lo que permiten los niveles de acceso para cada objeto y área en los siguientes artículos:

* [Concesión de acceso a proyectos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Concesión de acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Concesión de acceso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Concesión de acceso a documentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Concesión de acceso a portafolios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Concesión de acceso a programas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Concesión de acceso a equipos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Concesión de acceso a plantillas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Conceder acceso a la Administración de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Conceder acceso al Planificador de escenario](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Conceder acceso a los objetivos de Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
