---
title: Editar campos
description: En Adobe Workfront Planning, puede editar la configuración de campo de los campos que ya se han creado. En este artículo se describe cómo editar la configuración de los campos de Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Workfront Planning, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Editar campos

{{planning-important-intro}}

Puede editar la configuración de campo de los campos que ya se han creado en Adobe Workfront Planning.

Para obtener información sobre la creación de campos de Adobe Workfront Planning, consulte [Creación de campos](/help/quicksilver/planning/fields/create-fields.md).

En este artículo se describe cómo editar la configuración de los campos de Workfront Planning. Para obtener información sobre la edición de valores de campo para registros, consulte [Edición de registros](/help/quicksilver/planning/records/edit-records.md).

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
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <p>Cualquiera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuración del nivel de acceso</p></td>
   <td> <p>No hay controles de acceso para Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Editar configuración de campo

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos campos de registro desee editar.

   El espacio de trabajo se abre y todos los tipos de registros del espacio de trabajo se muestran en tarjetas.

1. Haga clic en la tarjeta de un tipo de registro.

   Se abre la página del tipo de registro.

1. (Condicional) Haga clic en la pestaña de un **Vista de tabla**.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.
1. Pase el ratón sobre el encabezado de columna de un campo que desee editar, haga clic en la flecha hacia abajo situada después del nombre del campo y, a continuación, haga clic en **Editar campo**

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

   Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

