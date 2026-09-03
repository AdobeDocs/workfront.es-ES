---
product-area: projects
navigation-topic: financials
title: Anular las tarifas de facturación a nivel de proyecto con las tarifas de facturación a nivel de compañía
description: Anular las tarifas de facturación a nivel de proyecto con las tarifas de facturación a nivel de compañía
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
TQID: https://experienceleague.adobe.com/GQSQGGHBZsBLtI8IEUltVXzxmEtOxue0iE6fpHmYWP4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 8c08e110aeccdf6d6416fd1070fbcbd40fd46983
workflow-type: tm+mt
source-wordcount: 480
ht-degree: 57%

---

# Anular las tarifas de facturación a nivel de proyecto con las tarifas de facturación a nivel de compañía

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Puede configurar un proyecto para que utilice tarifas de facturación a nivel de compañía en lugar de tarifas de facturación a nivel de proyecto.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso de edición a proyectos y datos financieros</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Administre permisos para el proyecto con permisos para Editar tarifas de facturación y Finanzas generales</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Active la opción de anulación Tarifas de facturación a nivel de compañía

Si una empresa está relacionada con un proyecto y esta opción está activada, los cambios hechos en las tarifas de facturación en la empresa anulan las tarifas establecidas en el proyecto.

Cuando un usuario recalcula manualmente las finanzas del proyecto, se aplican todos los cambios realizados en las tarifas de facturación a nivel de compañía. Los cálculos de ingresos históricos también se anulan, a menos que estén marcados como facturados.

1. Vaya a un proyecto.
1. Haga clic en el menú **Más** ![Menú más](assets/qs-more-icon-on-an-object.png) junto al nombre del proyecto en el encabezado y, a continuación, haga clic en **Editar**.
1. En la sección **Finanzas**, seleccione **Permitir que las tarifas de facturación a nivel de compañía anulen las tarifas a nivel de proyecto**.

   >[!CAUTION]
   >
   >Al habilitar esta opción se anulan los cálculos de ingresos históricos a menos que estén marcados como facturados. Puede conservar los cálculos de ingresos históricos creando un registro de facturación. Para obtener más información, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md).

1. Haga clic en **Guardar**.

## Actualizar las tarifas de facturación a nivel de compañía y aplicarlas a un proyecto

Después de habilitar la opción de anulación de tarifas de facturación a nivel de compañía en un proyecto, los cambios realizados en las tarifas de facturación de la compañía se aplican al proyecto cada vez que se recalculan las finanzas.

>[!NOTE]
>
>Los usuarios deben tener acceso a Compañías en su nivel de acceso para actualizar las tarifas de facturación a nivel de compañía.

{{step-1-to-setup}}

1. Haga clic en **Compañías**.
1. Haga clic en el nombre de la empresa asociada al proyecto para el que activó la anulación de tarifas de facturación en la empresa.
1. Haga clic en **Tarifas de facturación** en el panel de la izquierda.
1. Seleccione la tasa de rol que desea actualizar y haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png).

   Actualice la tarifa de facturación y las fechas en vigencia según sea necesario y haga clic en **Guardar**. Para obtener más información sobre las tarifas de facturación de la compañía con fecha efectiva, consulte [Anular tarifas de facturación de funciones a nivel de compañía](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Para actualizar las tarifas de la compañía de uno o más proyectos, realice una de las siguientes acciones:

   * Varios proyectos:

     1. Ir a una lista de proyectos.
     1. Active las casillas de verificación de los proyectos que desee actualizar.
     1. Haga clic en el menú **Más** ![Menú más](assets/qs-more-icon-on-an-object.png) en la parte superior de la lista y, a continuación, haga clic en **Recalcular finanzas**.

   * Un solo proyecto:

     1. Vaya al proyecto para el que ha habilitado la opción de anulación de las tarifas de facturación a nivel de compañía.
     1. Haga clic en el menú **Más** ![Menú más](assets/qs-more-icon-on-an-object.png) junto al nombre del proyecto en el encabezado y, a continuación, haga clic en **Volver a calcular finanzas**.

     Para obtener más información sobre cómo recalcular las finanzas de uno o más proyectos, vea [Recalcular finanzas de proyectos](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

