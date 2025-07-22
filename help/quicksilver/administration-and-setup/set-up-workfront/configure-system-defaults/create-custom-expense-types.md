---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear tipos de gastos personalizados
description: Como administrador, puede crear tipos de gastos personalizados para definir y realizar un seguimiento de los gastos asociados con sus tareas y proyectos.  [!DNL Adobe Workfront]  Los gastos son costos no laborales que pueden asociarse con tareas o proyectos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 7f95df7acfb1afd0974c0138152a68326631d265
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 18%

---

# Crear tipos de gastos personalizados

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador de [!DNL Adobe Workfront], puede crear tipos de gastos personalizados para definir y realizar un seguimiento de los gastos asociados con sus tareas y proyectos. Los gastos son costos no laborales que pueden asociarse con tareas o proyectos.

Puede editar o eliminar cualquier tipo de gasto que cree. No puede eliminar ni editar los tipos de gastos integrados de [!DNL Workfront].

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

## Tipos de gastos predeterminados

Los tipos de gastos predeterminados en [!DNL Workfront] que no se pueden eliminar ni editar incluyen los siguientes:

* [!UICONTROL Advertising]
* [!UICONTROL Consultoría]
* [!UICONTROL Entretenimiento]
* [!UICONTROL General]
* [!UICONTROL Materiales]
* [!UICONTROL Viaje]

## Crear tipos de gastos personalizados

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Tipos de gastos]**.
1. Haga clic en **[!UICONTROL Nuevo tipo de gasto]**.
1. En el cuadro de diálogo **[!UICONTROL Nuevo tipo de gasto]**, escriba la siguiente información:

   * **Nombre** - Un nombre para el gasto.
   * **Descripción** - Una descripción del gasto.
   * **Unidad calculada**: seleccione la unidad de medida del tipo de gasto en la lista desplegable. Están disponibles las siguientes unidades de medida:

      * Milla
      * Kilómetro
      * Kilogramo
      * Dólar
      * Hora
      * Día
      * Otros: al seleccionar esta opción, se le pedirá que asigne un nombre a la unidad de medida y que defina la unidad de medida como algo familiar para su organización.

   * **Tarifa** - El precio por unidad. Este es un campo con formato de moneda y representa el costo de cada unidad establecida en el campo **Unidad calculada**. La tasa puede contener un valor numérico con hasta 4 números después del decimal. Por ejemplo, 1,0375.

1. Haga clic en **[!UICONTROL Guardar]**.

   El tipo de gasto ya está disponible para que los usuarios lo asocien con sus gastos en proyectos y tareas.

## Modificar tipos de gastos personalizados

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Tipos de gastos]**.
1. Seleccione el tipo de gasto que desea modificar y luego haga clic en el icono **[!UICONTROL Editar]** ![Editar icono](assets/edit-icon.png).

   Aparece el cuadro de diálogo **[!UICONTROL Editar tipo de gasto]**.

1. Realice los cambios que desee y haga clic en **[!UICONTROL Guardar]**.

   El tipo de gasto ya está disponible para que los usuarios lo asocien con sus gastos en proyectos y tareas.

Para obtener más información sobre cómo usar gastos y cómo pueden afectar al costo de un proyecto, vea el artículo [Administrar gastos de proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).
