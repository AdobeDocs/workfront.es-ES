---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Editar y crear tipos de riesgos
description: Puede añadir riesgos a un proyecto en la fase de planificación para identificar posibles obstáculos antes de la aprobación de cualquier trabajo. Los riesgos son posibles eventos que podrían impedir la finalización del proyecto a tiempo o dentro del presupuesto.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 2%

---

# Editar y crear tipos de riesgo

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Puede añadir riesgos a un proyecto en la fase de planificación para identificar posibles obstáculos antes de la aprobación de cualquier trabajo. Los riesgos son posibles eventos que podrían impedir la finalización del proyecto a tiempo o dentro del presupuesto.

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

## Tipos de riesgos

Los tipos de riesgo son etiquetas que puede utilizar para clasificar los riesgos con fines de creación de informes. El administrador [!DNL Adobe Workfront] los crea en el área **[!UICONTROL Setup]**. Una vez establecidos los tipos de riesgos en el área **[!UICONTROL Configuración]**, son universales para el sistema. Todos los propietarios de proyecto pueden utilizar los mismos tipos de riesgo para sus proyectos.

## Editar y crear tipos de riesgo

Algunos tipos de riesgos ya están en [!DNL Workfront], de manera predeterminada. Para reflejar las necesidades de su organización, puede editar los tipos de riesgo existentes o crear nuevos tipos de riesgo.

* [Editar tipos de riesgos existentes](#edit-existing-risk-types)
* [Crear nuevos tipos de riesgos](#create-new-risk-types)

### Editar tipos de riesgos existentes {#edit-existing-risk-types}

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Tipos de riesgos]**.
1. Seleccione el tipo de riesgo que desea editar.
1. Haga clic en **[!UICONTROL Editar]**.
1. (Opcional) Cambie el nombre y la descripción del tipo de riesgo.

   Hay un límite de 50 caracteres para los campos **[!UICONTROL Nombre]** y **[!UICONTROL Descripción]**.

1. Haga clic en **[!UICONTROL Guardar cambios].**

### Crear nuevos tipos de riesgos {#create-new-risk-types}

Puede crear nuevos tipos de riesgo, además de los predeterminados, para reflejar las necesidades de su organización.

Para crear un nuevo tipo de riesgo:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Tipos de riesgos]**.
1. Haga clic en **[!UICONTROL Nuevo tipo de riesgo]**.
1. Escriba un **[!UICONTROL Nombre]** (obligatorio) y una **[!UICONTROL Descripción]** (opcional) para el tipo de riesgo.

   Hay un límite de 50 caracteres para los campos **[!UICONTROL Nombre]** y **[!UICONTROL Descripción]**.

1. Haga clic en **[!UICONTROL Crear tipo de riesgo]**. Si usó la edición en línea para agregar su tipo de riesgo, haga clic en **[!UICONTROL Introducir]** cuando haya terminado.

   >[!NOTE]
   >
   >Si necesita editar un tipo de riesgo personalizado, consulte la sección [[!UICONTROL Editar los tipos de riesgo existentes]](#edit-existing-risk-types) en este artículo.

## Adjuntar riesgos con tipos de riesgos en proyectos

Los tipos de riesgos se pueden utilizar para etiquetar los riesgos que se agregan a los proyectos. Para obtener más información sobre cómo agregar riesgos a los proyectos, vea [Crear y editar riesgos en proyectos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
