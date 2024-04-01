---
title: Editar campos
description: En Adobe Workfront Planning, puede editar la configuración de campo de los campos que ya se han creado.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# Editar campos

{{maestro-important-intro}}

Puede editar la configuración de campo de los campos que ya se han creado en Adobe Workfront Planning.

Para obtener información sobre la creación de campos de Adobe Workfront Planning, consulte [Creación de campos](../fields/create-fields.md).

En este artículo se describe cómo editar la configuración de los campos de Workfront Planning. Para obtener información sobre la edición de valores de campo para registros, consulte [Edición de registros](/help/quicksilver/maestro/records/edit-records.md).

## Consideraciones sobre la edición de información de campo

* Puede editar los campos que ha creado o los campos creados por otros usuarios si tiene permisos de administración en el espacio de trabajo al que pertenecen los campos.
* Puede editar un campo en la tabla de tipo de registro.
* No se puede editar un campo en la página de registro o en la vista de escala de tiempo.
* Una vez guardado el campo, no se puede editar el tipo de campo.
* No puede anular la selección de la opción Permitir números negativos seleccionada anteriormente para un campo Número, Porcentaje o Moneda si ya hay valores negativos almacenados en los registros a los que está asociada.
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
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
<p>Su organización debe estar inscrita en el programa beta de Adobe Workfront Planning. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
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
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Editar campos

{{step1-to-maestro}}

    El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo para la que desea eliminar los tipos de registros.

   Se abre el espacio de trabajo y se muestran los tipos de registro asociados a él.
1. Haga clic en la tarjeta del tipo de registro cuyos campos desee editar.

   Se abre la página del tipo de registro.
1. (Condicional) Seleccione una **Vista de tabla** desde el **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.
1. Pase el ratón sobre el encabezado de columna de un campo que desee editar, haga clic en la flecha hacia abajo situada después del nombre del campo y, a continuación, haga clic en **Editar campo**

   O

   Haga doble clic en el encabezado de columna del campo.

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Actualice la información sobre el campo y haga clic en **Guardar**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >No se puede actualizar el tipo de campo una vez guardado el campo.


1. (Condicional) Para los campos de registro vinculados, haga clic en **Editar campos de búsqueda** y agregue o quite cualquiera de los campos del tipo de registro vinculado.

   Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).
