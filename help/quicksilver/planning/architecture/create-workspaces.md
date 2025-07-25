---
title: Crear espacios de trabajo
description: Un espacio de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning. Los tipos de registro están organizados por secciones en un espacio de trabajo.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 78%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Crear espacios de trabajo

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

En Adobe Workfront Planning, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo.

Un espacio de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning.

Para obtener información general acerca de los espacios de trabajo, consulte [Información general sobre los espacios de trabajo](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

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
   <p> Productos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planificación de Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Plan de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera de los siguientes planes de Workfront:</p> 
<ul><li>Seleccionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning no está disponible para planes Workfront heredados</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Paquete de planificación de Adobe Workfront*</p></td> 
   <td> 
<p>Cualquiera </p> 
<p>Para obtener más información sobre qué se incluye en cada plan de Workfront Planning, póngase en contacto con su administrador de cuentas de Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma de Adobe Workfront</p></td> 
   <td> 
<p>La instancia de Workfront de su organización debe incorporarse a Adobe Unified Experience para poder acceder a Workfront Planning.</p> 
<p>Para obtener más información, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience para Workfront</a>. </p> 
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
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>No hay controles de nivel de acceso para Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Recibirá permisos de Administración en los espacios de trabajo que cree. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear un espacio de trabajo

Puede crear un espacio de trabajo y añadirle tipos de registro para organizar los objetos en Workfront Planning. Para obtener más información acerca de cómo editar un espacio de trabajo, consulte [Editar áreas de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Haga clic en **Crear espacio de trabajo**

   Se muestra el cuadro Crear espacio de trabajo. Puede crear un espacio de trabajo desde cero o crearlo con una de las plantillas disponibles.

1. (Opcional y condicional) Haga clic en **Vista previa** dentro de cualquiera de las siguientes plantillas de área de trabajo predefinidas:

   * Básico: administración de marketing
   * Administración avanzada de marketing
   * Empresa: administración de marketing
   * Administración de ventas
   * Administración de productos

   Se abrirá el cuadro de vista previa de plantilla.

   Existe una indicación de qué tipos de registros operativos, taxonomías y cuántos campos están asociados a cada plantilla.

   ![Vista previa de una plantilla de área de trabajo](assets/previewing-a-workspace-template.png)

   Para obtener información acerca de las plantillas de espacio de trabajo de Workfront Planning, consulte [Lista de plantillas de espacio de trabajo](/help/quicksilver/planning/architecture/workspace-templates.md).

1. En el cuadro de vista previa de la plantilla, haga clic en **Usar plantilla** para comenzar a crear el espacio de trabajo a partir de la plantilla seleccionada

   O

   Haga clic en **Atrás** y, a continuación, haga clic en **Nuevo espacio de trabajo** para crear un espacio de trabajo desde cero.

   Se crea uno para los siguientes tipos de espacios de trabajo:

   * Un espacio de trabajo vacío denominado **Espacio de trabajo sin título** donde puede empezar a añadir tipos de registros manualmente al crear un espacio de trabajo desde cero.
   * Espacio de trabajo con el nombre de la plantilla seleccionada que se rellena con tipos de registros de ejemplo. Puede personalizar aún más los tipos de registro y el espacio de trabajo.

   Para los administradores de Workfront, el nuevo espacio de trabajo se muestra en la ficha **Espacios de trabajo en los que participo**.

   Para todos los demás usuarios que pueden crear espacios de trabajo, el nuevo espacio de trabajo se muestra en el área **Espacios de trabajo**.

1. Haga clic dentro del nombre del espacio de trabajo en el encabezado del nuevo espacio de trabajo para cambiarle el nombre y, a continuación, pulse Entrar.

1. (Opcional y condicional) Si creó el área de trabajo a partir de una plantilla, haga clic dentro del nombre de las secciones **Tipos de registros operativos** o **Taxonomías**

   O

   Pase el ratón sobre el nombre de una sección, luego haga clic en el menú **Más** ![Menú más](assets/more-menu.png), luego haga clic en **Cambiar nombre** para cambiar el nombre de la sección.

   >[!TIP]
   >
   >Puede cambiar el nombre de cualquier sección desde cualquier espacio de trabajo, incluso si no ha creado la sección.

   Para obtener más información sobre la edición de espacios de trabajo, incluida la edición de espacios de trabajo, consulte [Editar espacios de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Opcional) Haga clic en **Añadir tipo de registro** para añadir tipos de registro al área de trabajo en cualquier sección.

   Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

   Para obtener más información sobre la edición y eliminación de tipos de registros en un área de trabajo, consulte [Editar áreas de trabajo](/help/quicksilver/planning/architecture/edit-workspaces.md).


