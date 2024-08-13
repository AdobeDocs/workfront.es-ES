---
title: Conceder acceso a los problemas
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los problemas de Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3c15f90f-ce87-484d-93a7-9eeb2963a798
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Conceder acceso a los problemas

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los problemas, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Conceder acceso al usuario a los problemas mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** que se encuentra a la derecha de Problemas y, a continuación, seleccione las facultades que desea conceder en **Ajustar la configuración**.

1. (Opcional) Para restringir permisos heredados para problemas de objetos de clasificación superior, haga clic en **Establecer restricciones adicionales** y, a continuación, seleccione **No heredar nunca acceso a documentos de proyectos, tareas, problemas, etc**.

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a las emisiones por tipo de licencia

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los problemas, vea la sección [Problemas](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#issues) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a problemas compartidos

Como propietario o creador de un problema, puede compartirlo con otros usuarios otorgándoles permisos, tal como se explica en [Compartir un problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

<!--
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
-->

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario sobre él se determinan mediante una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* Configuración del nivel de acceso del destinatario para el tipo de objeto

Además, si su nivel de acceso lo permite, los usuarios pueden obtener acceso a un problema a través de la jerarquía de objetos: si un usuario ya tiene permiso para trabajar en el proyecto o la tarea principal de un problema, también tiene permiso para hacerlo (consulte el paso 3 anterior). Cuando comparte un problema, puede ver una lista de los usuarios que le han heredado el permiso.

![](assets/inherited-permissions.png)
