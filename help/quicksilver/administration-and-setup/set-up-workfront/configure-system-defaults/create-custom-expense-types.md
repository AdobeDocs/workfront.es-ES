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
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

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
   <p>Actual: [!UICONTROL plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de gastos predeterminados

Los tipos de gastos que se encuentran en [!DNL Workfront] de manera predeterminada no se pueden eliminar ni editar; incluyen los siguientes:

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
1. En el cuadro **[!UICONTROL Nuevo tipo de gasto]** que se muestra, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre]</td> 
      <td>Especifique un nombre para el gasto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Especifique una descripción para el gasto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unidad calculada]</td> 
      <td> <p>Seleccione la unidad de medida del tipo de gasto en la lista desplegable.</p> <p>Están disponibles las siguientes unidades de medida:</p> 
       <ul> 
        <li>Milla</li> 
        <li>Kilómetro</li> 
        <li>Kilogramo</li> 
        <li>Dólar</li> 
        <li>Dólar</li> 
        <li>Día</li> 
        <li>Otros: al seleccionar esta opción, se le pedirá que asigne un nombre a la unidad de medida y que defina la unidad de medida como algo familiar para su organización.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tarifa</td> 
      <td> <p>Especifique el precio por unidad. Este es un campo con formato de moneda y representa el costo de cada unidad establecida en el campo <strong>[!UICONTROL Calculated Unit]</strong>. </p> <p>La tasa puede contener un valor numérico con hasta 4 números después del decimal. Por ejemplo, 1,0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear tipo de gasto]**.\
   El tipo de gasto ya está disponible para que los usuarios lo asocien con sus gastos en proyectos y tareas.

## Modificar tipos de gastos personalizados

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Tipos de gastos]**.
1. Seleccione el tipo de gasto que desea modificar y luego haga clic en **[!UICONTROL Editar]**.

   Se muestra el cuadro de diálogo **[!UICONTROL Editar tipo de gasto]**.

1. Realice los cambios que desee y luego haga clic en **[!UICONTROL Guardar cambios]**.\
   El tipo de gasto ya está disponible para que los usuarios lo asocien con sus gastos en proyectos y tareas.

Para obtener más información sobre cómo usar gastos y cómo pueden afectar al costo de un proyecto, vea el artículo [Administrar gastos de proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).
