---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Crear tipos de gastos personalizados
description: Como [!DNL Adobe Workfront] administrador, puede crear tipos de gastos personalizados para definir y rastrear los gastos asociados con sus tareas y proyectos. Los gastos son costes no laborales que pueden asociarse con tareas o proyectos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# Crear tipos de gastos personalizados

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como [!DNL Adobe Workfront] administrador, puede crear tipos de gastos personalizados para definir y rastrear los gastos asociados con sus tareas y proyectos. Los gastos son costes no laborales que pueden asociarse con tareas o proyectos.

Puede editar o eliminar cualquier tipo de gasto que cree. No puede eliminar ni editar el complemento [!DNL Workfront] tipos de gastos.

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

## Tipos de Gastos Predeterminados

Los tipos de gastos que se encuentran en [!DNL Workfront] de forma predeterminada, no se puede eliminar ni editar, incluya lo siguiente:

* [!UICONTROL Publicidad]
* [!UICONTROL Asesoramiento]
* [!UICONTROL Entretenimiento]
* [!UICONTROL General]
* [!UICONTROL Materiales]
* [!UICONTROL Viaje]

## Crear tipos de gastos personalizados

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront].
1. Haga clic en **[!UICONTROL Tipos de Gastos]**.
1. Haga clic en **[!UICONTROL Nuevo tipo de gasto]**.
1. En el **[!UICONTROL Nuevo tipo de gasto]** que se muestra, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Especifique un nombre para el gasto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Especifique una descripción para el gasto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unidad calculada]</td> 
      <td> <p>Seleccione la unidad de medida para el tipo de gasto en la lista desplegable.</p> <p>Se dispone de la siguiente unidad de medida:</p> 
       <ul> 
        <li>Milla</li> 
        <li>Kilómetro</li> 
        <li>Kilogramo</li> 
        <li>Dólar</li> 
        <li>Dólar</li> 
        <li>días</li> 
        <li>Otro : al seleccionar esta opción, se le pedirá que asigne un nombre a la unidad de medida y que la defina como algo familiar para su organización.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tarifa</td> 
      <td> <p>Especifique el precio por unidad. Se trata de un campo con formato de moneda que representa el coste de cada unidad establecida en la variable <strong>[!UICONTROL Unidad calculada]</strong> campo . </p> <p>La tasa puede contener un valor numérico con hasta 4 números después del decimal. Por ejemplo, 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear tipo de gasto]**.\
   El tipo de gasto ya está disponible para que los usuarios lo asocien a sus gastos en proyectos y tareas.

## Modificar tipos de gastos personalizados

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront].
1. Haga clic en **[!UICONTROL Tipos de Gastos]**.
1. Seleccione el tipo de gasto que desea modificar y haga clic en **[!UICONTROL Editar]**.

   La variable **[!UICONTROL Editar tipo de gasto]** se muestra.

1. Realice los cambios que desee y haga clic en **[!UICONTROL Guardar cambios]**.\
   El tipo de gasto ya está disponible para que los usuarios lo asocien a sus gastos en proyectos y tareas.

Para obtener más información sobre cómo utilizar los gastos y cómo pueden afectar al coste de un proyecto, consulte el artículo [Administrar los gastos del proyecto](../../../manage-work/projects/project-finances/manage-project-expenses.md).
