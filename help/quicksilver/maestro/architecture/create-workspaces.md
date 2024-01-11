---
title: Creación de espacios de trabajo
description: Un área de trabajo es un conjunto de tipos de registros operativos y taxonomías que utiliza un equipo y representa el ciclo de vida del trabajo del equipo. Puede personalizar completamente los espacios de trabajo en Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Creación de espacios de trabajo

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para utilizar las funciones de Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

En Adobe Maestro, los espacios de trabajo son ubicaciones centralizadas para que los equipos planifiquen el trabajo.

Un área de trabajo es un conjunto de tipos de registros operativos y taxonomías que utiliza un equipo y representa el ciclo de vida del trabajo del equipo. Puede personalizar completamente los espacios de trabajo en Maestro.

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
<p>Su organización debe estar inscrita en el programa beta cerrado de Adobe Maestro. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <p>Actual: Trabajo o superior</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Maestro</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Recibirá permisos de Administración en los espacios de trabajo que cree. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>Debe agregar el área de Maestro a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Para obtener más información sobre los requisitos de acceso, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Consideraciones sobre espacios de trabajo

* Puede crear espacios de trabajo para unidades organizativas específicas dentro de su organización, de modo que coincidan con el modo exclusivo en que funciona cada unidad.
* Los tipos de registro y las taxonomías que contiene un espacio de trabajo deben reflejar el ciclo de vida de trabajo de una unidad organizativa.
* Al crear un espacio de trabajo, sólo usted tiene permiso para acceder y administrar el espacio de trabajo. Debe compartirlo con otros usuarios para que puedan colaborar con usted en el mismo espacio. Para obtener más información, consulte [Compartir un espacio de trabajo](/help/quicksilver/maestro/access/share-workspaces.md).
* Puede tener un máximo de 1000 espacios de trabajo en su organización.
* Los espacios de trabajo contienen tipos de registros exclusivos de cada espacio de trabajo. <!--this might change-->

## Crear un espacio de trabajo

{{step1-to-maestro}}

1. (Condicional) Si no tiene ningún espacio de trabajo en su entorno, haga clic en **Crear espacio de trabajo**

   O bien, desde un espacio de trabajo existente, haga clic en el área de trabajo orientada hacia abajo a la derecha del nombre del espacio de trabajo y, a continuación, haga clic en **Crear espacio de trabajo**.

   ![](assets/workspace-drop-down-right-menu.png)

   Se abrirá el área Espacios de trabajo de Maestro.
1. (Opcional y condicional) Haga clic en **Previsualizar** dentro de cualquiera de las siguientes plantillas predefinidas de workspace:

   * Gestión de marketing
   * Administración de ventas
   * Administración de productos

   Existe una indicación de qué tipos de registros operativos, taxonomías y cuántos campos están asociados a cada plantilla.

   ![](assets/previewing-a-workspace-template.png)

   Para obtener información acerca de las plantillas de área de trabajo de Maestro, vea [Lista de plantillas de Workspace](../architecture/workspace-templates.md).

1. Clic **Usar plantilla** para empezar a crear el espacio de trabajo a partir de la plantilla seleccionada

   O

   Clic **Crear espacio de trabajo** para crear un espacio de trabajo desde cero.

   Se crea uno para los siguientes tipos de espacios de trabajo:

   * Espacio de trabajo vacío en el que puede empezar a agregar tipos de registros manualmente.
   * Espacio de trabajo rellenado con tipos de registros de ejemplo que se pueden personalizar aún más.

1. Haga clic dentro del nombre del espacio de trabajo en el encabezado del nuevo espacio de trabajo para cambiarle el nombre y, a continuación, pulse Entrar

   O

   Haga clic en **Más** menú ![](assets/more-menu.png)a la derecha del nombre del espacio de trabajo en el encabezado y haga clic en **Cambiar nombre**.

1. (Opcional) Haga clic en **Añadir tipo de registro** para agregar tipos de registros al espacio de trabajo.

   Para obtener más información, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

1. (Opcional) Haga clic en **Añadir taxonomía** para agregar taxonomías al espacio de trabajo.

   Para obtener más información, consulte [Creación de taxonomías](../architecture/create-a-taxonomy.md).
