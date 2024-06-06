---
title: Creación de espacios de trabajo
description: Un área de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar completamente los espacios de trabajo en Adobe Workfront Planning. Los tipos de registro están organizados por secciones en un espacio de trabajo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 3a819fc18e0b5f438a55265ea0c5c9679ef0fdd6
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Creación de espacios de trabajo

{{planning-important-intro}}

En Adobe Workfront Planning, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo.

Un área de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar completamente los espacios de trabajo en Adobe Workfront Planning.

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
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
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
   O
   <p>Actual: plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Recibirá permisos de Administración en los espacios de trabajo que cree. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>Debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Para obtener más información sobre los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Consideraciones sobre espacios de trabajo

* Puede crear espacios de trabajo para unidades organizativas específicas dentro de su organización, de modo que coincidan con el modo exclusivo en que funciona cada unidad.
* Los tipos de registro que contiene un espacio de trabajo deben reflejar el ciclo de vida laboral de una unidad organizativa.
* Al crear un espacio de trabajo, sólo usted tiene permiso para acceder y administrar el espacio de trabajo. Debe compartirlo con otros usuarios para que puedan colaborar con usted en el mismo espacio. Para obtener más información, consulte [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md). Los administradores del sistema pueden administrar todos los espacios de trabajo, incluso los que no hayan creado.
* Puede tener lo siguiente:

   * Hasta 50 secciones en un espacio de trabajo.
   * Hasta un total de 1000 tipos de registros de todas las secciones de un espacio de trabajo. Todos los tipos de registro son únicos para cada espacio de trabajo. <!--this might change-->
   * Hasta 1000 espacios de trabajo en la instancia de Workfront de su organización.


## Crear un espacio de trabajo

Puede crear un espacio de trabajo y agregarle tipos de registro para organizar los objetos en Workfront Planning. Para obtener más información sobre la edición de un espacio de trabajo, consulte [Editar espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

<!--replace the snippet with the new snippet with the landing page The Workfront Planning landing page opens. 
    ![](assets/planning-landing-page-admin.png)
    1. (Optional) Click the **My workspaces** tab to view workspaces you created
    Or
    Click the **Other workspaces** tab to view workspaces shared with you. 
    -->

1. (Condicional) Si no tiene ningún espacio de trabajo en su entorno, haga clic en **Crear espacio de trabajo**

   O bien, en un espacio de trabajo existente, haga clic en la flecha hacia abajo situada a la derecha del nombre del espacio de trabajo y, a continuación, haga clic en **Crear espacio de trabajo**.

   ![](assets/workspace-drop-down-right-menu.png)


1. (Opcional y condicional) Haga clic en **Previsualizar** dentro de cualquiera de las siguientes plantillas predefinidas de workspace:

   * Gestión de marketing
   * Administración de ventas
   * Administración de productos

   Existe una indicación de qué tipos de registros operativos, taxonomías y cuántos campos están asociados a cada plantilla.

   ![](assets/previewing-a-workspace-template.png)

   Para obtener información sobre las plantillas de espacio de trabajo de Workfront Planning, consulte [Lista de plantillas de Workspace](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Clic **Usar plantilla** para empezar a crear el espacio de trabajo a partir de la plantilla seleccionada

   O

   Clic **Crear espacio de trabajo** para crear un espacio de trabajo desde cero.

   Se crea uno para los siguientes tipos de espacios de trabajo:

   * Un espacio de trabajo vacío denominado **Espacio de trabajo sin título** donde puede empezar a agregar tipos de registros manualmente, al crear un espacio de trabajo desde cero.
   * Espacio de trabajo con el nombre de la plantilla seleccionada que se rellena con tipos de registros de ejemplo. Puede personalizar aún más los tipos de registro y el espacio de trabajo.

1. Haga clic dentro del nombre del espacio de trabajo en el encabezado del nuevo espacio de trabajo para cambiarle el nombre y, a continuación, pulse Entrar.

1. (Opcional y condicional) Si ha creado el espacio de trabajo a partir de una plantilla, haga clic dentro del nombre del **Tipos de registros operativos** o **Taxonomías** secciones

   O

   Pase el ratón sobre el nombre de una sección y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Cambiar nombre** para cambiar el nombre de la sección.

   >[!TIP]
   >
   >Puede cambiar el nombre de cualquier sección desde cualquier espacio de trabajo, incluso si no ha creado la sección.

   Para obtener más información sobre la edición de espacios de trabajo, incluida la edición de secciones de espacios de trabajo, consulte [Editar espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Opcional) Haga clic en **Añadir tipo de registro** para agregar tipos de registros al espacio de trabajo en cualquier sección.

   Para obtener más información, consulte [Creación de tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   Para obtener más información sobre cómo editar y eliminar tipos de registros en un espacio de trabajo, consulte [Editar espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).


