---
title: Adobe Workfront Planning Access Overview
description: No todos los usuarios de la organización tienen el mismo acceso y permisos para utilizar Adobe Workfront Planning. Este artículo describe el acceso y los permisos que los usuarios podrían tener para utilizar las capacidades de Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 31%

---


# Información general de acceso a Adobe Workfront Planning

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Workfront Planning, una funcionalidad adicional de Adobe Workfront.
>
>Your company must purchase an additional package for Workfront Planning to access its capabilities.
>
>For more information, contact your account manager
>
>Para obtener más información sobre Workfront Planning, consulte [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Existen restricciones de licencia y de permisos de uso compartido para utilizar Adobe Workfront Planning.

This article describes the access and settings that you need in place to use the capabilities of Workfront Planning.

## Requisitos de acceso

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

You must have the following access to use Workfront Planning:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
 <tr>
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td>
   <td>
   <p>Cualquier paquete de Workfront y Planning</p>
   <p>Cualquier paquete de flujo de trabajo y planificación</p>

<p><b>NOTA</b></p>

<p>For access to connectable record types:</p>
   <ul><li><p>Any Workfront package and a Planning package</p></li>
   <li><p>Any Workflow and a Planning Prime and Ultimate package</p></li></ul>

<p>For access to global record types:</p>
   <ul><li><p>Any Workfront package and a Planning Plus package</p></li>
   <li><p>Any Workflow package and a Planning Prime and Ultimate package</p></li></ul> </td></tr>

<!--
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Only users added to the Adobe Identity Management System (IMS) can be granted permissions and added to Planning fields.</p>
   <p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  -->

<tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <ul><li><p>Any, to view Workfront Planning information</p></li>
   <li><p>Estándar, para crear espacios de trabajo y vistas</p></li></ul>
    </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <ul>
   <li><p>View or higher permissions to workspaces, record types and views that you did not create to access them and their objects.</p></li>
   <li><p>Contribute or higher permissions to workspaces and record types that you did not create to edit them and create, edit, or delete record types and records.</p></li>
   <li><p>Contribute or higher permissions to views that you did not create, to edit, delete, and share them</p>
   </li>
    <li><p>Los administradores del sistema pueden administrar los espacios de trabajo que no hayan creado. </p></li>
    <li><p>System Administrators cannot access views they did not create. </p></li></ul>
   <p>Para obtener información acerca de los permisos de uso compartido para objetos de Workfront Planning, consulte 
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Información general sobre los permisos de uso compartido en Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> 
<p>Los usuarios estándar y los administradores del sistema tienen las áreas de Planning habilitadas de forma predeterminada.</p>
<p> A los usuarios con una licencia Light o Contributor se les debe asignar una plantilla de diseño que incluya la opción Planning en las áreas siguientes:</p>
   <ul><li>Menú principal</li>
   <li>Left panel of projects, portfolios, and programs</li>
   </ul>   
</td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Share the Planning area using a layout template

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

Standard users and System Administrators have the Planning areas enabled by default in the following areas:

* Menú principal
* Left panel of projects, portfolios, or programs

Your system administrator must add the Planning areas to you, if you have any other Workfront license and you need to contribute to Workfront Planning work.

El administrador puede añadir la opción de planificación a las siguientes áreas modificando y asignándole una plantilla de diseño:

* Menú principal
* Landing page
* Panel izquierdo para proyectos, portafolios y programas
* Fijadores

To add or remove Workfront Planning areas from users of your Workfront instance:

1. Inicie sesión en **Workfront** como administrador.

1. Vaya a **Menú principal** > **Configuración** > **Interfaz** > **Plantillas de diseño** y abra o cree una plantilla de diseño.

   Para obtener información acerca de cómo personalizar una plantilla de diseño, vea [Crear y administrar plantillas de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Asigne la plantilla de diseño a los usuarios a los que desea tener acceso en Workfront Planning.

   Para obtener más información, consulte [Asignar usuarios a una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Todos los usuarios asignados a la plantilla pueden ahora acceder a Workfront Planning en su menú principal.

   Los usuarios pueden empezar a crear espacios de trabajo, tipos de registros, registros y campos.

## Assign licenses to users

You can assign licenses to users when you configure their Access level while editing or creating them.

Para obtener más información, consulte [Editar el perfil de un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Configuración del nivel de acceso

No hay controles de nivel de acceso de Workfront para Workfront Planning.

Los usuarios con cualquier tipo de licencia de Workfront pueden acceder a Workfront Planning.

<!--For information about granting access in Workfront, see [Create and modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Conceder permisos

Puede conceder permisos a las siguientes entidades en Workfront Planning:

* Espacios de trabajo
* Tipos de registro
* Vistas
  <!--move this above Views: * <span class="preview">Records</span>-->

Para obtener más información, consulte [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Your Adobe Workfront license type works with your Workfront Planning permissions to give you access to view, contribute, or manage Workfront Planning objects.

Para obtener información acerca de cómo afectan los tipos de licencia a los niveles de permisos de los objetos de Workfront Planning, consulte [Descripción general del tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


