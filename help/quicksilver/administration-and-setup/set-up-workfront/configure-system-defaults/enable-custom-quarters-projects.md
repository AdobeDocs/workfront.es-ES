---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Habilitar trimestres personalizados para proyectos
description: Con fines de creación de informes, es posible que desee crear trimestres personalizados si los trimestres de su organización se basan en criterios específicos distintos de las fechas del calendario (como días laborables o días de compras).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Habilitar trimestres personalizados para proyectos

Con fines de creación de informes, es posible que desee crear trimestres personalizados si los trimestres de su organización se basan en criterios específicos distintos de las fechas del calendario (como días laborables o días de compras).

Puede configurar hasta ocho trimestres personalizados para su sistema [!DNL Adobe Workfront].

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Debe ser administrador de [!DNL Workfront].</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Configurar trimestres personalizados para su sistema [!DNL Workfront]

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Proyectos].**

1. En la sección **[!UICONTROL Líneas de tiempo]**, seleccione **[!UICONTROL Habilitar trimestres personalizados]**.

1. Escriba un nombre para el trimestre personalizado, como &quot;Primer trimestre fiscal de 2021&quot;.
1. Seleccione las fechas de inicio y finalización del trimestre personalizado.

   ![](assets/custom-quarters-nwe.png)

1. (Opcional) Haga clic en **[!UICONTROL Agregar trimestre personalizado]** para agregar trimestres personalizados adicionales al sistema.
1. (Opcional) Cree un elemento de informe que haga referencia a los trimestres fiscales.

   **Ejemplo:** Cree un filtro para una lista de [!UICONTROL proyecto] e incluya la fecha planificada de finalización de un proyecto que haga referencia a los trimestres personalizados.

   ![](assets/example-of-project-filter-with-custom-quarters.png)

   Las referencias a &quot;Este trimestre&quot;, &quot;Próximo trimestre&quot; y &quot;Último trimestre&quot; se sustituyen por nuevas referencias a los trimestres personalizados.

   Para obtener información acerca de los elementos de informes, vea [Elementos de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Para obtener información acerca de cómo crear filtros, vea [Crear o editar filtros en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
