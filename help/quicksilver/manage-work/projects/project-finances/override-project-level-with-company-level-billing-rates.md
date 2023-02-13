---
product-area: projects
navigation-topic: financials
title: Anular tasas de facturación a nivel de proyecto con tasas de facturación a nivel de empresa
description: Anular tasas de facturación a nivel de proyecto con tasas de facturación a nivel de empresa
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Anular tasas de facturación a nivel de proyecto con tasas de facturación a nivel de empresa

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Puede configurar un proyecto para que utilice tasas de facturación a nivel de empresa en lugar de tasas de facturación a nivel de proyecto.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y Datos Financieros</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos para el proyecto con permisos para Administrar finanzas</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Habilitar la opción de anulación de las tasas de facturación a nivel de empresa

Cuando una empresa está asociada a un proyecto y esta opción está habilitada, los cambios realizados en las tasas de facturación a nivel de empresa anulan la tasa de facturación establecida en el proyecto.

Cuando un usuario vuelve a calcular manualmente las finanzas del proyecto, se aplica cualquier cambio en las tasas de facturación a nivel de empresa. Los cálculos de ingresos históricos también se anulan a menos que se marquen como facturados.

1. Vaya a un proyecto.
1. Haga clic en el **Más** menú ![](assets/qs-more-icon-on-an-object.png) junto al nombre del proyecto en el encabezado y, a continuación, haga clic en **Editar**.
1. En el **Finanzas** , habilite **Permitir que las tasas de facturación a nivel de empresa anulen las tasas de facturación a nivel de proyecto**.

   >[!CAUTION]
   >
   >Al habilitar esta opción, se anulan los cálculos de ingresos históricos a menos que se marquen como facturados. Puede conservar los cálculos de ingresos históricos creando un registro de facturación. Para obtener más información, consulte el artículo [Crear registros de facturación](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Haga clic en **Guardar cambios**.

## Actualizar las tasas de facturación a nivel de empresa y aplicarlas a un proyecto

Después de habilitar la opción de anulación de las tasas de facturación a nivel de empresa en un proyecto, los cambios realizados en las tasas de facturación de la empresa se aplican al proyecto cada vez que se vuelven a calcular las finanzas.

>[!NOTE]
>
>Los usuarios deben tener acceso a las empresas en su nivel de acceso para actualizar las tasas de facturación a nivel de empresa.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración**.
1. Haga clic en **Compañías**.
1. Haga clic en el nombre de la empresa asociada al proyecto para el que ha habilitado la anulación de las tasas de facturación a nivel de empresa.
1. Haga clic en **Tasas de facturación** en el panel izquierdo.
1. Introduzca la nueva tasa de facturación para una función de trabajo existente en la **Tasa de facturación de la empresa** y, a continuación, pulse Intro.
1. Para actualizar las tasas de compañía de uno o varios proyectos, realice una de las siguientes acciones:

   * Varios proyectos:
   1. Vaya a una lista de proyectos.
   1. Seleccione la casilla de verificación en línea con los proyectos que desee actualizar.
   1. Haga clic en **Editar**.
   1. En la sección Configuración , habilite la opción **Volver A Calcular Los Costes Y Los Ingresos** .
   1. Haga clic en **Guardar cambios**.
   * Proyecto único:

      1. Vaya al proyecto para el que ha habilitado la anulación de las tasas de facturación a nivel de empresa.
      1. Haga clic en el **Más** menú ![](assets/qs-more-icon-on-an-object.png) junto al nombre del proyecto en el encabezado y, a continuación, haga clic en **Volver a calcular finanzas**.
