---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Habilitar trimestres personalizados para proyectos
description: Para generar informes, es posible que desee crear trimestres personalizados si los trimestres de su organización se basan en criterios específicos que no sean fechas del calendario (como días laborables o días de compras).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Habilitar trimestres personalizados para proyectos

Para generar informes, es posible que desee crear trimestres personalizados si los trimestres de su organización se basan en criterios específicos que no sean fechas del calendario (como días laborables o días de compras).

Puede configurar hasta ocho trimestres personalizados para su [!DNL Adobe Workfront] sistema.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure los trimestres personalizados para su [!DNL Workfront] sistema

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Proyectos].**

1. En el **[!UICONTROL Líneas de tiempo]** , seleccione **[!UICONTROL Habilitar trimestres personalizados]**.

1. Escriba un nombre para el trimestre personalizado, como &quot;Fiscal T1 2021&quot;.
1. Seleccione las fechas de inicio y finalización del trimestre personalizado.

   ![](assets/custom-quarters-nwe.png)

1. (Opcional) Haga clic en **[!UICONTROL Agregar trimestre personalizado]** para agregar trimestres personalizados adicionales al sistema.
1. (Opcional) Cree un elemento de informe que haga referencia a los trimestres fiscales.

   **Ejemplo:** Cree un filtro para un [!UICONTROL proyecto] e incluya la fecha de finalización prevista de un proyecto que haga referencia a los trimestres personalizados.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   Las referencias a &quot;Este trimestre&quot;, &quot;Siguiente trimestre&quot; y &quot;Último trimestre&quot; se sustituyen por nuevas referencias a los trimestres personalizados.

   Para obtener información sobre los elementos de informes, consulte [Elementos de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Para obtener información sobre la creación de filtros, consulte [Crear o editar filtros en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
