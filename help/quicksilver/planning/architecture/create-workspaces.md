---
title: Crear espacios de trabajo
description: Un área de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar completamente los espacios de trabajo en Adobe Workfront Planning. Los tipos de registro están organizados por secciones en un espacio de trabajo.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Creación de espacios de trabajo

{{planning-important-intro}}

En Adobe Workfront Planning, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo.

Un área de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar completamente los espacios de trabajo en Adobe Workfront Planning.

Para obtener información general acerca de los espacios de trabajo, vea [Información general sobre los espacios de trabajo](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

Debe tener lo siguiente para poder acceder a Workfront Planning:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plan Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Plan de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a la experiencia Adobe unificado para poder acceder a todas las funcionalidades de Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiencia unificada de Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront*</p></td> 
   <td><p> Estándar </p>
   <p>Workfront Planning no está disponible para licencias de Workfront heredadas</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Recibirá permisos de Administración en los espacios de trabajo que cree. </p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!---
OLD:

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
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>You receive Manage permissions to the workspaces you create. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Planning area to your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 
-->

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

   Para los administradores de Workfront, el nuevo espacio de trabajo se muestra en la ficha **Espacios de trabajo en los que participo**.

   Para todos los demás usuarios que pueden crear espacios de trabajo, el nuevo espacio de trabajo se muestra en el área **Espacios de trabajo**.

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


