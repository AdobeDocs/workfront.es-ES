---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Como administrador de Adobe Workfront, puede configurar los tipos de cambio en Workfront.
description: Configurar tipos de cambio
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Configurar tipos de cambio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador de Adobe Workfront, puede configurar los tipos de cambio en Workfront. Esto incluye lo siguiente:

* Configuración de la moneda predeterminada para el sistema Workfront
* Actualización de los tipos de cambio en Workfront para que coincidan con los tipos de cambio actuales
* Configuración de los tipos de cambio para múltiples monedas (esto permite a los usuarios elegir una moneda predeterminada para proyectos individuales)

Los tipos de cambio afectan a todos los elementos financieros de Workfront. La moneda base es la moneda predeterminada para todos los proyectos del sistema, a menos que se sobrescriba para un proyecto o función de trabajo determinados. También puede seleccionar mostrar la información financiera en monedas disponibles en su sistema que sean diferentes a la moneda base o a la del proyecto cuando las vea en un informe o lista. Para obtener más información, consulte [Crear informes de datos financieros con tipos de cambio únicos](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Para obtener más información sobre la anulación de la moneda base en Workfront para proyectos y funciones de trabajo, consulte los siguientes artículos:

* [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

La forma en que se configuran los tipos de cambio afecta a si los usuarios pueden modificar los tipos de cambio de un proyecto determinado.

>[!IMPORTANT]
>
>Los tipos de cambio en Workfront no son dinámicos; el valor que haya establecido debe actualizarse cuando se produzcan cambios en los tipos de cambio.

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
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar tipos de cambio

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Preferencias de proyecto** > **Tipos de Cambio.**

1. Haga clic en **Agregar moneda.**
1. Empiece a escribir el nombre de la moneda y, a continuación, haga clic en él cuando aparezca en la lista desplegable.

1. En el campo proporcionado, especifique la tasa para la moneda seleccionada, ya que está relacionada con la moneda que se ha establecido como moneda base en el sistema.
1. (Opcional) Defina la moneda como la moneda base (predeterminada) para Workfront.

   Esta es la moneda que se usa de forma predeterminada para todos los proyectos e informes del sistema.

1. Haga clic en **Guardar** para guardar los cambios.

## Permitir que los usuarios modifiquen la moneda predeterminada de un proyecto

Los usuarios pueden modificar la moneda predeterminada de un proyecto cuando se cumplan las siguientes condiciones:

* El usuario tiene una licencia Plan con acceso administrativo a las tasas de cambio.

   Para obtener más información, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Se habilita más de una moneda en el sistema Workfront.

Para obtener información sobre cómo los usuarios pueden cambiar la moneda predeterminada en un proyecto determinado, consulte [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permitir que los usuarios modifiquen la moneda predeterminada para una función de trabajo

Los usuarios pueden modificar la moneda de una función de trabajo cuando se cumplen las siguientes condiciones:

* El usuario tiene una licencia Plan con acceso administrativo a Funciones de Trabajo.

   Para obtener más información, consulte [Conceder a los usuarios acceso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Se habilita más de una moneda en el sistema Workfront.

Para obtener información sobre cómo los usuarios pueden cambiar la moneda predeterminada en una función de trabajo determinada, consulte [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
