---
title: Agregar o eliminar tipos de objetos de un formulario personalizado existente
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede añadir o quitar tipos de objetos de los formularios personalizados con el diseñador de formularios.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 96%

---

# Añadir o eliminar tipos de objetos de un formulario personalizado existente

Puede añadir o eliminar tipos de objetos de un formulario personalizado existente con el diseñador de formularios.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Para realizar los pasos de este artículo, debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td><p>Acceso administrativo a formularios personalizados</p></td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir tipos de objetos a un formulario personalizado existente

Puede añadir tipos de objetos adicionales al formulario para que se pueda adjuntar a varios objetos.

>[!NOTE]
>
>Los permisos de salto de sección pueden verse afectados por el tipo de objeto. El permiso de Edición limitada para saltos de sección de formularios personalizados solo está disponible para los tipos de objeto Proyecto, Tarea, Problema y Usuario.
>
>Para obtener más información, vea [Cómo pueden afectar varios tipos de objetos a los permisos de saltos de sección](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados** en el panel izquierdo.

   En la vista que aparece, puede revisar todos los formularios personalizados que se han creado para su organización. También puede ver quién creó cada formulario, con qué tipo de objeto funciona y si está activo.

1. Seleccione el formulario personalizado al que desee añadir tipos de objetos adicionales y, a continuación, haga clic en ![Editar icono](assets/edit-icon2.png).

1. En la parte superior del formulario, haga clic en el signo + después de **Tipos de objetos** y, a continuación, seleccione el tipo que desee en el menú que aparece. Puede repetir esta acción para añadir todos los tipos de objetos que desee.

   ![Agregar nuevo objeto](assets/add-new-object.png)

1. Haga clic en **Guardar y cerrar**.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras crea un formulario personalizado para guardar los cambios y mantener el formulario abierto.

## Eliminar tipos de objetos en un formulario personalizado

Puede eliminar tipos de objetos de un formulario personalizado existente. Un formulario personalizado debe tener al menos un tipo de objeto.

>[!CAUTION]
>
>Si las personas ya han adjuntado el formulario personalizado a objetos del tipo que desea eliminar y le han añadido datos, esos datos se eliminan de forma permanente al eliminar ese tipo de objeto en el formulario. Puede incluir información histórica que los usuarios necesitarán más adelante.
>
>En general, se recomienda minimizar el número de veces que se edita un formulario personalizado que ya está en uso. No hay ningún sistema de notificación que avise a las personas que utilizan el formulario personalizado sobre sus cambios.

Para eliminar un tipo de objeto:

{{step-1-to-setup}}

1. Haga clic en **Formularios personalizados** en el panel izquierdo.
1. Seleccione el formulario personalizado que desee editar y luego haga clic en ![Editar icono](assets/edit-icon2.png).
1. Haga clic en la X de cualquiera de los **Tipos de objetos** que desee eliminar del formulario.

   ![Eliminar tipos de objetos](assets/delete-object-types.png)

1. (Opcional) Repita el paso anterior para cualquier otro tipo de objeto que desee quitar del formulario.
1. Haga clic en **Aplicar** y luego haga clic en **Guardar y cerrar**.
