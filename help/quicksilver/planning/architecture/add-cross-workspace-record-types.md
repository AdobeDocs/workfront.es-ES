---
title: Agregar tipos de registros entre espacios de trabajo
description: Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. En Workfront Planning, puede importar un tipo de registro existente desde otro espacio de trabajo.
hidefromtoc: true
hide: true
source-git-commit: 459e3883101b644a91d5e2a32288cf5b02a02bd9
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 25%

---


<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Añadir tipos de registros entre espacios de trabajo

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como administrador de espacio de trabajo, puede importar o agregar un tipo de registro existente a otro espacio de trabajo.

Primero debe definir las capacidades de un tipo de registro entre espacios de trabajo para que los administradores de espacios de trabajo puedan importarlo a otros espacios de trabajo.

Las funciones entre espacios de trabajo de un tipo de registro se definen al crear o editar un tipo de registro.

Para obtener más información, vea [Configurar las capacidades entre espacios de trabajo para los tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

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
   <td><p> Estándar</p>
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
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al agregar tipos de registros existentes desde otro espacio de trabajo

* Cuando no hay ningún tipo de registro configurado para añadirse a otro espacio de trabajo, no se muestra la opción de importarlo desde otro espacio de trabajo al crear un tipo de registro. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* Después de agregar el tipo de registro desde otro espacio de trabajo, también se agrega la siguiente información desde el tipo de registro existente:

   * Campos
   * Registros
   * Registrar conexiones

## Crear un tipo de registro a partir de un tipo de registro global existente

1. Comience a crear un tipo de registro, tal como se describe en el artículo [Crear tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md), y después haga clic en **Usar tipo de registro global**. <!--check this - the option might have been renamed in the UI-->