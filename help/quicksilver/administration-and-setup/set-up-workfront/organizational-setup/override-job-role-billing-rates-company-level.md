---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Anular las tarifas de facturación de funciones en el nivel de compañía
description: Cuando se crea un rol, tiene la opción de seleccionar una tarifa de facturación por hora para ese rol. Puede crear una tarifa de facturación por hora específica de una compañía.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

---

# Anular las tarifas de facturación de funciones en el nivel de compañía

{{highlighted-preview}}

Cuando se crea un rol, tiene la opción de seleccionar una tarifa de facturación por hora para ese rol. <span class="preview">Puede crear varias tarifas de facturación por hora específicas de una compañía. Cada tarifa de facturación entra en vigor para un intervalo de fechas específico.</span>

En el nivel de proyecto, puede habilitar una opción para permitir que las tarifas de facturación en la empresa anulen las tarifas en el nivel de proyecto. Para obtener más información, consulte [Anular Tarifas de facturación a nivel de proyecto con Tarifas de facturación a nivel de compañía](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a Compañías si no es administrador del sistema</p> <p>Acceso de [!UICONTROL Edit] a datos financieros</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Anular o cambiar una tarifa de facturación establecida utilizada para un rol específico

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Compañías]**.
1. Busque la empresa donde se asigna el rol.
1. <span class="preview">Haga clic en el nombre de la empresa en la lista.</span>
1. <span class="preview">Clic **[!UICONTROL Tarifas de facturación]** en el panel izquierdo.</span>
1. <span class="preview">Clic **[!UICONTROL Agregar tarifa de facturación] > [!UICONTROL Nueva tarifa de facturación]**, o elija una tasa existente para editar.</span>
1. <span class="preview">En el [!UICONTROL Nueva tarifa de facturación] diálogo, seleccione una [!UICONTROL **Rol**] para definir la tasa de facturación de.</span>

   <span class="preview">El [!UICONTROL **Tarifa de facturación predeterminada**] muestra la tasa en el nivel del sistema para este rol.</span>

   <span class="preview">![Cuadro de diálogo Nueva tarifa de facturación](assets/date-effective-billing-rates-for-company.png)</span>

1. <span class="preview">En el [!DNL **Tarifas de facturación 1**] , introduzca la tarifa de facturación. A continuación, haga clic en [!UICONTROL **Guardar**] para anular la tarifa de facturación una vez.</span>

   <span class="preview">O</span>

   <span class="preview">Clic [!UICONTROL **Agregar tarifa**] para agregar más tarifas de facturación con fechas efectivas.</span>

1. <span class="preview">(Condicional) Si agrega más de una tarifa de facturación, ingrese la siguiente información:</span>

   * <span class="preview">**[!UICONTROL Tarifas de facturación 1], 2, etc.**: Valor de la tasa de facturación para el período de tiempo.</span>
   * <span class="preview">**[!UICONTROL Fecha de inicio ]**: La fecha en la que la tasa entra en vigor.</span>
   * <span class="preview">**[!UICONTROL Fecha de finalización ]**: La fecha en la que finaliza la tarifa.</span>

     <span class="preview">La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización. Algunas fechas se añaden automáticamente. Por ejemplo, si la Tarifa de facturación 1 no tiene una fecha de finalización y agrega la Tarifa de facturación 2 con una fecha de inicio del 1 de mayo de 2023, se agrega la fecha de finalización del 30 de abril de 2023 a la Tarifa de facturación 1 para que no existan lagunas.</span>

1. <span class="preview">Haga clic en [!UICONTROL **Guardar**].</span>

   >[!NOTE]
   >
   >Las tasas de rol cambiadas en el proyecto solo afectarán a ese proyecto. Las tarifas cambiadas a nivel de compañía afectarán a todos los proyectos. Para obtener más información, consulte [Resumen de anulación de Tarifas de facturación de rol y cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
