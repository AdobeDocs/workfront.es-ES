---
title: Editar espacios de trabajo
description: Puede editar la información de un espacio de trabajo existente, como cambiarle el nombre.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Editar espacios de trabajo

{{planning-important-intro}}

En Adobe Workfront Planning, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo.

Un área de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar completamente los espacios de trabajo en Adobe Workfront Planning.

Para obtener información sobre la creación de espacios de trabajo, consulte [Creación de espacios de trabajo](/help/quicksilver/maestro/architecture/create-workspaces.md).

Todos los cambios que realice en un espacio de trabajo son visibles para todos los que tengan al menos permisos de visualización en el espacio de trabajo.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta cerrado de Adobe Workfront Planning. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td>
   <td>
   <p>Nuevo: estándar</p>
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en el espacio de trabajo </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>Debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Para obtener más información sobre los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Editar un espacio de trabajo

{{step1-to-maestro}}

Se abrirá el área de Espacios de trabajo de Workfront Planning.

1. Haga clic dentro del nombre del espacio de trabajo en el encabezado del nuevo espacio de trabajo para cambiarle el nombre y, a continuación, pulse **Entrar**.
1. Haga clic en **Más** menú ![](assets/more-menu.png)a la derecha del nombre del espacio de trabajo en el encabezado y haga clic en **Editar**.

   ![](assets/edit-workspace-box.png)

   Actualice la siguiente información en la **Editar espacio de trabajo** cuadro:

   * Añada un nombre al espacio de trabajo. <!--did they add a label for this field?-->
   * **Descripción**: Añada información sobre el espacio de trabajo.
   * Seleccione un icono para asociarlo al espacio de trabajo.

1. Clic **Guardar** para cerrar el cuadro Editar espacio de trabajo y aplicar los cambios.

1. (Opcional) Para agregar una nueva sección de espacio de trabajo, siga uno de estos procedimientos:

   * Clic **Agregar sección** en la parte inferior del espacio de trabajo.
   * Pase el ratón sobre el nombre de una sección y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Agregar sección anterior** o **Agregar sección debajo**.

1. (Opcional) Para cambiar la ubicación de una sección, siga uno de estos procedimientos:

   * Pase el ratón sobre el nombre de una sección y haga clic en **agarrar** icono ![](assets/grab-icon.png)A continuación, arrástrela y suéltela en el lugar correcto.
   * Pase el ratón sobre el nombre de una sección y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Mover hacia arriba** o **Mover hacia abajo**. La sección se mueve hacia arriba o hacia abajo dentro del espacio de trabajo.

1. (Opcional) Para eliminar una sección de Workspace, haga lo siguiente:

   1. Pase el ratón sobre el nombre de una sección y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Eliminar**. <!--add screen shot when UI is final?-->
   1. Seleccione una nueva sección para mover todos los tipos de registros y haga clic en **Eliminar**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Todos los tipos de registro se mueven a la sección de selección y esta se elimina.

1. (Opcional) Haga clic en **Añadir tipo de registro** para agregar tipos de registros al espacio de trabajo.

   Para obtener más información, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

1. (Opcional) Pase el ratón sobre una tarjeta de tipo de registro y haga clic en **Más** menú ![](assets/more-menu.png) en la esquina superior derecha, haga clic en **Editar** para modificar el aspecto de un tipo de registro.

   Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/maestro/architecture/edit-record-types.md).

1. (Opcional) Pase el ratón sobre una tarjeta de tipo de registro y haga clic en **Más** menú ![](assets/more-menu.png) en la esquina superior derecha, haga clic en **Eliminar** para eliminar un tipo de registro.

   Para obtener más información, consulte [Eliminar tipos de registros](/help/quicksilver/maestro/architecture/delete-record-types.md).

1. (Opcional) Pulse y haga clic en una tarjeta de tipo de registro para arrastrarla y soltarla en un nuevo lugar. Puede arrastrar y soltar tipos de registros de una sección de Workspace a otra.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Opcional) Haga clic en **Compartir** en la esquina superior derecha del espacio de trabajo para compartir el espacio de trabajo con otros usuarios.

   Para obtener más información, consulte [Compartir espacios de trabajo](/help/quicksilver/maestro/access/share-workspaces.md).
