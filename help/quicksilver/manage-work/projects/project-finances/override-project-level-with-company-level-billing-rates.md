---
product-area: projects
navigation-topic: financials
title: Anular las tarifas de facturación a nivel de proyecto con las tarifas de facturación a nivel de compañía
description: Anular las tarifas de facturación a nivel de proyecto con las tarifas de facturación a nivel de compañía
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 100%

---

# Anular las tarifas de facturación a nivel de proyecto con las tarifas de facturación a nivel de compañía

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Puede configurar un proyecto para que utilice tarifas de facturación a nivel de compañía en lugar de tarifas de facturación a nivel de proyecto.

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Acceso de edición a proyectos y datos financieros</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td>Permisos de administración para el proyecto con permisos para administrar finanzas</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Habilitar la opción de anulación de tarifas de facturación a nivel de compañía

Si una compañía está asociada con un proyecto y esta opción está habilitada, los cambios realizados en las tarifas de facturación a nivel de compañía anulan las tarifas de facturación establecidas en el proyecto.

Cuando un usuario recalcula manualmente las finanzas del proyecto, se aplican todos los cambios realizados en las tarifas de facturación a nivel de compañía. Los cálculos de ingresos históricos también se anulan, a menos que estén marcados como facturados.

1. Vaya a un proyecto. 
1. Haga clic en el menú **Más** ![](assets/qs-more-icon-on-an-object.png) junto al nombre del proyecto visible en el encabezado y, a continuación, haga clic en **Editar**.
1. En la sección **Finanzas**, habilite **Permitir que las tarifas de facturación a nivel de compañía anulen las tarifas de facturación a nivel de proyecto**.

   >[!CAUTION]
   >
   >Al habilitar esta opción se anulan los cálculos de ingresos históricos a menos que estén marcados como facturados. Puede conservar los cálculos de ingresos históricos creando un registro de facturación. Para obtener más información, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

1. Haga clic en **Guardar cambios**.

## Actualizar las tarifas de facturación a nivel de compañía y aplicarlas a un proyecto

Después de habilitar la opción de anulación de tarifas de facturación a nivel de compañía en un proyecto, los cambios realizados en las tarifas de facturación de la compañía se aplican al proyecto cada vez que se recalculan las finanzas.

>[!NOTE]
>
>Los usuarios deben tener acceso a Compañías en su nivel de acceso para actualizar las tarifas de facturación a nivel de compañía.

{{step-1-to-setup}}

1. Haga clic en **Compañías**.
1. Haga clic en el nombre de la compañía asociada al proyecto para el que habilitó la anulación de tarifas de facturación a nivel de compañía.
1. Haga clic en **Tarifas de facturación** en el panel de la izquierda.
1. Actualice la **Tarifa de facturación de la compañía** y las fechas de inicio/finalización de una función existente y, a continuación, presione Intro.

   Para añadir una nueva tarifa de facturación de la compañía con fecha efectiva, seleccione una tarifa de facturación de funciones y haga clic en **Editar**. Para obtener más información sobre las tarifas de facturación de la compañía con fecha efectiva, consulte [Anular tarifas de facturación de funciones a nivel de compañía](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Para actualizar las tarifas de la compañía de uno o más proyectos, realice una de las siguientes acciones:

   * Varios proyectos:

      1. Ir a una lista de proyectos.
      1. Seleccione la casilla de verificación en línea con los proyectos que desee actualizar.
      1. Haga clic en **Editar**.
      1. En la sección Configuración, habilite la opción **Recalcular costes e ingresos**.
      1. Haga clic en **Guardar cambios**.

   * Un solo proyecto:

      1. Vaya al proyecto para el que ha habilitado la opción de anulación de las tarifas de facturación a nivel de compañía.
      1. Haga clic en el menú **Más** ![](assets/qs-more-icon-on-an-object.png) junto al nombre del proyecto visible en el encabezado y, a continuación, haga clic en **Recalcular finanzas**.
