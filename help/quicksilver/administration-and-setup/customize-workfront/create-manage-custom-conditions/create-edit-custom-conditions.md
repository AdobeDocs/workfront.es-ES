---
title: Creación o edición de una condición personalizada
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Como administrador de Adobe Workfront, puede crear o editar una condición personalizada para proyectos, tareas y problemas que se ajuste a las necesidades de su organización.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 2%

---

# Creación o edición de una condición personalizada

Como administrador de Adobe Workfront, puede crear o editar una condición personalizada para proyectos, tareas y problemas que se ajuste a las necesidades de su organización.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Creación o edición de una condición personalizada

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Preferencias de proyecto** > **Condiciones**.

1. Haga clic en la ficha del tipo de objeto (**Proyecto**, **Tarea** o **Problema**) que desea asociar a la condición.

1. Para crear una nueva condición, haga clic en **Agregar una nueva condición**.

   O

   Para editar una condición existente, pase el ratón sobre la condición que desee editar y luego haga clic en la **Editar** que aparece en el extremo derecho.

   ![](assets/custom-condition-edit-nwe.jpg)

1. Configure la condición personalizada mediante las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Nombre de la condición</td> 
      <td>(Obligatorio) Escriba un nombre descriptivo para la condición.</td> 
     </tr> 
     <tr> 
      <td>Descripción</td> 
      <td>(Opcional) Escriba una descripción del propósito de la condición para quienes la usen.</td> 
     </tr> 
     <tr> 
      <td>Color</td> 
      <td>(Opcional) Haga clic en el icono de color y, a continuación, elija el color que desee para la condición cuando se muestre en proyectos, tareas o problemas. También puede escribir un número hexadecimal.</td> 
     </tr> 
     <tr> 
      <td>Igual que </td> 
      <td><p>(Necesario, solo para proyectos) Haga clic en la opción de la lista desplegable que mejor describe la función de la nueva condición. Por ejemplo, para una condición denominada Tracking Well, haría clic en On Target. Esto determina cómo funcionan las condiciones predeterminadas. Cada condición que cree debe coincidir con una de las opciones del menú desplegable.</p>
      <p>Para obtener información sobre las condiciones predeterminadas, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Establecer una condición personalizada como predeterminada para los proyectos</a> y <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Establecer una condición personalizada como predeterminada para tareas y problemas</a>.</p>
      <p>Esta opción no se puede modificar una vez que haya terminado de crear la condición.</p></td> 
     </tr> 
     <tr> 
      <td>Clave</td> 
      <td><p>(Obligatorio) Para una condición de proyecto, escriba una abreviatura alfanumérica que los usuarios puedan reconocer. Para una tarea o condición de problema, escriba un código numérico de dos dígitos del 01 al 99. </p>
      <p>Esta clave, que se utiliza en la API y se puede utilizar para la generación de informes, debe ser única para cada objeto.</p>
      <p>Después de guardar la condición, no se puede cambiar la clave de una condición. </p></td> 
     </tr> 
     <tr> 
      <td>Ocultar condición</td> 
      <td><p>(Opcional) Esta opción está disponible para condiciones personalizadas que ya no desea que utilicen las personas, pero que desea mantener por motivos históricos. </p>
      <p>Si oculta una condición personalizada que se ha utilizado en elementos de trabajo, seguirá apareciendo en esos elementos de trabajo después de ocultarla. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Puede estandarizar la terminología y los colores de las condiciones en los tres tipos de objetos. Para ello, copie la condición Name y el código hexadecimal de color de una pestaña (Proyecto, Tarea, Problema) a la condición correspondiente en las otras dos pestañas.

1. (Opcional) Arrastre ![](assets/move-icon---dots.png) cualquier condición a una nueva posición para reordenar la lista.

   Esto cambia el orden en el que se muestran las condiciones en los proyectos, tareas y problemas:

   * Cuando un usuario está editando un proyecto

      ![](assets/change-condition-edit-project.png)

   * Cuando un usuario cambia la condición de una tarea o un problema en la pestaña Actualizaciones :

      ![](assets/change-condition-update-comment.png)

   * Cuando un usuario cambia la condición de una tarea o un problema en una vista de lista:

      ![](assets/change-conditions-list-dropdown-only.png)

1. Haga clic en **Guardar**.

Puede establecer la condición personalizada como condición predeterminada para proyectos o para tareas y problemas. Para obtener más información, consulte [Establecer una condición personalizada como predeterminada para los proyectos](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) y [Establecer una condición personalizada como predeterminada para tareas y problemas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Para obtener más información sobre las condiciones personalizadas, consulte [Condiciones personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
