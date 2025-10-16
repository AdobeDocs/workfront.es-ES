---
title: Editar configuración de campo
description: En Adobe Workfront Planning, puede editar la configuración de campo de los campos que ya se han creado. En este artículo se describe cómo editar la configuración de los campos de Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 48%

---


# Editar configuración de campo

<!--leave the choice value information in yellow till January 2026-->

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Puede editar la configuración de los campos existentes en Adobe Workfront Planning.

Para obtener información sobre la creación de campos de Adobe Workfront Planning, consulte [Creación de campos](/help/quicksilver/planning/fields/create-fields.md).

En este artículo se describe cómo editar la configuración de los campos de Workfront Planning. Para obtener información sobre cómo editar los valores de campo de los registros, consulte [Edición de registros](/help/quicksilver/planning/records/edit-records.md).

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
   <td role="rowheader"><p>paquete de Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Cualquier Workfront y cualquier paquete de Planning</p></li>
O
<li><p>Cualquier flujo de trabajo y cualquier paquete de Planning</p></li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++     

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Consideraciones sobre la edición de configuración de campo

Debe tener en cuenta lo siguiente antes de realizar cambios en la configuración de un campo:

* La configuración de campos solo se puede editar desde la tabla de tipo de registro.
* No se puede editar la configuración de un campo en la página de registro o en cualquier otra vista, fuera de la vista de tabla.
* Una vez guardado el campo, no puede editar el tipo de campo.
* No puede anular la selección de la opción Permitir números negativos seleccionada anteriormente para un campo Número, Porcentaje o Moneda, si ya hay valores negativos almacenados en los registros a los que está asociada.
* Sí puede editar la configuración de los siguientes elementos de campo después de guardar el campo:

   * El nombre o la descripción de cualquier campo
   * Las opciones de un campo de selección única o de selección múltiple.
   * La expresión de un campo de fórmula.

  >[!WARNING]
  >
  >Cuando cambian las expresiones de fórmula, o se añaden o eliminan opciones de un campo de tipo de selección, se perderán datos de los registros que ya tienen información almacenada en los campos cuya configuración se modifica.
  >
  >No se muestra ninguna advertencia ni indicación de que esta pérdida de datos pueda producirse al cambiar la configuración de los campos.
  >
  >No se muestra ninguna notificación a otros usuarios de que la configuración del campo haya cambiado.

* Puede editar los campos de búsqueda existentes de los registros conectados.
* Además de editar el campo como se describe en la sección [Editar configuración de campo](#edit-field-settings-1) de este artículo, <span class="preview">puede editar las opciones de un campo de selección única o múltiple cuando edita un registro en la vista de tabla, a medida que actualiza los valores de los campos. Para obtener más información, vea la sección [Agregar nuevas opciones a un campo de selección existente al editar registros en la vista de tabla](#add-new-choices-to-an-existing-select-field-when-editing-records-in-the-table-view) de este artículo.</span>

<!--at production - April 10, 2025 - remove the last bullet altogether-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

## Editar configuración de campo

{{step1-to-planning}}

1. Haga clic en el espacio de trabajo cuyos campos de registro desee editar.

   El espacio de trabajo se abre y todos los tipos de registros del espacio de trabajo se muestran en tarjetas.

1. Haga clic en la tarjeta de un tipo de registro.

   Se abre la página del tipo de registro.

1. (Condicional) Haga clic en la pestaña de una **vista de tabla**.

   Todos los registros existentes asociados al tipo de registro se muestran en las filas de la vista de tabla.
1. Pase el puntero por encima del encabezado de columna del campo que desee editar, a continuación haga clic en la flecha que apunta hacia abajo detrás del nombre del campo y por último haga clic en **Editar campo**

   O

   Haga doble clic en el encabezado de columna del campo.

   ![Menú de flecha después del nombre del campo en el encabezado de tabla resaltado](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. Actualice la información sobre el campo y haga clic en **Guardar**.

   Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >* Una vez guardado el campo, no puede actualizar el tipo de campo.
   >
   >* Al modificar las configuraciones de campo (opciones de campo o expresiones de fórmula), los registros que ya contienen información en los campos modificados actualizarán sus valores en tiempo real. No se muestran advertencias ni registros de auditoría para los cambios de valor activados por los cambios en la configuración del campo. Todos los usuarios que vean los campos verán inmediatamente los nuevos valores con las modificaciones.

   La información de campo se actualiza para todos los que tengan acceso a la vista del espacio de trabajo.

1. (Condicional) Para los campos de registro conectados, haga clic en **Editar campos de búsqueda** y agregue o quite cualquiera de los campos de búsqueda del tipo de registro conectado.

   Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).


<div class="preview">

## Agregar nuevas opciones a un campo de selección existente al editar registros en la vista de tabla

<!--some of this information is also available in Edit records article - update both when necessary-->

Puede agregar nuevas opciones a un campo de selección única o múltiple existente al editar registros en la vista de tabla.

>[!IMPORTANT]
>
>La funcionalidad descrita en esta sección solo está disponible en la vista de tabla. No está disponible en ninguna otra área en la que se muestren campos de selección única o múltiple.

**EJEMPLO**

Puede tener un campo de selección único llamado Estado que tiene las opciones Nuevo y Cerrado, y desea agregar una opción para un estado En curso. Puede agregar la opción realizando una de las siguientes acciones:

* Edición del campo. Para obtener más información, consulte la sección [Editar configuración de campo](#edit-field-settings-1) en este artículo.
* Agregar una nueva opción mientras se edita el registro en la vista de tabla, como se describe a continuación.

Para agregar una nueva opción a un campo de selección existente al editar un registro:

1. Vaya a una página de tipo de registro y abra la vista de tabla.
1. Agregue el campo de selección única o múltiple al que desee agregar una opción en la vista de tabla como una nueva columna. Para obtener más información, consulte [Crear campos](/help/quicksilver/planning/fields/create-fields.md).
1. Comience a editar el campo en línea haciendo doble clic en la celda del campo.
1. Escriba el nombre de la opción que desea agregar y haga clic en **Agregar opción**.

   ![Agregar opción en un campo de selección única en la vista de tabla](assets/add-choice-in-table-view-for-single-select-field.png)

   La nueva opción se agrega inmediatamente al campo de selección única.

   <!--<span class="preview">A new choice value is also added to each choice. You can use the choice values in API calls or other integrations. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). </span>-->

</div>