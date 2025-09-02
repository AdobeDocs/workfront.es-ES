---
title: Agregar tipos de registro existentes
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede importar un tipo de registro existente desde otro espacio de trabajo.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 976810c8cedc5d3c5afd8333fdbace4fe8d0ccda
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 9%

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

Como administrador de espacio de trabajo, puede importar o agregar un tipo de registro existente a otro espacio de trabajo.

Primero debe designar un tipo de registro como centralizado antes de que los administradores de espacio de trabajo puedan importarlo a otros espacios de trabajo.

Puede designar un tipo de registro como centralizado al crearlo o editarlo, al definir su configuración de espacio de trabajo cruzado.

Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

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
   <td role="rowheader"><p>Paquete Adobe Workfront*</p></td> 
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

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Descripción general de los tipos de registros centralizados

Consideraciones al agregar tipos de registros existentes desde otro espacio de trabajo

* Cuando no hay ningún tipo de registro configurado para añadirse a otro espacio de trabajo, no se muestra la opción de importarlo desde otro espacio de trabajo al crear un tipo de registro. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* Después de agregar el tipo de registro desde otro espacio de trabajo, también se agrega la siguiente información desde el tipo de registro existente:

   * Campos
   * Registrar conexiones

* Solo se pueden ver los registros añadidos desde otros espacios de trabajo si se dispone de permisos para dichos espacios de trabajo.

* Sólo puede editar el tipo de registro, incluidos sus campos, en su espacio de trabajo original. No puede editarlo desde los espacios de trabajo en los que se añadió.
* Los registros añadidos desde todos los espacios de trabajo serán visibles para todos los usuarios que accedan a ellos desde todos los espacios de trabajo, incluso si se crean en un espacio de trabajo en el que no tienen permisos.

## Crear un tipo de registro a partir de un tipo de registro existente

1. Comience a crear un tipo de registro, tal como se describe en el artículo [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md), luego haga clic en **Agregar tipos de registros existentes**. <!--check this - the option might have been renamed in the UI-->

   ![Modal para agregar el tipo de registro con la opción de importar desde otro espacio de trabajo](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Haga clic en **Continuar**.
1. En el cuadro **Elegir tipo de registro**, haga clic en la tarjeta del tipo de registro que desee agregar desde un área de trabajo existente y, a continuación, haga clic en **Agregar**.

   El tipo de registro se añade al espacio de trabajo seleccionado y se producen las siguientes situaciones:

   * El icono **tipo de registro entre espacios de trabajo** ![icono de conexión entre espacios de trabajo](assets/global-icon.png) se agrega a la tarjeta del tipo de registro importado.
   * El campo **Workspace** de solo lectura se agrega al tipo de registro importado. El campo muestra en qué espacio de trabajo se creó cada registro.

     >[!NOTE]
     >
     >* No se puede editar el tipo de registro importado ni sus campos. Puede editar el tipo de registro y sus campos desde el espacio de trabajo original.

1. (Opcional) Haga clic en el menú **Más** ![Más menú](assets/more-menu.png) en la tarjeta del tipo de registro importado, o a la derecha del nombre del tipo de registro en su página, luego haga clic en **Eliminar**.
1. (Condicional) Escriba **delete** en el campo proporcionado y luego haga clic en **Eliminar permanentemente**.

   Quita el tipo de registro importado del espacio de trabajo seleccionado. El tipo de registro original y sus campos permanecen en su espacio de trabajo original.

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



