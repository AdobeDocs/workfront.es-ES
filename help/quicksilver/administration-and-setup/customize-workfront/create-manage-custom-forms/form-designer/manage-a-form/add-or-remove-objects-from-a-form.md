---
title: Agregar o eliminar tipos de objetos de un formulario personalizado existente con el diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede agregar o quitar tipos de objetos de los formularios personalizados con el diseñador de formularios.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# Agregar o eliminar tipos de objetos de un formulario personalizado existente con el diseñador de formularios

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa para todos los clientes de o en el entorno de producción para los clientes que habilitaron versiones rápidas de.</span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Activar o desactivar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obtener más información sobre la versión actual, consulte [Información general sobre la versión del segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Puede agregar o eliminar tipos de objetos de un formulario personalizado existente con el diseñador de formularios.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront</p> </td> 
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

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Agregar tipos de objetos a un formulario personalizado existente

Puede agregar tipos de objetos adicionales al formulario para que se pueda adjuntar a varios objetos.

>[!NOTE]
>
>Los permisos de salto de sección pueden verse afectados por el tipo de objeto. El permiso Editar de forma limitada para saltos de sección de formulario personalizados solo está disponible para los tipos de objeto Proyecto, Tarea, Problema y Usuario.
>
>Para obtener más información, consulte [Cómo pueden afectar varios tipos de objetos a los permisos de salto de sección](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Clic **Forms personalizado** en el panel izquierdo.

   En la vista que aparece, puede revisar todos los formularios personalizados que se han creado para su organización. También puede ver quién creó cada formulario, con qué tipo de objeto funciona y si está activo.

1. Seleccione el formulario personalizado al que desee agregar tipos de objeto adicionales y, a continuación, haga clic en **Editar** <span class="preview">o ![Icono Editar](assets/edit-icon.png).</span>

1. En la parte superior del formulario, haga clic en el signo más + después **Tipos de objetos**, a continuación, seleccione el tipo que desee en el menú que se muestra. Puede repetir esto para agregar todos los tipos de objetos que desee.

   ![](assets/add-new-object.png)

1. Clic **Guardar y cerrar**.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras crea un formulario personalizado para guardar los cambios y mantener el formulario abierto.

## Eliminar tipos de objetos en un formulario personalizado

Puede eliminar tipos de objetos de un formulario personalizado existente. Un formulario personalizado debe tener al menos un tipo de objeto.

>[!CAUTION]
>
>Si las personas ya han adjuntado el formulario personalizado a objetos del tipo que desea eliminar y le han agregado datos, esos datos se eliminan de forma permanente al eliminar ese tipo de objeto en el formulario. Puede incluir información histórica que los usuarios necesitarán más adelante.
>
>En general, se recomienda minimizar el número de veces que se edita un formulario personalizado que ya está en uso. No hay ningún sistema de notificación que avise a las personas que utilizan el formulario personalizado sobre sus cambios.

Para eliminar un tipo de objeto:

{{step-1-to-setup}}

1. Clic **Forms personalizado** en el panel izquierdo.
1. Seleccione el formulario personalizado que desee editar y haga clic en **Editar** <span class="preview">o ![Icono Editar](assets/edit-icon.png).</span>
1. Haga clic en la X de cualquiera de las **Tipos de objetos** que desee eliminar del formulario.

   ![](assets/delete-object-types.png)

1. (Opcional) Repita el paso anterior para cualquier otro tipo de objeto que desee quitar del formulario.
1. Clic **Listo**, luego haga clic en **Guardar y cerrar**.
