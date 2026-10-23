---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Anular las tarifas de facturación del rol en el nivel de compañía
description: Cuando se crea una función, tiene la opción de seleccionar una tarifa de facturación por hora para dicha función. Puede crear una tarifa de facturación por hora específica de una compañía.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
TQID: 'https://experienceleague.adobe.com/EbnybXqWehstH2ziLqNZfMHtarMvUiugvWioYv9wLds'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a41c8c19f14058571c027da1dc49041b060e4b65
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 43%
---
# Anular tarifas de facturación de funciones a nivel de compañía

Cuando se crea una función, tiene la opción de seleccionar una tarifa de facturación por hora para dicha función. Puede crear varias tarifas de facturación por hora específicas de una compañía. Cada tarifa de facturación entra en vigor para un intervalo de fechas específico.

En el nivel de proyecto, puede habilitar una opción para permitir que las tarifas de facturación en la empresa anulen las tarifas en el nivel de proyecto. Para obtener más información, consulte [Anular tarifas de facturación de nivel de proyecto con tarifas de facturación de nivel de compañía](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Para agregar atributos de tarifa a las tarifas de facturación en la empresa: Flujo de trabajo Ultimate</p>
       <p>Para crear tarifas de facturación en la empresa y editar todas las demás configuraciones de tarifas: Cualquier paquete de Workfront o de flujo de trabajo</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a Compañías si no es administrador del sistema</p>
   <p>Editar acceso a datos financieros</p> </td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anulación o cambio de una tarifa de facturación establecida utilizada para una función específica

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Compañías]**.
1. Busque la empresa donde se asigna la función.
1. Haga clic en el nombre del usuario en la lista.
1. Haga clic en **[!UICONTROL Tarifas de facturación]** en el panel de la izquierda.
1. Haga clic en **[!UICONTROL Agregar tarifa de facturación]**.
1. En el cuadro de diálogo [!UICONTROL Nueva tarifa de facturación], seleccione una [!UICONTROL **Función**] para definir la tarifa de facturación.

1. Seleccione atributos para la tasa, como Agencia, Ubicación o Centro de Coste.

   Estos atributos se definen por separado y pueden afectar a los cálculos de ingresos y costes. Para obtener más información, vea [Definir atributos de tasa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

   ![Nuevo cuadro de diálogo de tarifa de facturación](assets/company-billing-rates-090326.png)

1. Seleccione **Divisa** para la tarifa. El administrador de Workfront añade la Moneda base en el área de Configuración. Puede cambiar la selección a otra divisa disponible y cambiar la divisa en intervalos de fechas en vigor.

   >[!TIP]
   >
   >En este campo sólo están disponibles las divisas disponibles en el área Tasas de cambio del sistema. Si solo tiene configurada una moneda, solo estará disponible esa moneda.

   Para obtener información sobre cómo configurar la divisa base en Workfront, consulte [Configurar tasas de cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Para obtener información acerca de cómo cambiar la moneda de un proyecto, vea [Cambiar la moneda del proyecto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. En el campo [!DNL **Tarifa de facturación**], introduzca la tarifa de facturación para el rol.

   tarifa de facturación por hora de la función del puesto. Este valor calcula los ingresos planificados y reales de las tareas y los problemas asociados a la función, y, en última instancia, los ingresos planificados y reales de los proyectos. Introduzca el tipo de cambio utilizando la divisa seleccionada.

   Si utiliza atributos, los atributos y la función se combinan para definir una tasa única. Por ejemplo, una función de Designer en Nueva York para la Agencia A puede tener una tasa separada de una función de Designer en París para la Agencia B.

   Para ver las tarifas de facturación vigentes por fecha, haga clic en **Agregar tarifa vigente por fecha**. Introduzca la tasa de facturación por hora para el período de tiempo y asigne una Fecha de inicio y una Fecha de finalización según sea necesario. La primera tarifa de facturación no tendrá fecha de inicio y la última tarifa de facturación no tendrá fecha de finalización.

   Workfront le permite dejar espacios entre intervalos de fechas, pero recibirá una advertencia para confirmar que esto es intencional.

   Para obtener información sobre cómo Workfront calcula los ingresos, consulte [Información general sobre facturación e ingresos](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Al editar una tarifa existente, puede ordenar la lista para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.

1. Haga clic en [!UICONTROL **Guardar**].

   >[!NOTE]
   >
   >Las tarifas de funciones cambiadas en el proyecto solo afectarán a ese proyecto. Las tarifas cambiadas a nivel de compañía afectarán a todos los proyectos que tengan la compañía asignada. Para obtener más información, consulte [Información general sobre cómo anular las tarifas de facturación y calcular los ingresos en un proyecto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).




<!--

   The [!UICONTROL **Default Billing Rate**] displays the system-level rate for this job role.

   ![New Billing Rate dialog](assets/date-effective-billing-rates-for-company.png)

1. In the [!DNL **Billing Rates 1**] field, enter the billing rate. Then, click [!UICONTROL **Save**] to override the billing rate one time.

   Or

   Click [!UICONTROL **Add Rate**] to add more billing rates with effective dates.

1. (Conditional) If you are adding more than one billing rate, enter the following information:

   * **[!UICONTROL Billing Rates 1], 2, etc.**: The value of the billing rate for the time period.
   * **[!UICONTROL Start Date]**: The date when the rate becomes effective.
   * **[!UICONTROL End Date]**: The date when the rate ends.

     Billing Rate 1 will not have a start date and the last billing rate will not have an end date. Some dates are added automatically. For example, if Billing Rate 1 does not have an end date, and you add Billing Rate 2 with a start date of May 1, 2023, an end date of April 30, 2023 is added to Billing Rate 1 so that no gaps exist.

1. Click [!UICONTROL **Save**].

   >[!NOTE]
   >
   >Job role rates changed on the project will only impact only that project. Rates changed at the company level will impact all projects. For more information, see [Overview of overriding billing rates and calculating revenue on a project](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

-->


