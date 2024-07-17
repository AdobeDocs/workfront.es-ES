---
product-area: projects
navigation-topic: financials
title: Anular Tarifas de facturación a nivel de proyecto con Tarifas de facturación a nivel de compañía
description: Anular Tarifas de facturación a nivel de proyecto con Tarifas de facturación a nivel de compañía
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 72511f98e05c160e2ca69def8aa3a929ed62bb40
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---

# Anular Tarifas de facturación a nivel de proyecto con Tarifas de facturación a nivel de compañía

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Puede configurar un proyecto para que utilice tarifas de facturación en la empresa en lugar de tarifas en el proyecto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y datos financieros</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Active la opción de anulación Tarifas de facturación a nivel de compañía

Si una empresa está relacionada con un proyecto y esta opción está habilitada, los cambios hechos en las tarifas de facturación en la empresa anulan las tarifas establecidas en el proyecto.

Cuando un usuario recalcula manualmente las finanzas en el proyecto, se aplican todos los cambios en las tarifas de facturación en la empresa. Los cálculos de ingresos históricos también se anulan, a menos que se marquen como facturados.

1. Vaya a un proyecto.
1. Haga clic en el menú **Más** ![](assets/qs-more-icon-on-an-object.png) junto al nombre del proyecto en el encabezado y, a continuación, haga clic en **Editar**.
1. En la sección **Finanzas**, habilite **Permitir que las tarifas de facturación en la compañía anulen las tarifas en el nivel de proyecto**.

   >[!CAUTION]
   >
   >Al habilitar esta opción, se anulan los cálculos de ingresos históricos a menos que se marquen como facturados. Puede conservar los cálculos de ingresos históricos creando un registro de facturación. Para obtener más información, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Haga clic en **Guardar cambios**.

## Actualizar las tarifas de facturación a nivel de compañía y aplicarlas a un proyecto

Después de habilitar la opción de anulación de tarifas de facturación en la empresa en un proyecto, los cambios realizados en las tarifas de facturación de la empresa se aplican al proyecto cada vez que se recalculan las finanzas.

>[!NOTE]
>
>Los usuarios deben tener acceso a Compañías en su nivel de acceso para actualizar las tarifas de facturación en el nivel de compañía.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar**.
1. Haga clic en **Compañías**.
1. Haga clic en el nombre de la empresa asociada al proyecto para el que habilitó la anulación de tarifas de facturación en la empresa.
1. Haga clic en **Tarifas de facturación** en el panel izquierdo.
1. Actualice la **tarifa de facturación de la compañía** y las fechas de inicio/finalización de un rol existente y, a continuación, presione Entrar.

   Para agregar una nueva tarifa de facturación de empresa con fecha efectiva, selecciona una tarifa de facturación para el rol y haz clic en **Editar**. Para obtener más información sobre las tarifas de facturación efectiva de la compañía por fecha, consulte [Anular las tarifas de facturación de rol a nivel de compañía](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Para actualizar las tarifas de compañía de uno o más proyectos, realice una de las siguientes acciones:

   * Varios proyectos:

      1. Ir a una lista de proyectos.
      1. Seleccione la casilla de verificación en línea con los proyectos que desee actualizar.
      1. Haga clic en **Editar**.
      1. En la sección Configuración, habilite la opción **Recalcular costos e ingresos**.
      1. Haga clic en **Guardar cambios**.

   * Proyecto único:

      1. Vaya al proyecto para el que habilitó la anulación de tarifas de facturación en la empresa.
      1. Haga clic en el menú **Más** ![](assets/qs-more-icon-on-an-object.png) junto al nombre del proyecto en el encabezado y, a continuación, haga clic en **Volver a calcular finanzas**.
