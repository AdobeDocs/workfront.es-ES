---
title: Información general sobre el acceso a Adobe Workfront Planning
description: No todos los usuarios de la organización tienen el mismo acceso y permisos para utilizar Adobe Workfront Planning. Este artículo describe el acceso y los permisos que los usuarios podrían tener para utilizar las capacidades de Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 25%

---


# Información general sobre el acceso a Adobe Workfront Planning

<!--do not use the snippet for IMPORTANT , as it links to this article-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Workfront Planning, una funcionalidad adicional de Adobe Workfront.
>
>Su empresa debe adquirir un paquete adicional para que Workfront Planning pueda acceder a sus funciones.
>
>Para obtener más información, póngase en contacto con el administrador de cuentas
>
>Para obtener más información sobre Workfront Planning, consulte [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Existen restricciones de licencia y de permisos de uso compartido para utilizar Adobe Workfront Planning.

Este artículo describe el acceso y la configuración que necesita para utilizar las capacidades de Workfront Planning.

## Requisitos de acceso

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

Debe tener el siguiente acceso para utilizar Workfront Planning:

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

<p>Para acceder a tipos de registros conectables:</p>
   <ul><li><p>Cualquier paquete Workfront y un paquete Planning</p></li>
   <li><p>Cualquier flujo de trabajo y un paquete de Planning Prime y Ultimate</p></li></ul>

<p>Para acceder a los tipos de registros globales:</p>
   <ul><li><p>Cualquier paquete Workfront y un paquete Planning Plus</p></li>
   <li><p>Cualquier paquete de flujo de trabajo y un paquete de Planning Prime y Ultimate</p></li></ul> </td></tr>

<tr>
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td>
   <td>
   <p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p>
   <p><b>IMPORTANTE</b></p>
   <p>Solo los usuarios agregados al sistema Adobe Identity Management (IMS) pueden obtener permisos y agregarse a los campos de Planning.</p>
   <p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <ul><li><p>Cualquiera, para ver información de Workfront Planning</p></li>
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
   <li><p>Ver o permisos superiores a espacios de trabajo, tipos de registros y vistas que no se han creado para acceder a ellos y a sus objetos.</p></li>
   <li><p>Conceder permisos de contribución o superiores a espacios de trabajo y tipos de registros que no haya creado para editarlos y crear, editar o eliminar tipos de registros y registros.</p></li>
   <li><p>Permisos de contribución o superiores para vistas que no haya creado, para editarlas, eliminarlas y compartirlas</p>
   </li>
    <li><p>Los administradores del sistema pueden administrar los espacios de trabajo que no hayan creado. </p></li>
    <li><p>Los administradores del sistema no pueden acceder a las vistas que no han creado. </p></li></ul>
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
   <li>Panel izquierdo de proyectos, portafolios y programas</li>
   </ul>   
</td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Uso compartido del área de Planning mediante una plantilla de diseño

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

Los usuarios estándar y los administradores del sistema tienen habilitadas las áreas de Planning de forma predeterminada en las siguientes áreas:

* Menú principal
* Panel izquierdo de proyectos, portafolios o programas

El administrador del sistema debe agregarle las áreas de Planning si tiene cualquier otra licencia de Workfront y necesita contribuir al trabajo de Workfront Planning.

El administrador puede añadir la opción de planificación a las siguientes áreas modificando y asignándole una plantilla de diseño:

* Menú principal
* Landing page
* Panel izquierdo para proyectos, portafolios y programas
* Fijadores

Para agregar o quitar áreas de Workfront Planning de los usuarios de la instancia de Workfront:

1. Inicie sesión en **Workfront** como administrador.

1. Vaya a **Menú principal** > **Configuración** > **Interfaz** > **Plantillas de diseño** y abra o cree una plantilla de diseño.

   Para obtener información acerca de cómo personalizar una plantilla de diseño, vea [Crear y administrar plantillas de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Asigne la plantilla de diseño a los usuarios a los que desea tener acceso en Workfront Planning.

   Para obtener más información, consulte [Asignar usuarios a una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Todos los usuarios asignados a la plantilla pueden ahora acceder a Workfront Planning en su menú principal.

   Los usuarios pueden empezar a crear espacios de trabajo, tipos de registros, registros y campos.

## Asignar licencias a usuarios

Puede asignar licencias a los usuarios al configurar su nivel de acceso mientras los edita o crea.

Para obtener más información, consulte [Editar los perfiles de un usuario](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)

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

El tipo de licencia de Adobe Workfront funciona con los permisos de Workfront Planning para proporcionarle acceso para ver, contribuir o administrar objetos de Workfront Planning.

Para obtener información acerca de cómo afectan los tipos de licencia a los niveles de permisos de los objetos de Workfront Planning, consulte [Descripción general del tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


