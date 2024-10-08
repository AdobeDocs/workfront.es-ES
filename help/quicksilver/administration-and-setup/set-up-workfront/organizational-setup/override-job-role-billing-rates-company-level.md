---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Anular las tarifas de facturación del rol en el nivel de compañía
description: Cuando se crea un rol, tiene la opción de seleccionar una tarifa de facturación por hora para ese rol. Puede crear una tarifa de facturación por hora específica de una compañía.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 1%

---

# Anular las tarifas de facturación de funciones en el nivel de compañía

Cuando se crea un rol, tiene la opción de seleccionar una tarifa de facturación por hora para ese rol. Puede crear varias tarifas de facturación por hora específicas de una compañía. Cada tarifa de facturación entra en vigor para un intervalo de fechas específico.

En el nivel de proyecto, puede habilitar una opción para permitir que las tarifas de facturación en la empresa anulen las tarifas en el nivel de proyecto. Para obtener más información, consulte [Anular tarifas de facturación de nivel de proyecto con tarifas de facturación de nivel de compañía](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>
   <p>Nuevo: [!UICONTROL Standard]</p>
   <p>O</p>
   <p>Actual: [!UICONTROL plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a Compañías si no es administrador del sistema</p>
   <p>Editar acceso a datos financieros</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anular o cambiar una tarifa de facturación establecida utilizada para un rol específico

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Compañías]**.
1. Busque la empresa donde se asigna el rol.
1. Haga clic en el nombre de la empresa en la lista.
1. Haga clic en **[!UICONTROL Tarifas de facturación]** en el panel izquierdo.
1. Haga clic en **[!UICONTROL Agregar tarifa de facturación] > [!UICONTROL Nueva tarifa de facturación]**, o bien elija una tarifa existente para editar.
1. En el cuadro de diálogo [!UICONTROL Nueva tarifa de facturación], seleccione un [!UICONTROL **Rol**] para definir la tarifa de facturación.

   La [!UICONTROL **tarifa de facturación predeterminada**] muestra la tarifa a nivel del sistema para este rol.

   ![Cuadro de diálogo Nueva tarifa de facturación](assets/date-effective-billing-rates-for-company.png)

1. En el campo [!DNL **Tarifas de facturación 1**], introduzca la tarifa de facturación. A continuación, haga clic en [!UICONTROL **Guardar**] para anular la tarifa de facturación una vez.

   O

   Haz clic en [!UICONTROL **Agregar tarifa**] para agregar más tarifas de facturación con fechas de vigencia.

1. (Condicional) Si agrega más de una tarifa de facturación, ingrese la siguiente información:

   * **[!UICONTROL Tarifas de facturación 1], 2, etc.**: el valor de la tarifa de facturación durante el período de tiempo.
   * **[!UICONTROL Fecha de inicio]**: La fecha en que la tarifa entra en vigencia.
   * **[!UICONTROL Fecha de finalización]**: La fecha en la que finaliza la tarifa.

     La tarifa de facturación 1 no tendrá una fecha de inicio y la última tarifa de facturación no tendrá una fecha de finalización. Algunas fechas se añaden automáticamente. Por ejemplo, si la Tarifa de facturación 1 no tiene una fecha de finalización y agrega la Tarifa de facturación 2 con una fecha de inicio del 1 de mayo de 2023, se agrega la fecha de finalización del 30 de abril de 2023 a la Tarifa de facturación 1 para que no existan lagunas.

1. Haga clic en [!UICONTROL **Guardar**].

   >[!NOTE]
   >
   >Las tasas de rol cambiadas en el proyecto solo afectarán a ese proyecto. Las tarifas cambiadas a nivel de compañía afectarán a todos los proyectos. Para obtener más información, consulte [Información general sobre cómo anular las tarifas de facturación del rol y calcular los ingresos en un proyecto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).
