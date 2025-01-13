---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Acceso a objetos y áreas con nuevas licencias
description: En la siguiente tabla se indica el nivel más alto de acceso (Editar o Ver) que cada una de las licencias de Adobe Workfront permite para los objetos y áreas en Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: b333ea67bb909ca55306f6474832c275ebad590c
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 95%

---

# Acceso a objetos y áreas con nuevas licencias

<!-- Audited: 2/2024 -->

En la siguiente tabla se indica el nivel más alto de acceso (Editar o Ver) que cada una de las licencias de Adobe Workfront permite para los objetos y áreas en Workfront.

* **Ver**: el usuario puede revisar y compartir los elementos.
* **Editar**: el usuario puede crear, editar, eliminar y compartir los elementos. 

  >[!NOTE]
  >
  >Cuando otro usuario comparte un objeto, dicho usuario puede especificar permisos que limiten su capacidad para editarlo. Para obtener más información, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

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
        <td>Ver</td>
        <td>Ver</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Tareas</td>
        <td>Editar</td>
        <td>Ver</td>
        <td>Ver</td>
        <td>Ver</td>
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
        <td>Ver</td>
        <td>Ver</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Programas</td>
        <td>Editar</td>
        <td>Ver</td>
        <td>Ver</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Informes, paneles de control y calendarios</td>
        <td>Editar</td>
        <td>Ver</td>
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
        <td>Ver</td>
        <td>Ver</td>
        <td>Ver</td>
    </tr>
    <tr>
        <td>Equipos</td>
        <td>Editar</td>
        <td>Ver</td>
        <td>Ver</td>
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
        <td>Ver</td>
        <td>Sin acceso</td>
        <td>Sin acceso</td>
    </tr>
    <tr>
        <td>Planificador de escenarios</td>
        <td>Editar</td>
        <td>Ver</td>
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

&#42; Los usuarios con una licencia de colaborador solamente pueden ver los informes, paneles y calendarios que se han compartido con ellos.

>[!NOTE]
>
>* Los usuarios con una licencia Light o de colaborador tienen capacidades de uso compartido limitadas. Para obtener más información, consulte [Información general sobre las licencias](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>* Los usuarios externos no pueden buscar elementos en Workfront. Pueden ver documentos y calendarios que se comparten específicamente con ellos. También pueden ver los usuarios que comparten elementos con ellos.
>
>* Los usuarios colaboradores y los usuarios externos no pueden ver el contenido que se comparte en todo el sistema.  Debe compartirse con ellos explícitamente.

Puede encontrar información detallada sobre lo que permiten los niveles de acceso para cada objeto y área en los siguientes artículos:

* [Conceder acceso a los proyectos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Conceder acceso a los problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Conceder acceso a los documentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Conceder acceso a los portafolios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Conceder acceso a los programas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Conceder acceso a los usuarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Conceder acceso a los equipos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Conceder acceso a las plantillas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Conceder acceso a Administración de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Conceder acceso al Planificador de escenarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Conceder acceso a Adobe Workfront Goals](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
