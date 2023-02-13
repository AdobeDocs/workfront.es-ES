---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Anular las tasas de facturación de funciones de trabajo a nivel de empresa
description: Cuando se crea una función de trabajo, tiene la opción de seleccionar una tasa de facturación por hora para esa función. Puede crear una tasa de facturación por hora específica de una empresa.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Anular las tasas de facturación de funciones de trabajo a nivel de empresa

Cuando se crea una función de trabajo, tiene la opción de seleccionar una tasa de facturación por hora para esa función. Puede crear una tasa de facturación por hora específica de una empresa.

A nivel de proyecto, puede activar una opción para permitir que las tasas de facturación a nivel de empresa anulen las tasas a nivel de proyecto. Para obtener más información, consulte [Anular tasas de facturación a nivel de proyecto con tasas de facturación a nivel de empresa](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

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
   <td> <p>Acceso administrativo a las empresas si no es administrador del sistema</p> <p>Acceso de [!UICONTROL Edit] a datos financieros</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Anular o cambiar una tasa de facturación establecida utilizada para una función de trabajo específica

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Compañías]**.
1. Busque la empresa a la que se asigna la función de trabajo.
1. Haga clic en **[!UICONTROL Editar empresa]** en la esquina superior derecha.
1. En el **[!UICONTROL Tasas de facturación]** , seleccione la función de trabajo que desea editar e introduzca la nueva tasa de facturación para esa función de trabajo en la **[!UICONTROL Tasa de facturación de la empresa]** en la ventana

   >[!NOTE]
   >
   >Las tasas de función de trabajo cambiadas en el proyecto solo afectarán a ese proyecto. Las tasas cambiadas a nivel de empresa afectarán a todos los proyectos. Para obtener más información, consulte [Información general sobre la anulación de la función de trabajo Tasas de facturación y el cálculo de ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
