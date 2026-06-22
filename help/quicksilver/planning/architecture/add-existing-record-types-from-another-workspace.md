---
title: Agregar tipos de registros existentes desde otro Workspace
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede agregar un tipo de registro existente creado en otro espacio de trabajo.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grtTc9KyoVJXzU27qkmFyJhY0mYtdSjz-Q1Pb-YqxLI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 793
ht-degree: 5%

---

# Agregar tipos de registros existentes desde otro espacio de trabajo

{{planning-important-intro}}


<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después del lanzamiento en Vista previa, las mismas funciones también están disponibles mensualmente en el entorno de producción para los clientes que habilitaron lanzamientos rápidos. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Como administrador de espacio de trabajo, puede agregar un tipo de registro que exista en otro espacio de trabajo a un espacio de trabajo que administre en Adobe Workfront Planning.

Un administrador de espacio de trabajo debe designar primero un tipo de registro como tipo de registro global antes de poder agregarlo a los espacios de trabajo que administre como tipo de registro existente. Los administradores de Workspace pueden designar un tipo de registro como global cuando lo crean o editan, definiendo la configuración de área de trabajo cruzada del tipo de registro.

Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Este artículo describe cómo agregar un tipo de registro de uno existente.

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
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Cualquier paquete Workfront y un paquete Planning Plus</p></li>
O
<li><p>Cualquier flujo de trabajo y un paquete de Planning Prime o Ultimate</p></p></li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--

Old:
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
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>

-->

## Crear un tipo de registro agregando uno existente de otro espacio de trabajo

>[!NOTE]
>
>Asegúrese de que haya al menos un tipo de registro designado para ser global en al menos otro espacio de trabajo principal.
>
>Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

1. Vaya a un espacio de trabajo en el que desee crear un tipo de registro (espacio de trabajo secundario).
1. Comience a crear un tipo de registro, tal como se describe en el artículo [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md), luego haga clic en **Agregar tipos de registros existentes**. <!--check this - the option might have been renamed in the UI-->

   ![Modal para agregar el tipo de registro con la opción de agregar desde otro espacio de trabajo](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Cuando no hay tipos de registros configurados para agregarse a otros espacios de trabajo en el sistema, no se muestra la opción **Agregar existentes**.

1. Haga clic en **Continuar**.
1. (Condicional) En el cuadro **Elija el tipo de registro**, haga clic en la tarjeta del tipo de registro que desee agregar desde un área de trabajo existente y, a continuación, haga clic en **Agregar**.

   <span class="preview">Si está usando el entorno de vista previa, puede hacer clic para seleccionar varios tipos de registros y, a continuación, hacer clic en **Agregar**. Se muestran en la lista todos los tipos de registros globales de todos los espacios de trabajo donde están disponibles.</span>

   El tipo de registro se agrega al espacio de trabajo secundario que seleccionó y el icono **tipo de registro global** ![icono de registro global en el espacio de trabajo secundario](assets/global-icon-secondary-workspace.png) se muestra en la tarjeta del tipo de registro.
El icono de tipo de registro global incluye una flecha cuando se muestra en un tipo de registro del espacio de trabajo secundario para indicar que el tipo de registro se agregó desde un tipo de registro existente.

   Ocurren lo siguiente:

   * También se agrega la siguiente información desde el tipo de registro global existente:

      * Todos los campos originales
      * Todas las conexiones de registros
   * No se pueden ver los registros agregados desde el espacio de trabajo original del tipo de registro desde el espacio de trabajo secundario.
   * Puede ver los registros agregados desde el espacio de trabajo original del tipo de registro en ese espacio de trabajo, sólo en el espacio de trabajo original, si tiene al menos permisos de Vista en ese espacio de trabajo.
   * El campo **Workspace** de solo lectura se agrega a la nueva vista de tabla de tipo de registro. El campo muestra el espacio de trabajo donde se creó cada registro.

     >[!NOTE]
     >
     >No puede editar el aspecto, la configuración adicional ni los campos originales del nuevo tipo de registro. Sólo se puede editar el tipo de registro y todos sus campos y configuraciones originales desde el espacio de trabajo original.
     >

1. (Opcional) Pase el ratón sobre el icono de tipo de registro global ![Icono de registro global en el espacio de trabajo secundario](assets/global-icon-secondary-workspace.png) para ver el nombre del espacio de trabajo original desde el que se agregó el tipo de registro.
1. (Opcional) Haga clic en y, a continuación, arrastre y suelte el tipo de registro recién añadido en cualquier sección del espacio de trabajo.
1. (Opcional) Haga clic en el menú **Más** de la tarjeta del nuevo tipo de registro o a la derecha del nombre del tipo de registro en su página y, a continuación, haga clic en una de las siguientes opciones:

   * **Compartir** para compartir el tipo de registro desde el espacio de trabajo secundario.
   * **Eliminar** para eliminar el tipo de registro del espacio de trabajo secundario. Al eliminar los tipos de registro del espacio de trabajo secundario también se eliminan los registros agregados desde el espacio de trabajo secundario.

     Las vistas añadidas desde el espacio de trabajo secundario no se eliminan. <!--checking with Lilit - not sure if this is by design??-->

   Para obtener más información, vea la sección &quot;Eliminar tipos de registros globales&quot; en el artículo [Eliminar tipos de registros](/help/quicksilver/planning/architecture/delete-record-types.md).

<!--
This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—consultando con Lilit si podemos añadir automatizaciones o formularios de solicitud a RT globales secundarios??—añadir paso con enlaces a esos artículos si/ cuando sí—>







