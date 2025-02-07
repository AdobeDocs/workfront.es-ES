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
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 97%

---

# Habilitar trimestres personalizados para proyectos

<!--Audited: 11/2024-->

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
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar trimestres personalizados para su sistema [!DNL Workfront]

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Project Preferences]** > **[!UICONTROL Projects].**

1. En la sección **[!UICONTROL Timelines]**, seleccione **[!UICONTROL Enable Custom Quarters]**.

1. Escriba un nombre para el trimestre personalizado, como “Primer trimestre fiscal de 2021”.
1. Seleccione las fechas de inicio y finalización del trimestre personalizado.

   ![Trimestres personalizados](assets/custom-quarters-nwe.png)

1. (Opcional) Haga clic en **[!UICONTROL Add Custom Quarter]** para añadir trimestres personalizados adicionales al sistema.
1. (Opcional) Cree un elemento de creación de informes que haga referencia a los trimestres fiscales.

   **Ejemplo:** cree un filtro para una lista de [!UICONTROL project] e incluya la fecha planificada de finalización de un proyecto que haga referencia a los trimestres personalizados.

   ![Filtro de proyecto con trimestres personalizados](assets/example-of-project-filter-with-custom-quarters.png)

   Las referencias a “Este trimestre”, “Próximo trimestre” y “Último trimestre” se sustituyen por nuevas referencias a los trimestres personalizados.

   Para obtener información acerca de los elementos de informes, consulte [Elementos de creación de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Para obtener información acerca de cómo crear filtros, consulte [Crear o editar filtros en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
