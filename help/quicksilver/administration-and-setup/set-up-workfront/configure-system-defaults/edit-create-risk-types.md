---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Editar y crear tipos de riesgo
description: Puede añadir riesgos a un proyecto en la fase de planificación para identificar posibles obstáculos antes de la aprobación de cualquier trabajo. Los riesgos son posibles eventos que podrían impedir la finalización del proyecto a tiempo o dentro del presupuesto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: a8d2447eea4ca8d814035d183f40921cad49a0d8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 37%

---

# Editar y crear tipos de riesgo

<!--Audited: 03/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Adobe Workfront tiene una serie de tipos de riesgo predeterminados que puede asociar con proyectos en la fase de planificación para identificar posibles obstáculos antes de la aprobación de cualquier trabajo.

Los riesgos son posibles eventos que podrían impedir la finalización del proyecto a tiempo o dentro del presupuesto.

Además de los tipos de riesgo predeterminados, puede agregar nuevos tipos de riesgo para reflejar las necesidades de su organización.

Puede asociar tipos de riesgos con riesgos de proyecto para identificar el tipo de riesgo que podría presentar un proyecto.

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
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
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

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de riesgos

Los tipos de riesgo son etiquetas que puede utilizar para clasificar los riesgos con fines de creación de informes.

Como administrador de [!DNL Workfront], puede crear [!UICONTROL tipos de riesgos] en el área de [!UICONTROL **Configuración**].

Después de configurar los tipos de riesgo, son universales para su sistema.

Todos los propietarios de proyecto pueden utilizar los mismos tipos de riesgo para sus proyectos.

## Editar y crear tipos de riesgo

Algunos tipos de riesgos ya están en [!DNL Workfront], de manera predeterminada.


Puede hacer lo siguiente para mejorar el número de tipos de riesgo en la instancia de Workfront:

* [Editar tipos de riesgo existentes](#edit-existing-risk-types)
* [Crear tipos de riesgos](#create-risk-types)

### Editar tipos de riesgo existentes {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Tipos de riesgo]**.
1. Seleccione el tipo de riesgo que desea editar.
1. Haga clic en el icono **[!UICONTROL Editar]** ![Editar icono](assets/edit-icon.png).

   <span class="preview">Se abre el cuadro [!UICONTROL **Editar tipo de riesgo**].</span>

   ![Editar cuadro de tipo de riesgo](assets/edit-risk-type-box.png)

   >[!TIP]
   >
   >   Puede editar la información de tipo de riesgo en línea, al hacer doble clic en el Nombre o la Descripción de un tipo de riesgo en una lista de tipos de riesgo.

1. (Opcional) Cambie el nombre y la descripción del tipo de riesgo.

   Hay un límite de 50 caracteres para los campos **[!UICONTROL Nombre]** y **[!UICONTROL Descripción]**.

1. Haga clic en **[!UICONTROL Guardar cambios].**

1. (Opcional) Para eliminar un tipo de riesgo, selecciónelo en la lista, haga clic en el icono [!UICONTROL **Eliminar**] ![Eliminar icono](assets/delete.png) y, a continuación, en [!UICONTROL **Sí, eliminarlo**]. El tipo de riesgo se elimina y no se puede recuperar.

1. (Opcional) Para exportar una lista de tipos de riesgos, haga clic en el icono [!UICONTROL **Exportar**] ![Icono Exportar](assets/export-icon.png). Puede exportar a los siguientes tipos de archivo:

   * PDF
   * Excel
   * Excel (xlsx)
   * Delimitado por tabulaciones

   >[!TIP]
   >
   >   Primero puede seleccionar un número limitado de tipos de riesgo y luego exportarlos para una lista más pequeña.


### Crear tipos de riesgos {#create-risk-types}

Puede crear tipos de riesgo, además de los predeterminados.

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Tipos de riesgo]**.

1. Haga clic en **[!UICONTROL Nuevo tipo de riesgo]** para abrir el cuadro [!UICONTROL **Nuevo tipo de riesgo**]

   O

   Haga clic en [!UICONTROL **Agregar más tipos de riesgos**] en la esquina inferior izquierda de la lista de tipos de riesgos para agregar tipos de riesgos en línea.

   <span class="preview">Se abre el cuadro **Nuevo tipo de riesgo**. <span>

   ![Nuevo cuadro de tipo de riesgo](assets/new-risk-type-box.png)


1. Agregue un **[!UICONTROL Nombre]** (obligatorio) y una **[!UICONTROL Descripción]** (opcional) para el tipo de riesgo.

   Hay un límite de 50 caracteres para los campos **[!UICONTROL Nombre]** y **[!UICONTROL Descripción]**.

1. Haga clic en **[!UICONTROL Crear tipo de riesgo]**,

   O bien, si usó la edición en línea para agregar su tipo de riesgo, haga clic en **[!UICONTROL Introducir]** cuando haya terminado.

   >[!TIP]
   >
   >Para editar un tipo de riesgo personalizado, consulte la sección [[!UICONTROL Editar los tipos de riesgo existentes]](#edit-existing-risk-types) en este artículo.

## Adjuntar riesgos con tipos de riesgo en proyectos

Puede utilizar tipos de riesgos para etiquetar los riesgos agregados a sus proyectos.

Para obtener más información sobre cómo añadir riesgos a los proyectos, consulte [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
