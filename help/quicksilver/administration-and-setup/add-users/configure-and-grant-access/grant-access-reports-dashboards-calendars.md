---
title: Conceder acceso a informes, tableros y calendarios
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los informes, tableros y calendarios en Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Conceder acceso a informes, tableros y calendarios

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a los informes, tableros y calendarios, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Este acceso también incluye el acceso a Páginas externas. Para obtener información sobre las páginas externas, consulte [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Si desea otorgar a los usuarios acceso a informes, tableros y calendarios, también debe darles acceso a filtros, vistas y agrupaciones. Para obtener instrucciones, consulte [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Cuando alguien comparte un informe, tablero o calendario con otro usuario, los derechos del destinatario se determinan mediante una combinación de dos cosas: La configuración de nivel de acceso del destinatario para informes, tableros y calendarios _y_ cualquier permiso que el usuario que comparte haya concedido para el informe, panel o calendario
>
>Para obtener información sobre los permisos que los usuarios pueden conceder en un informe, tablero o calendario al compartirlo, consulte [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

## Requisitos de acceso

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configuración del acceso de los usuarios a los informes, tableros y calendarios mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono del engranaje ![](assets/gear-icon-settings.png) en el **Ver** o **Editar** a la derecha de Informes y, a continuación, seleccione las capacidades que desee conceder en **Ajustar la configuración**.

   ![reports_access.png](assets/reports-access.png)

   Las siguientes opciones están habilitadas de forma predeterminada:

   * **Crear**
   * **Eliminar**
   * **Ver informes integrados**: Debe seleccionarse para ver los informes creados por Workfront.
   * **Compartir**
   * **Compartir informes públicamente**: Los informes se pueden compartir públicamente compartiendo un vínculo público al informe con cualquier persona que no tenga una cuenta de Workfront. Esta opción debe estar seleccionada para permitir este nivel de uso compartido.
   * **Compartir todo el sistema**: Los informes se pueden compartir con todas las personas del sistema que dispongan de una licencia de Workfront. Esta opción debe estar seleccionada para permitir este nivel de uso compartido.

      Para obtener información sobre cómo compartir informes, tableros y calendarios, consulte [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Opcional) Para configurar las opciones de acceso de otros objetos y áreas del nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configuración del acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Concesión de acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Concesión de acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando haya terminado, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a informes, tableros y calendarios por tipo de licencia

Para obtener información sobre lo que los usuarios de cada nivel de acceso pueden hacer con los problemas, consulte la sección [Informes](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a informes, tableros y calendarios compartidos

Como propietario o creador de un informe, tablero o calendario, puede compartirlo con otros usuarios concediéndoles permisos, tal como se explica en [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario están determinados por una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* La configuración del nivel de acceso del destinatario para el tipo del objeto
