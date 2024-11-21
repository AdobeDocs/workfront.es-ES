---
title: Editar configuración de campo
description: En Adobe Workfront Planning, puede editar la configuración de campo de los campos que ya se han creado. En este artículo se describe cómo editar la configuración de los campos de Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 1%

---


# Editar configuración de campo

{{planning-important-intro}}

Puede editar la configuración de campo de los campos que ya se han creado en Adobe Workfront Planning.

Para obtener información acerca de cómo crear campos de Adobe Workfront Planning, vea [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

En este artículo se describe cómo editar la configuración de los campos de Workfront Planning. Para obtener información acerca de cómo editar los valores de campo de los registros, vea [Editar registros](/help/quicksilver/planning/records/edit-records.md).

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso para Workfront Planning.

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
   <td role="rowheader"><p>plan Adobe Workfront*</p></td> 
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
   <td>   <p>Administrar permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Plantilla de diseño</p></td> 
   <td> <p>A todos los usuarios, incluidos los administradores de Workfront, se les debe asignar una plantilla de diseño que incluya el área de Planning en el menú principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obtener más información sobre los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD

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
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Consideraciones sobre la edición de configuración de campo

Debe tener en cuenta lo siguiente antes de realizar cambios en la configuración de un campo:

* Puede editar los campos que ha creado o los campos creados por otros usuarios si tiene permisos de administración en el espacio de trabajo al que pertenecen los campos.
* Puede editar un campo en la tabla de tipo de registro.
* No se puede editar un campo en la página de registro ni en ninguna otra vista, fuera de la vista de tabla.
* Una vez guardado el campo, no se puede editar el tipo de campo.
* No puede anular la selección de la opción Permitir números negativos seleccionada anteriormente para un campo Número, Porcentaje o Moneda si ya hay valores negativos almacenados en los registros a los que está asociada.
* Puede editar la configuración de los siguientes elementos de campo después de guardar el campo:

   * El nombre o la descripción de cualquier campo
   * Las opciones de un campo de selección única o de selección múltiple.
   * La expresión de un campo de fórmula.

  >[!WARNING]
  >
  >Cuando cambian las expresiones de fórmula o se agregan o eliminan opciones de un campo de tipo select, se perderán datos de los registros que ya tienen información almacenada en los campos cuya configuración se modifica.
  >
  >No hay advertencia ni indicación de que esta pérdida de datos pueda producirse al cambiar la configuración de los campos.
  >
  >No hay ninguna notificación a otros usuarios de que la configuración del campo haya cambiado.

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Editar configuración de campo

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos campos de registro desee editar.

   El espacio de trabajo se abre y todos los tipos de registros del espacio de trabajo se muestran en tarjetas.

1. Haga clic en la tarjeta de un tipo de registro.

   Se abre la página del tipo de registro.

1. (Condicional) Haga clic en la ficha de una **vista de tabla**.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.
1. Pase el ratón sobre el encabezado de columna del campo que quiera editar, luego haga clic en la flecha que apunta hacia abajo después del nombre del campo y luego haga clic en **Editar campo**

   O

   Haga doble clic en el encabezado de columna del campo.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Actualice la información sobre el campo y haga clic en **Guardar**. <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* No se puede actualizar el tipo de campo una vez guardado el campo.
   >
   >* Al modificar las configuraciones de campo (opciones de campo o expresiones de fórmula), los registros que ya contienen información en los campos modificados actualizarán sus valores en tiempo real. No hay advertencias ni registros de auditoría para los cambios de valor activados por los cambios de configuración de campo. Todos los usuarios que vean los campos verán inmediatamente los nuevos valores con las modificaciones.

   La información de campo se actualiza para todos los que tengan acceso a la vista del espacio de trabajo.

1. (Condicional) Para los campos de registro vinculados, haga clic en **Editar campos de búsqueda** y agregue o quite cualquiera de los campos del tipo de registro vinculado.

   Para obtener más información, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

