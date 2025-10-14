---
title: Agregar tipos de registros existentes desde otro Workspace
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede agregar un tipo de registro existente creado en otro espacio de trabajo.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 4%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Agregar tipos de registros existentes desde otro espacio de trabajo

{{planning-important-intro}}

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como administrador de espacio de trabajo, puede agregar un tipo de registro que exista en otro espacio de trabajo a un espacio de trabajo que administre en Adobe Workfront Planning.

Un administrador de espacio de trabajo debe designar primero un tipo de registro como tipo de registro global antes de poder agregarlo a los espacios de trabajo que administre como tipo de registro existente. Los administradores de Workspace pueden designar un tipo de registro como global cuando lo crean o editan, definiendo la configuración de área de trabajo cruzada del tipo de registro.

Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Este artículo describe cómo se puede agregar un tipo de registro de uno existente y cómo se puede eliminar, si ya no es necesario.

Antes de agregar registros a un área de trabajo desde un tipo de registro global, vea también el artículo [Información general sobre los tipos de registros entre áreas de trabajo](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<p>Y</p>
<li><p>Cualquier paquete de Planning para crear tipos de registros conectables</p></li>
<li><p>Un paquete de Planning Plus para crear tipos de registros globales</p></li>
</ul>
O
<ul><li><p>Un paquete de flujo de trabajo de Prime o Ultimate</p> </li>
Y
<li><p>Un paquete de Planning Prime o Ultimate</p></li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administrar permisos en un área de trabajo y en el tipo de registro </a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Crear un tipo de registro agregando uno existente de otro espacio de trabajo

>[!NOTE]
>
>Asegúrese de que haya al menos un tipo de registro designado para ser global en al menos otro espacio de trabajo.

1. Comience a crear un tipo de registro, tal como se describe en el artículo [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md), luego haga clic en **Agregar tipos de registros existentes**. <!--check this - the option might have been renamed in the UI-->

   ![Modal para agregar el tipo de registro con la opción de agregar desde otro espacio de trabajo](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Cuando no hay tipos de registros configurados para agregarse a otros espacios de trabajo en el sistema, no se muestra la opción **Agregar existentes**.

1. Haga clic en **Continuar**.
1. En el cuadro **Elija el tipo de registro**, haga clic en la tarjeta del tipo de registro que desee agregar desde un área de trabajo existente y, a continuación, haga clic en **Agregar**.

   El tipo de registro se agrega al área de trabajo seleccionada y el icono **tipo de registro global** ![](assets/global-icon.png) se muestra en la tarjeta del tipo de registro.

   Ocurren lo siguiente:

   * También se agrega la siguiente información desde el tipo de registro global existente:

      * Todos los campos originales
      * Todas las conexiones de registros
   * Solo se pueden ver los registros agregados desde otros espacios de trabajo que utilizan el mismo tipo de registro global cuando se tiene al menos permisos de visualización para dichos espacios de trabajo.
   * El campo **Workspace** de solo lectura se agrega a la nueva vista de tabla de tipo de registro. El campo muestra el espacio de trabajo donde se creó cada registro.

     >[!NOTE]
     >
     >No puede editar el aspecto, la configuración adicional ni los campos originales del nuevo tipo de registro. Sólo se puede editar el tipo de registro y todos sus campos y configuraciones originales desde el espacio de trabajo original.

1. (Opcional) Haga clic en y, a continuación, arrastre y suelte el tipo de registro recién añadido en cualquier sección del espacio de trabajo.

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—consultar con Lilit si podemos añadir automatizaciones o formularios de solicitud a RT globales secundarios??—añadir paso con enlaces a esos artículos si/ cuando sí—>

## Eliminar un tipo de registro global de un espacio de trabajo secundario

Puede eliminar un tipo de registro que haya añadido desde otro espacio de trabajo si ya no es necesario. Al eliminarla, solo se eliminará del espacio de trabajo secundario.

Al eliminar un tipo de registro global de un espacio de trabajo secundario, también se eliminan los siguientes elementos:

* Los registros añadidos desde el espacio de trabajo secundario.
* Los campos añadidos desde el espacio de trabajo secundario.

Los tipos de registros globales eliminados de sus espacios de trabajo secundarios no se pueden recuperar.

El tipo de registro original permanece en su espacio de trabajo original, así como en otros espacios de trabajo en los que se ha agregado.

Para suprimir un tipo de registro global de un espacio de trabajo secundario:

1. Vaya al tipo de registro global en el espacio de trabajo secundario.

1. (Opcional) Haga clic en el menú **Más** ![Más menú](assets/more-menu.png) de la tarjeta del tipo de registro o a la derecha del nombre del tipo de registro en su página y, a continuación, haga clic en **Eliminar**.
1. (Condicional) Escriba **delete** en el campo proporcionado y luego haga clic en **Eliminar permanentemente**.

   ![Eliminar cuadro de confirmación de tipo de registro global secundario](assets/delete-secondary-global-record-type.png)

   Ocurren lo siguiente:

   * El tipo de registro creado a partir de un tipo de registro global se quita del espacio de trabajo seleccionado.
   * El tipo de registro original y sus campos permanecen en su espacio de trabajo original.
   * El tipo de registro permanece en todos los demás espacios de trabajo en los que se ha añadido.
   * Se eliminan los registros y campos agregados al tipo de registro del espacio de trabajo actual. Se conservan todos los demás registros agregados desde espacios de trabajo adicionales donde se agregó el tipo de registro global. Los campos se conservan en los espacios de trabajo en los que se añadieron.





