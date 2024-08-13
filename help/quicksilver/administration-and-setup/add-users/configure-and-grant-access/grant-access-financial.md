---
title: Concesión de acceso a los datos financieros
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede definir el acceso de un usuario a los datos financieros en Workfront a través de su nivel de acceso.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bf4a37ee-9435-4c1c-b18c-a7338a548ab7
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 0%

---

# Concesión de acceso a los datos financieros

{{highlighted-preview}}

Como administrador de Adobe Workfront, puede definir el acceso de un usuario a lo siguiente a través del nivel de acceso del usuario, como se explica en [Información general sobre los niveles de acceso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md):

* Información financiera sobre proyectos en Workfront
* Información de presupuestación de recursos en las herramientas de planificación de recursos

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

## Consideraciones para conceder acceso a los datos financieros

Tenga en cuenta lo siguiente al conceder a los usuarios acceso a los datos financieros en Workfront:

* Un usuario cuyo nivel de acceso no permite el acceso a los datos financieros no puede crear un riesgo para un proyecto. Para obtener más información, vea [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
* También puede utilizar un nivel de acceso para determinar qué actividades de Administración de recursos puede utilizar un usuario para presupuestar o ver la asignación de recursos. Para obtener más información, consulte [Conceder acceso a Administración de recursos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Configuración del acceso de los usuarios a los datos financieros mediante un nivel de acceso personalizado

1. Comience a crear o editar el nivel de acceso, tal como se explica en [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en el botón **Ver** o **Editar** que se encuentra a la derecha de Datos financieros y, a continuación, seleccione las facultades que desea conceder en **Ajustar la configuración**.

   ![](assets/financial-data-fine-tune-nwe.png)

1. (Opcional) En el área **Permitir acceso administrativo para**, seleccione las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipos de cambio</td> 
      <td> <p>Añada una nueva moneda en Workfront.</p> <p>Sin este acceso, el usuario solo puede agregar una moneda existente a un proyecto que cree.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gastos</td> 
      <td> <p>Vea todos los gastos en objetos en Workfront.</p> <p>Esto no permite al usuario crear nuevos tipos de gastos.</p> <p>Sin este acceso, el usuario solo puede ver lo siguiente:</p> 
       <ul> 
        <li>Gastos en proyectos, tareas o problemas que administran</li> 
        <li>Sus propios gastos</li> 
        <li>Los gastos de sus subordinados</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Para establecer la configuración de acceso para otros objetos y áreas en el nivel de acceso en el que está trabajando, continúe con uno de los artículos enumerados en [Configurar el acceso a Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acceso a tareas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).
1. Cuando termine, haga clic en **Guardar**.

   Una vez creado el nivel de acceso, puede asignarlo a un usuario. Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acceso a información financiera compartida

Puede compartir información financiera sobre un proyecto, tarea o problema con otros usuarios otorgándoles permisos para ello, como se explica en [Compartir permisos financieros en un objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Cuando comparte cualquier objeto con otro usuario, los derechos del destinatario sobre él se determinan mediante una combinación de dos cosas:

* Los permisos que concede al destinatario para el objeto
* Configuración del nivel de acceso del destinatario para el tipo de objeto

## Acceso a la información financiera por tipo de licencia

Para obtener información acerca de lo que los usuarios de cada nivel de acceso pueden hacer con la información financiera, vea la sección [Datos financieros](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#financia) en el artículo [Funcionalidad disponible para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acceso a la información financiera mediante la configuración

La siguiente información puede ayudarle a comprender cómo utilizar la configuración del nivel de acceso para controlar el acceso de los usuarios a los datos financieros.

### Sin acceso

Un usuario sin acceso a datos financieros no tiene acceso a lo siguiente:

* Sección Finanzas bajo Objetos de proyecto y tarea
* Caso comercial
* Tarifas de facturación y registros de facturación
* <span class="preview">Tarjetas de tarifa</span>
* Coste por hora y facturación por hora según las preferencias del usuario

  Puede configurarlo con el icono de engranaje ![](assets/gear-icon-settings.png) en el botón Ver del paso 4 anterior.

* Coste por hora y facturación por hora en Funciones del puesto

  Puede configurarlo con el icono de engranaje ![](assets/gear-icon-settings.png) en el botón Ver del paso 4 anterior.

### Ver acceso

Un usuario con acceso de visualización de datos financieros puede ver (no editar) lo siguiente:

* Sección Finanzas bajo Objetos de proyecto y tarea
* Caso comercial
* Tarifas de facturación y registros de facturación
* Coste por hora y facturación por hora según las preferencias del usuario

  Puede configurarlo con el icono de engranaje ![](assets/gear-icon-settings.png) en el botón Ver del paso 4 anterior.

* Coste por hora y facturación por hora en Funciones del puesto

  Puede configurarlo con el icono de engranaje ![](assets/gear-icon-settings.png) en el botón Ver del paso 4 anterior.

### Editar acceso

Un usuario con acceso de edición de datos financieros puede ver y editar lo siguiente:

* Sección Finanzas bajo Objetos de proyecto y tarea
* Caso comercial
* Tarifas de facturación y registros de facturación
* <span class="preview">Tarjetas de tarifa</span>
* Coste por hora y facturación por hora según las preferencias del usuario

  Puede configurarlo con el icono de engranaje ![](assets/gear-icon-settings.png) en el botón Editar del paso 4 anterior.

* Coste por hora y facturación por hora en Funciones del puesto

  Puede configurarlo con el icono de engranaje ![](assets/gear-icon-settings.png) en el botón Editar del paso 4 anterior.
