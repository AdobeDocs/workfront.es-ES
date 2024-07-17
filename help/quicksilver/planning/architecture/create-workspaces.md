---
title: Creación de espacios de trabajo
description: Un área de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar completamente los espacios de trabajo en Adobe Workfront Planning. Los tipos de registro están organizados por secciones en un espacio de trabajo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '642'
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
   <td> <p>Debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Resumen de acceso</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Para obtener más información acerca de los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
* Al crear un espacio de trabajo, sólo usted tiene permiso para acceder y administrar el espacio de trabajo. Debe compartirlo con otros usuarios para que puedan colaborar con usted en el mismo espacio. Para obtener más información, vea [Compartir un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md). Los administradores del sistema pueden administrar todos los espacios de trabajo, incluso los que no hayan creado.
* Puede tener lo siguiente:

   * Hasta 50 secciones en un espacio de trabajo.
   * Hasta un total de 1000 tipos de registros de todas las secciones de un espacio de trabajo. Todos los tipos de registro son únicos para cada espacio de trabajo. <!--this might change-->
   * Hasta 1000 espacios de trabajo en la instancia de Workfront de su organización.


## Crear un espacio de trabajo

Puede crear un espacio de trabajo y agregarle tipos de registro para organizar los objetos en Workfront Planning. Para obtener más información acerca de cómo editar un área de trabajo, vea [Editar áreas de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Haga clic en **Crear espacio de trabajo**

   Se muestra el cuadro Crear espacio de trabajo. Puede crear un espacio de trabajo desde cero o crearlo con una de las plantillas disponibles.

1. (Opcional y condicional) Haga clic en **Vista previa** dentro de cualquiera de las siguientes plantillas de área de trabajo predefinidas:

   * Básico: gestión de marketing
   * Avanzado: Gestión de marketing
   * Empresa: gestión de marketing
   * Administración de ventas
   * Administración de productos

   Se abrirá el cuadro de vista previa de plantilla.

   Existe una indicación de qué tipos de registros operativos, taxonomías y cuántos campos están asociados a cada plantilla.

   ![](assets/previewing-a-workspace-template.png)

   Para obtener información acerca de las plantillas de área de trabajo de Workfront Planning, vea [Lista de plantillas de área de trabajo](/help/quicksilver/planning/architecture/workspace-templates.md).

1. En el cuadro de vista previa de la plantilla, haga clic en **Usar plantilla** para comenzar a crear el área de trabajo a partir de la plantilla seleccionada

   O

   Haga clic en **Atrás** y, a continuación, haga clic en **Nuevo espacio de trabajo** para crear un espacio de trabajo desde cero.

   Se crea uno para los siguientes tipos de espacios de trabajo:

   * Un área de trabajo vacía denominada **Workspace sin título** donde puede empezar a agregar tipos de registros manualmente al crear un área de trabajo desde cero.
   * Espacio de trabajo con el nombre de la plantilla seleccionada que se rellena con tipos de registros de ejemplo. Puede personalizar aún más los tipos de registro y el espacio de trabajo.

1. Haga clic dentro del nombre del espacio de trabajo en el encabezado del nuevo espacio de trabajo para cambiarle el nombre y, a continuación, pulse Entrar.

1. (Opcional y condicional) Si creó el área de trabajo a partir de una plantilla, haga clic dentro del nombre de las secciones **Tipos de registros operativos** o **Taxonomías**

   O

   Pase el ratón sobre el nombre de una sección, luego haga clic en el menú **Más** ![](assets/more-menu.png) y luego haga clic en **Cambiar nombre** para cambiar el nombre de la sección.

   >[!TIP]
   >
   >Puede cambiar el nombre de cualquier sección desde cualquier espacio de trabajo, incluso si no ha creado la sección.

   Para obtener más información acerca de cómo editar espacios de trabajo, incluidas las secciones de los mismos, consulte [Editar espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Opcional) Haga clic en **Agregar tipo de registro** para agregar tipos de registro al área de trabajo en cualquier sección.

   Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   Para obtener más información acerca de cómo editar y eliminar tipos de registros en un área de trabajo, vea [Editar áreas de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).


