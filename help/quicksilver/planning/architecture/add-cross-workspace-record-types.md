---
title: Agregar tipos de registro existentes
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede agregar un tipo de registro existente creado en otro espacio de trabajo.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 6%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Agregar tipos de registros existentes

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como administrador de área de trabajo, puede agregar un tipo de registro que exista en un área de trabajo a un área de trabajo que administre en Adobe Workfront Planning.

Primero debe designar un tipo de registro como centralizado antes de que los administradores de espacio de trabajo puedan agregarlo a otros espacios de trabajo como un tipo de registro existente.

Puede designar un tipo de registro como centralizado al crearlo o editarlo, al definir su configuración de espacio de trabajo cruzado.

Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Antes de agregar registros a un área de trabajo desde un tipo de registro centralizado, vea el artículo [Información general sobre los tipos de registros centralizados](/help/quicksilver/planning/architecture/centralized-record-types-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr>

</tr>   
<tr> 
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Cualquier paquete de Workfront</p></li>
Y
<li><p>Paquete Planning Plus</p></li></ul>
O
<ul><li><p>Cualquier paquete de flujo de trabajo</p> </li>
Y
<li><p>Planificación del paquete de Prime o Ultimate</p></li></ul>
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Crear un tipo de registro a partir de un tipo de registro existente

1. Comience a crear un tipo de registro, tal como se describe en el artículo [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md), luego haga clic en **Agregar tipos de registros existentes**. <!--check this - the option might have been renamed in the UI-->

   ![Modal para agregar el tipo de registro con la opción de agregar desde otro espacio de trabajo](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Haga clic en **Continuar**.
1. En el cuadro **Elegir tipo de registro**, haga clic en la tarjeta del tipo de registro que desee agregar desde un área de trabajo existente y, a continuación, haga clic en **Agregar**.

   El tipo de registro se añade al espacio de trabajo seleccionado.

   >[!TIP]
   >
   >Cuando no hay ningún tipo de registro configurado para agregarse a otro espacio de trabajo, no se muestra la opción de agregarlo desde otro espacio de trabajo al crear un tipo de registro.

   Ocurren lo siguiente:

   * También se agrega la siguiente información del tipo de registro centralizado existente:

      * Todos los campos originales
      * Todas las conexiones de registros
   * Solo puede ver los registros añadidos desde otros espacios de trabajo si tiene al menos permisos de visualización en dichos espacios de trabajo.
   * El icono **tipo de registro centralizado** ![icono de tipo de registro centralizado](assets/global-icon.png) se agrega a la tarjeta del nuevo tipo de registro.
   * El campo **Workspace** de solo lectura se agrega a la nueva vista de tabla de tipo de registro. El campo muestra en qué espacio de trabajo se creó cada registro.

     >[!NOTE]
     >
     >* No puede editar el aspecto, la configuración avanzada o los campos originales del nuevo tipo de registro. Sólo se puede editar el tipo de registro y todos sus campos y configuraciones originales desde el espacio de trabajo original.

1. (Opcional) Haga clic en y, a continuación, arrastre y suelte el tipo de registro recién añadido en cualquier sección del espacio de trabajo.

1. (Opcional) Haga clic en el menú **Más** ![Más menú](assets/more-menu.png) en la tarjeta del nuevo tipo de registro o a la derecha del nombre del tipo de registro en su página y, a continuación, haga clic en **Compartir** para compartirlo con otros usuarios del mismo área de trabajo.

1. (Opcional) Haga clic en el menú **Más** ![Más menú](assets/more-menu.png) en la tarjeta del nuevo tipo de registro, o a la derecha del nombre del tipo de registro en su página, y luego haga clic en **Eliminar**.
1. (Condicional) Escriba **delete** en el campo proporcionado y luego haga clic en **Eliminar permanentemente**.

   Ocurren lo siguiente:

   * El tipo de registro creado a partir de un tipo de registro centralizado se elimina del espacio de trabajo seleccionado.
   * El tipo de registro original y sus campos permanecen en su espacio de trabajo original.
   * Todos los demás tipos de registro agregados desde el mismo tipo de registro centralizado permanecen en sus espacios de trabajo.
   * Se eliminan los registros agregados al tipo de registro del área de trabajo actual. Se conservan todos los demás registros agregados desde espacios de trabajo adicionales en los que se agregó el tipo de registro centralizado.





