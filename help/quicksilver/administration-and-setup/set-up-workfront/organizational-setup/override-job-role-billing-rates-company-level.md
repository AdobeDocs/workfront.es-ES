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
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 96%

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
   <td><p>Cualquiera</p></td> 
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
1. Haga clic en **[!UICONTROL Añadir tarifa de facturación] > [!UICONTROL Nueva tarifa de facturación]** o bien elija una tarifa existente para editar.
1. En el cuadro de diálogo [!UICONTROL Nueva tarifa de facturación], seleccione una [!UICONTROL **Función**] para definir la tarifa de facturación.

   La [!UICONTROL **tarifa de facturación predeterminada**] muestra la tarifa en el nivel del sistema para esta función.

   ![Nuevo cuadro de diálogo de tarifa de facturación](assets/date-effective-billing-rates-for-company.png)

1. En el campo [!DNL **Tarifas de facturación 1**], introduzca la tarifa de facturación. A continuación, haga clic en [!UICONTROL **Guardar**] para anular la tarifa de facturación una vez.

   O

   Haga clic en [!UICONTROL **Añadir tarifa**] para añadir más tarifas de facturación con fechas de entrada en vigor.

1. (Condicional) Si añade más de una tarifa de facturación, introduzca la siguiente información:

   * **[!UICONTROL Tarifas de facturación 1], 2, etc.**: el valor de la tarifa de facturación durante el período de tiempo.
   * **[!UICONTROL Fecha de inicio]**: fecha en la que la tarifa entra en vigor.
   * **[!UICONTROL Fecha de finalización]**: fecha en la que finaliza la tarifa.

     La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización. Algunas fechas se añaden automáticamente. Por ejemplo, si la tarifa de facturación 1 no tiene una fecha de finalización y añade la tarifa de facturación 2 con una fecha de inicio del 1 de mayo de 2023, se añade la fecha de finalización del 30 de abril de 2023 a la tarifa de facturación 1 para que no existan lagunas.

1. Haga clic en [!UICONTROL **Guardar**].

   >[!NOTE]
   >
   >Las tarifas de funciones cambiadas en el proyecto solo afectarán a ese proyecto. Las tarifas cambiadas a nivel de compañía afectarán a todos los proyectos. Para obtener más información, consulte [Información general sobre cómo anular las tarifas de facturación de funciones y calcular los ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
