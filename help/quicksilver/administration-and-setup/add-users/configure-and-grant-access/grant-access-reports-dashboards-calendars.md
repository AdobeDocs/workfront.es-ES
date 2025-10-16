---
title: Conceder acceso a informes, tableros y calendarios
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a informes, paneles y calendarios en Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 35%

---

# Conceder acceso a informes, tableros y calendarios

Como administrador de Adobe Workfront, puede utilizar un nivel de acceso para definir el acceso de un usuario a informes, tableros y calendarios, tal como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Este acceso también incluye el acceso a las páginas externas. Para obtener información sobre páginas externas, consulte [Conceder acceso a datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Si desea conceder a los usuarios acceso a informes, tableros y calendarios, también debe darles acceso a filtros, vistas y agrupaciones. Para obtener instrucciones, consulte [Conceder acceso a filtros, vistas y agrupaciones](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Cuando alguien comparte un informe, tablero o calendario con otro usuario, los derechos del destinatario están determinados por una combinación de dos cosas: La configuración del nivel de acceso del destinatario para informes, tableros y calendarios _y_ cualquier permiso que el usuario que comparte haya concedido para el informe, tablero o calendario
>
>Para obtener información sobre los permisos que los usuarios pueden conceder en un informe, panel o calendario al compartirlo, vea [Compartir informes, paneles y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure el acceso de los usuarios a los informes, paneles y calendarios mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** que se encuentra a la derecha de Informes y, a continuación, seleccione las capacidades que desea conceder en **Ajustar la configuración**.

   ![reports_access.png](assets/reports-access.png)

   Las siguientes opciones están habilitadas de forma predeterminada:

   * **Crear**
   * **Eliminar**
   * **Ver informes integrados**: Es necesario seleccionarlo para ver los informes creados por Workfront.
   * **Compartir**
   * **Compartir informes públicamente**: los informes se pueden compartir públicamente, compartiendo un vínculo público al informe con cualquier persona que no tenga una cuenta de Workfront. Esta opción debe estar seleccionada para permitir este nivel de uso compartido.
   * **Compartir en todo el sistema**: los informes se pueden compartir con todos los usuarios del sistema que tengan una licencia de Workfront. Esta opción debe estar seleccionada para permitir este nivel de uso compartido.

     Para obtener información sobre cómo compartir informes, tableros y calendarios, vea [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que esté trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a las tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) y [Conceder acceso a los datos financieros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a informes, paneles de control y calendarios por tipo de licencia

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con los problemas, vea la sección [Informes](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a informes, tableros y calendarios compartidos

Como propietario o creador de un informe, tablero o calendario, puede compartirlo con otros usuarios concediéndoles permisos, como se explica en [Compartir informes, tableros y calendarios](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario sobre él se determinan mediante una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* Configuración del nivel de acceso del destinatario para el tipo de objeto
