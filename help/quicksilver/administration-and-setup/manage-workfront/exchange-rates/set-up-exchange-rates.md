---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Configurar tasas de cambio
description: Como administrador de Adobe Workfront, puede configurar tipos de cambio de divisa en Workfront.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 2%

---

# Configuración de tipos de cambio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador de Adobe Workfront, puede configurar tipos de cambio de divisa en Workfront. Esto incluye lo siguiente:

* Configuración de la moneda predeterminada para el sistema de Workfront
* Actualizar las tasas de cambio en Workfront para que coincidan con las tasas de cambio actuales
* Configuración de las tasas de cambio para varias monedas (al hacerlo, los usuarios pueden elegir una moneda predeterminada para proyectos individuales)

Los tipos de cambio afectan a todos los elementos financieros de Workfront. La Moneda base es la moneda predeterminada para todos los proyectos del sistema, a menos que se anule para un proyecto o rol determinado. También puede seleccionar mostrar información financiera en monedas disponibles en el sistema que sean diferentes a la moneda base o a la del proyecto cuando las visualice en un informe o lista. Para obtener más información, consulte [Crear informes de datos financieros con tasas de cambio únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Para obtener más información sobre la anulación de la divisa base en Workfront para proyectos y funciones de puesto, consulte los siguientes artículos:

* [Cambiar la divisa del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

La forma en que se configuran los tipos de cambio afecta a la posibilidad de que los usuarios modifiquen los tipos de cambio de un proyecto determinado.

>[!IMPORTANT]
>
>Las tasas de cambio en Workfront no son dinámicas; el valor que configure debe actualizarse cuando se produzcan cambios en las tasas de cambio.

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
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuración de tipos de cambio

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Tasas de cambio.**

1. Haga clic en **Agregar moneda.**
1. Empiece a escribir el nombre de la moneda y, a continuación, haga clic en ella cuando aparezca en la lista desplegable.

1. En el campo proporcionado, especifique la tasa para la moneda seleccionada, en relación con la moneda configurada como moneda base en el sistema.
1. (Opcional) Establezca la moneda como la moneda base (predeterminada) para Workfront.

   Esta es la moneda que se usa como predeterminada para todos los proyectos e informes de todo el sistema.

1. Haga clic en **Guardar** para guardar los cambios.

## Permitir que los usuarios modifiquen la moneda predeterminada de un proyecto

Los usuarios pueden modificar la moneda predeterminada de un proyecto cuando se cumplen las siguientes condiciones:

* El usuario tiene una licencia de planificación con acceso administrativo a las tasas de cambio.

  Para obtener más información, consulte [Conceder a los usuarios acceso administrativo a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Hay más de una divisa habilitada en el sistema de Workfront.

Para obtener información sobre cómo los usuarios pueden cambiar la moneda predeterminada en un proyecto determinado, vea [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permitir que los usuarios modifiquen la moneda predeterminada de un rol

Los usuarios pueden modificar la moneda de un rol cuando se cumplan las siguientes condiciones:

* El usuario tiene una licencia de planificación con acceso administrativo a las funciones del puesto.

  Para obtener más información, consulte [Conceder a los usuarios acceso administrativo a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Hay más de una divisa habilitada en el sistema de Workfront.

Para obtener información sobre cómo los usuarios pueden cambiar la moneda predeterminada en un rol determinado, consulte [Crear y administrar roles](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
