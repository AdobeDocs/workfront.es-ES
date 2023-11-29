---
title: Edición de registros
description: Puede editar la información de los registros en Adobe Maestro. Debe crear tipos de registros antes de empezar a crear y editar registros.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 66a4a1e11ff04008d1d0c77fbd6887e8f5f1c46b
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Edición de registros

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para utilizar las funciones de Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede editar la información de los registros en Adobe Maestro. Debe crear tipos de registros antes de empezar a crear y editar registros.
Para obtener más información, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

&lt;!— mencione aquí que los campos de la vista Detalles son los mismos que los de la vista de tabla — este artículo está vinculado desde Administrar vistas de registros a hacer referencia a esta información—>

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

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Consideraciones acerca de la edición de registros

* Puede editar los registros que usted u otro usuario hayan creado. <!--will change with access levels-->
* No se pueden editar campos vinculados desde otros registros o campos que contengan cálculos.
* Si los registros que muestra están vinculados a otros registros, la nueva información de los registros que está modificando se reflejará en los registros vinculados.
* No puede editar registros de forma masiva. <!--this will probably change-->
* Las direcciones URL se reconocen como vínculos en tipos de campo de texto de una sola línea solo cuando comienzan con lo siguiente: http://, https://, ftp:// o www. .
* Puede utilizar las siguientes opciones de formato de texto enriquecido al editar un campo de tipo párrafo:

   * Negrita
   * Cursiva
   * Subrayado
   * Añadir un vínculo
   * Agregar una lista con viñetas
   * Añadir una lista numerada

## Edición de registros

Puede editar un registro desde las siguientes áreas:

* [Desde la página Detalles de un registro](#edit-a-record-from-the-records-details-page)
* [Desde la vista de tabla de un tipo de registro](#edit-a-record-from-the-record-type-table-view)

### Editar un registro desde la página de detalles del registro

1. Haga clic en **Menú principal** ![](assets/main-menu-workfront.png) en la esquina superior derecha, o la **Menú principal** ![](assets/main-menu-shell.png) en la esquina superior izquierda, si está disponible, haga clic en **Maestro**.

   El espacio de trabajo al que se accede por última vez se abre.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.
1. Realice una de las siguientes acciones:

   * En la vista Tabla, haga clic en el nombre de un registro.
   * En la vista Tabla, pase el ratón sobre el nombre de un registro y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Ver**

     ![](assets/contextual-menu-for-record-row.png)
   * En una vista Línea de tiempo, haga clic en una barra de registros.

   El registro **Detalles** se abre la página.

1. Haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre del registro y haga clic en **Editar**

   O

   Haga clic dentro de cualquier campo editable de la página Detalles para editar la información.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Clic **Guardar cambios**. <!--logged a bug for this - this needs to be "Save"-->

### Editar un registro desde la vista de tabla de tipo de registro

1. Haga clic en **Menú principal** ![](assets/main-menu-workfront.png) en la esquina superior derecha, o la **Menú principal** ![](assets/main-menu-shell.png) en la esquina superior izquierda, si está disponible, haga clic en **Maestro** ![](assets/maestro-icon.png).

   Se abre el espacio de trabajo al que accedió por última vez.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.
1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) Desde el **Ver** menú desplegable en la esquina superior derecha de la tabla, seleccione un **Tabla** vista. Esta debe ser la vista predeterminada, a menos que haya visto el tipo de registro en la vista de escala de tiempo cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Haga clic dentro de la fila de un registro para empezar a editar la información sobre el registro en línea.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Prensa **Entrar** en el teclado o haga clic fuera de una fila para guardar los cambios. Los cambios se guardan automáticamente. Un indicador Guardado aparece brevemente en la esquina superior derecha de la vista de tabla para mostrar que los cambios se han guardado.

   >[!NOTE]
   >
   >  No puede editar la información de los siguientes campos, ya que son de solo lectura y Workfront los actualiza automáticamente:
   >  
   >  * Campos vinculados que se crean vinculando tipos de registros
   >  * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación


1. (Opcional) Copie un valor existente de un campo, péguelo en un campo del mismo tipo en otro registro y haga clic en **Entrar** en el teclado para guardar los cambios.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente:
   >
   >* No puede copiar información de otro origen que no sea un campo Maestro del mismo tipo que el campo en el que pega la información.
   >
   >* No se pueden copiar y pegar valores de campo para campos que se muestran en el área Detalles de un registro.
   >* No puede copiar y pegar valores de campo para los siguientes tipos de campo:
   ><ul>
   >
   > * Personas
   >
   > * Campos del sistema
   >
   > * Campos vinculados creados como resultado de la conexión de registros

   <!--take People out of the list above when they release this - this might be coming later-->
