---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Activar trimestres personalizados
description: Con fines de creación de informes, es posible que desee crear trimestres personalizados si los trimestres de su organización se basan en criterios específicos distintos de las fechas del calendario (como días laborables o días de compras).
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 56%

---

# Habilitar trimestres personalizados

<!--Audited: 11/2024-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes que han comprado [!DNL Adobe Workfront Planning]. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Con fines de creación de informes, es posible que desee crear trimestres personalizados si los trimestres de su organización se basan en criterios específicos distintos de las fechas del calendario (como días laborables o días de compras).

<div class="preview">

Según los productos que haya adquirido su compañía, puede configurar el siguiente número de trimestres en el área Configuración de Workfront:

* Los clientes que solo compraron [!DNL Workfront], pueden configurar hasta ocho trimestres personalizados para el sistema [!DNL Adobe Workfront].
* Los clientes que compraron [!DNL Workfront] y [!DNL Workfront Planning], pueden configurar hasta 100 trimestres para el sistema [!DNL Workfront], que también están disponibles en [!DNL Planning].

</div>

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

   >[!IMPORTANT]
   >
   > <span class="preview">Si su empresa compró [!DNL Workfront Planning], no puede guardar sus trimestres personalizados si hay espacios o superposiciones entre los trimestres. </span>
   ><span class="preview">![Trimestres personalizados con advertencia de superposición](assets/custom-quarters-with-overlap-warning.png)</span>
   >Solo se permiten espacios y superposiciones entre los trimestres para [!DNL Workfront] clientes.

1. (Opcional y condicional) Si su empresa compró solo [!DNL Workfront], sin [!DNL Workfront Planning], cree un elemento de informe que haga referencia a los trimestres fiscales.


   **Ejemplo:** cree un filtro para una lista de [!UICONTROL project] e incluya la fecha planificada de finalización de un proyecto que haga referencia a los trimestres personalizados.

   ![Filtro de proyecto con trimestres personalizados](assets/example-of-project-filter-with-custom-quarters.png)

   Las referencias a “Este trimestre”, “Próximo trimestre” y “Último trimestre” se sustituyen por nuevas referencias a los trimestres personalizados.

   Para obtener información acerca de los elementos de informes, consulte [Elementos de creación de informes: filtros, vistas y agrupaciones](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   Para obtener información acerca de cómo crear filtros, consulte [Crear o editar filtros en [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
1. <span class="preview"> (opcional y condicional) Si tiene acceso a [!DNL Workfront Planning], vaya a una página de tipo de registro y abra una vista de escala de tiempo. La vista muestra los nuevos trimestres personalizados. </span>
