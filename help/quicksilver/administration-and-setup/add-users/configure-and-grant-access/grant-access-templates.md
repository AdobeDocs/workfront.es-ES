---
title: Conceder acceso a las plantillas
user-type: administrator
product-area: system-administration;templates
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a las plantillas de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c8e6af1b-8cf3-4522-b0eb-7e5f2d34f5a9
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Concesión de acceso a las plantillas

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a las plantillas, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Solo los usuarios con una licencia de planificación pueden tener acceso completo a las plantillas.

Para obtener información acerca del uso de niveles de acceso personalizados para administrar el acceso de los usuarios a otros tipos de objetos en Workfront, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configuración del acceso de los usuarios a las plantillas mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** que se encuentra a la derecha de Plantillas y, a continuación, seleccione las facultades que desea conceder en **Ajustar la configuración**.

   ![](assets/access-level-to-templates-with-edit-expanded-1.png)

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a plantillas por tipo de licencia

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con las plantillas, vea la sección [Plantillas](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#template) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a plantillas compartidas

Como propietario o creador de un problema, puede compartirlo con otros usuarios otorgándoles permisos, tal como se explica en [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario sobre él se determinan mediante una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* Configuración del nivel de acceso del destinatario para el tipo de objeto
