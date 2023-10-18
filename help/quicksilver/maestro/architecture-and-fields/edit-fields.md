---
title: Editar campos
description: En Adobe Maestro, puede editar la configuración de los campos que ya se han creado.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Editar campos

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede editar la configuración de campo de los campos que ya se han creado.

Para obtener información sobre la creación de campos Maestro de Adobe, consulte [Creación de campos](../architecture-and-fields/create-fields.md).

Este artículo describe cómo puede editar la configuración de los campos de Maestro. Para obtener información acerca de cómo modificar los valores de los campos de los registros Maestro, consulte [Edición de registros](../records/edit-records.md).

## Consideraciones sobre la edición de información de campo

* Puede editar los campos que ha creado o los campos creados por otros usuarios. <!--this will change with access levels/ permissions-->
* Puede editar un campo en la tabla de tipo de registro.
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
 <tbody>
<td>
   <p> producto de Adobe</p> </td>
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
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <p>Cualquiera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Nivel de acceso</td>
   <td> <p>Cualquiera</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Plantilla de diseño</td>
   <td> <p>El administrador del sistema debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/grant-access.md">Conceder acceso a Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Editar campos

1. Haga clic en **Menú principal** icono ![](assets/main-menu-workfront.png) en la esquina superior derecha de Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> luego haga clic en **Maestro** ![](assets/maestro-icon.png).

   El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo para la que desea eliminar los tipos de registros.

   El espacio de trabajo se abre y se muestran los tipos de registro y las taxonomías asociadas a él.
1. Haga clic en la tarjeta del tipo de registro o de la taxonomía cuyos campos desee editar.

   Se abre la página del tipo de registro.
1. (Condicional) Seleccione una **Vista de tabla** desde el **Ver** menú desplegable en la esquina superior derecha de la página tipo de registro.
1. Pase el ratón sobre el encabezado de columna de un campo que desee editar y, a continuación, haga clic en la flecha hacia abajo situada después del nombre del campo.
1. Clic **Editar campo**, actualice la información del campo y haga clic en **Guardar**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >No se puede actualizar el tipo de campo una vez guardado el campo.


1. (Condicional) Para los campos de registro vinculados, haga clic en **Editar campos de búsqueda** y agregue o quite cualquiera de los campos del tipo de registro vinculado.

   Para obtener más información, consulte [Conectar tipos de registros](../architecture-and-fields/connect-record-types.md).
