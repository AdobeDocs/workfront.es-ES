---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Configurar tasas de cambio
description: Los tipos de cambio afectan a todos los elementos financieros de Workfront. La moneda de base es la moneda predeterminada para todos los proyectos del sistema.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc820b4012fec494ce5ebb1baefb4ee0df214916
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 56%

---

# Configuración de tipos de cambio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador de Adobe Workfront, puede configurar tipos de cambio de divisa en Workfront. Esto incluye lo siguiente:

* Configuración de la moneda predeterminada para el sistema de Workfront
* Actualizar las tasas de cambio en Workfront para que coincidan con las tasas de cambio actuales
* Configuración de las tasas de cambio para varias monedas (al hacerlo, los usuarios pueden elegir una moneda predeterminada para proyectos individuales)

Los tipos de cambio afectan a todos los elementos financieros de Workfront. La moneda de base es la moneda predeterminada para todos los proyectos del sistema, a menos que se anule para un proyecto o rol determinado. La base actual o la moneda predeterminada se indica con un icono ![Icono de moneda predeterminado](assets/default-icon.png) en la lista. También puede seleccionar mostrar información financiera en monedas disponibles en el sistema que sean diferentes a la moneda base o a la del proyecto cuando las visualice en un informe o lista. Para obtener más información, consulte [Crear informes de datos financieros con tasas de cambio únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Para obtener más información sobre la anulación de la divisa de base en Workfront para proyectos y funciones de puesto, consulte los siguientes artículos:

* [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md)
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
   <td role="rowheader">Plan de Adobe Workfront</td> 
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
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configuración de tipos de cambio

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Tasas de cambio**.

1. Haga clic en **Agregar moneda**.
1. En el cuadro **Agregar moneda**, empiece a escribir el nombre de la moneda y, a continuación, haga clic en ella cuando aparezca en la lista desplegable.
1. En el campo **Tasa de cambio**, escriba la tasa de la moneda seleccionada, en comparación con la moneda establecida como moneda base en el sistema.
1. Haga clic en **Agregar** para agregar la nueva moneda y su tipo de cambio.
1. (Opcional) Para cambiar la divisa base (predeterminada), realice una de las siguientes acciones:

   * Seleccione la casilla de verificación situada junto al nombre de la moneda y seleccione **Establecer como predeterminado** en la barra de acciones de la parte inferior de la pantalla.
   * Pase el ratón sobre el nombre de la moneda y haga clic en el menú **Más** que aparece. A continuación, seleccione **Establecer como predeterminado**.

     La nueva moneda predeterminada se actualiza con el icono.

     >[!NOTE]
     >
     >La moneda predeterminada siempre aparece primero en la lista, independientemente de cómo esté ordenada.

1. (Opcional) Para eliminar una moneda, seleccione la casilla de verificación situada junto al nombre de la moneda y seleccione **Eliminar** en la barra de acciones de la parte inferior de la pantalla. No puede eliminar la moneda predeterminada.

## Permitir que los usuarios modifiquen la moneda predeterminada de un proyecto

Los usuarios pueden modificar la moneda predeterminada de un proyecto cuando se cumplen las siguientes condiciones:

* El usuario tiene una licencia estándar o de planificación con acceso administrativo a las tasas de cambio.

  Para obtener más información, consulte [Conceder a los usuarios acceso administrativo a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Hay más de una moneda habilitada en el sistema de Workfront.

Para obtener información sobre cómo los usuarios pueden cambiar la moneda predeterminada en un proyecto determinado, vea [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permitir que los usuarios modifiquen la moneda predeterminada de una función

Los usuarios pueden modificar la moneda de una función cuando se cumplan las siguientes condiciones:

* El usuario tiene una licencia estándar o de planificación con acceso administrativo a las funciones del puesto.

  Para obtener más información, consulte [Conceder a los usuarios acceso administrativo a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Hay más de una divisa habilitada en el sistema de Workfront.

Para obtener información sobre cómo los usuarios pueden cambiar la moneda predeterminada en un rol determinado, consulte [Crear y administrar funciones](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).


<!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->
