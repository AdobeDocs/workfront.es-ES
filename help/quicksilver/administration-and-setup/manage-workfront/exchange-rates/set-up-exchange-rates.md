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
TQID: https://experienceleague.adobe.com/7D54XR0cFqGEbzYzRh9dWHVEKj0xZLR-GYLIe5-0NMo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 839
ht-degree: 41%

---

# Configuración de tipos de cambio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador de Adobe Workfront, puede configurar tipos de cambio de divisa en Workfront. Esto incluye lo siguiente:

* Configuración de la moneda predeterminada para el sistema de Workfront
* Actualizar las tasas de cambio en Workfront para que coincidan con las tasas de cambio actuales
* Configuración de las tasas de cambio para varias monedas (al hacerlo, los usuarios pueden elegir una moneda predeterminada para proyectos individuales)

Los tipos de cambio afectan a todos los elementos financieros de Workfront. La moneda de base es la moneda predeterminada para todos los proyectos e informes del sistema, a menos que se anule para un proyecto o rol determinado. La base actual o la moneda predeterminada se indica con un icono ![Icono de moneda predeterminado](assets/default-icon.png) en la lista. También puede seleccionar mostrar información financiera en monedas disponibles en el sistema que sean diferentes a la moneda base o a la del proyecto cuando las visualice en un informe o lista. Para obtener más información, consulte [Crear informes de datos financieros con tasas de cambio únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Para obtener más información sobre la anulación de la divisa de base en Workfront para proyectos y funciones de puesto, consulte los siguientes artículos:

* [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Crear y administrar funciones de trabajo](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

La forma en que se configuran los tipos de cambio afecta a la posibilidad de que los usuarios modifiquen los tipos de cambio de un proyecto determinado.

>[!IMPORTANT]
>
>Las tasas de cambio en Workfront no son dinámicas; el valor que configure debe actualizarse cuando se produzcan cambios en las tasas de cambio.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Para configurar tasas de cambio: Cualquier paquete de flujo de trabajo o Workfront</p>
       <p>Para aplicar fechas en vigor a los tipos de cambio: Paquete Ultimate de flujo de trabajo</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

     La nueva moneda predeterminada se actualiza con el icono ![Icono de moneda predeterminado](assets/default-icon.png).

     >[!NOTE]
     >
     >La moneda predeterminada siempre aparece primero en la lista, independientemente de cómo esté ordenada.

1. (Opcional) Para eliminar una moneda, seleccione la casilla de verificación situada junto al nombre de la moneda y seleccione **Eliminar** en la barra de acciones de la parte inferior de la pantalla. No puede eliminar la moneda predeterminada.

## Establecer fechas en vigor para los tipos de cambio de una divisa

Las fechas en vigor para los tipos de cambio de una divisa se configuran de modo que un valor de tipo de cambio termine en una fecha específica y comience otra tasa. El tipo de cambio de la fecha correcta se utiliza en los cálculos financieros.

{{step-1-to-setup}}

1. Haga clic en **Preferencias del proyecto** > **Tasas de cambio**.
1. Seleccione una moneda de la lista y haga clic en **Administrar fechas** en la barra de acciones.
1. En el cuadro de diálogo **(nombre de moneda) tipos de cambio efectivos**, elija una **Fecha de finalización** para el tipo de cambio actual.

   O

   Elija una **fecha de inicio** para la nueva tasa de cambio.

   El primer tipo de cambio no tendrá fecha de inicio y el último tipo no tendrá fecha de finalización. Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tasa no tiene una fecha de finalización y agrega una tasa de cambio con una fecha de inicio del 1 de diciembre de 2025, se agrega una fecha de finalización del 30 de noviembre de 2025 a la primera tasa para que no existan huecos.

   ![Cuadro de diálogo de tipos de cambio efectivos por fecha](assets/euro-date-effective-rates.png)

1. Escriba el nuevo valor **Exchange rate**.
1. (Opcional) Haga clic en **Agregar fecha efectiva** para agregar más tasas de cambio con fechas efectivas para esta moneda.
1. Haga clic en **Guardar**.

## Permitir que los usuarios modifiquen la moneda predeterminada de un proyecto

Los usuarios pueden modificar la moneda predeterminada de un proyecto cuando se cumplen las siguientes condiciones:

* El usuario tiene una licencia Standard o Plan con acceso administrativo a las tasas de cambio.

  Para obtener más información, consulte [Conceder a los usuarios acceso administrativo a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Hay más de una moneda habilitada en el sistema de Workfront.

Para obtener información sobre cómo los usuarios pueden cambiar la moneda predeterminada en un proyecto determinado, vea [Cambiar la moneda del proyecto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permitir que los usuarios modifiquen la moneda predeterminada de una función

Los usuarios pueden modificar la moneda de una función cuando se cumplan las siguientes condiciones:

* El usuario tiene una licencia estándar o de planificación con acceso administrativo a las funciones del puesto.

  Para obtener más información, consulte [Conceder a los usuarios acceso administrativo a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Hay más de una divisa habilitada en el sistema de Workfront.

Para obtener información sobre cómo los usuarios pueden cambiar la moneda predeterminada en un rol determinado, consulte [Crear y administrar funciones](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).



