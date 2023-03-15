---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Agregar un salto de sección a un formulario personalizado con el generador de formularios heredado
description: Puede agrupar los campos personalizados y las utilidades de un formulario personalizado en secciones con encabezados. Esto resulta útil para presentar una experiencia organizada a los usuarios que rellenen el formulario. Además, si necesita limitar el acceso a ciertos campos y utilidades personalizados a ciertos usuarios, puede colocarlos en una sección y, a continuación, conceder acceso a la sección únicamente a esos usuarios.
feature: System Setup and Administration
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 0%

---

# Agregar un salto de sección a un formulario personalizado con el generador de formularios heredado

Puede agrupar los campos personalizados y las utilidades de un formulario personalizado en secciones con encabezados. Esto resulta útil para presentar una experiencia organizada a los usuarios que rellenen el formulario. Además, si necesita limitar el acceso a ciertos campos y utilidades personalizados a ciertos usuarios, puede colocarlos en una sección y, a continuación, conceder acceso a la sección únicamente a esos usuarios.

Por ejemplo, si necesita realizar un seguimiento de la información confidencial que solo los administradores del sistema deben poder ver o editar, puede crear un salto de sección con los permisos Solo administrador y colocar los campos confidenciales en esa sección.

La configuración de acceso que seleccione para una sección está directamente vinculada a los permisos que los usuarios tienen en el objeto Workfront al que está adjunto el formulario personalizado. Puede ocultar o mostrar una sección en función de si el usuario tiene acceso para ver, contribuir o administrar ese objeto. O puede establecer una sección en Solo administración para que solo puedan acceder a ella los usuarios con un nivel de acceso de administrador del sistema.

Para obtener información sobre los permisos de los objetos, consulte [Información general sobre cómo compartir permisos en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obtener información sobre los campos personalizados y las utilidades de los formularios personalizados, consulte [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear y configurar el acceso a una sección en un formulario personalizado

1. Comience a crear o editar un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Agregue campos personalizados y utilidades al formulario, tal como se describe en [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. Mientras se sigue creando o editando el formulario personalizado, en la **Añadir un campo** , haga clic en **Salto de sección**.

   ![](assets/click-section-break.jpg)

1. En el **Configuración de campos** , configure las opciones que desee para la sección :

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima de la sección. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: Evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba texto si desea explicar a los usuarios para qué es la sección. Se muestra debajo de la etiqueta de la sección en el formulario personalizado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agregar lógica</td> 
      <td>Utilice la lógica de visualización para especificar si la sección debe mostrarse en el formulario, en función de las selecciones que los usuarios realicen en campos personalizados de varias opciones cuando rellenen el formulario. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Agregar lógica de visualización y de omisión de lógica a un formulario personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Conceder acceso</p> </td> 
      <td> <p> Seleccione los permisos que necesitan los usuarios en un objeto al que esté adjunto el formulario personalizado para ver esta sección y editar sus valores de campo. 
       <p>Los siguientes permisos están disponibles en <b>Los usuarios con este acceso al objeto pueden ver los valores de los campos</b>:</p> 
         <ul>  
          <li><p><b>Edición limitada</b>: (Disponible solo si el objeto es un proyecto, una tarea, un problema o un usuario):</p> 
          <p>Permite a los usuarios contribuir al objeto si se trata de un proyecto, una tarea o un problema.</p>
          <p>Permite a los usuarios editar el perfil o poseer el permiso de perfil del objeto si se trata de un usuario.</p></li> 
          <li><b>Editar</b>: Administrar permisos en el objeto </li> 
          <li><b>Solo administrador</b>: Nivel de acceso del administrador del sistema</li> 
         </ul> </li> 
        <p>Los siguientes permisos están disponibles en <b>Los usuarios con este acceso al objeto pueden editar los valores de los campos</b>: </p> 
         <ul> 
          <li> <p><b>Edición limitada</b>: (Disponible solo si el objeto es un proyecto, una tarea, un problema o un usuario):</p> 
           <p>Si el objeto es un proyecto, una tarea o un problema, este permiso permite a los usuarios contribuir al objeto</p>
          <p>Si el objeto es un usuario, este permiso permite a los usuarios editar el perfil o poseer el permiso de perfil del objeto.</p> 
          <li><b>Editar</b>: Administrar permisos en el objeto </li> 
          <li><b>Solo administrador</b>: Nivel de acceso del administrador del sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Para obtener información sobre los permisos de los objetos, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre cómo compartir permisos en objetos</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Los usuarios sin los permisos especificados aquí no pueden ver los campos personalizados y las utilidades de la sección . </p> <p>Esto también ocurre si se muestran los valores de los campos en los informes o se utilizan en campos calculados en los informes de modo de texto.</p> </li> 
       <li> <p>La asociación de varios tipos de objetos con el formulario puede cambiar los permisos de visualización y edición disponibles en estos pasos. Para obtener más información, consulte <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Cómo pueden afectar varios tipos de objetos a los permisos de salto de sección en un formulario personalizado</a> en este artículo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Arrastre o agregue al menos un campo o widget personalizado a la nueva sección.

   Esto es necesario antes de guardar la sección.

1. Haga clic en **Listo**.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras esté creando un formulario personalizado para guardar los cambios y mantener el formulario abierto.

1. Si desea seguir creando el formulario personalizado de otras formas, continúe con uno de los siguientes artículos:

   * [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Colocación de campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar lógica de visualización y de omisión de lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Obtener una vista previa y completar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## Cómo pueden afectar varios tipos de objetos a los permisos de salto de sección {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

Los saltos de sección de permisos de edición limitada para formularios personalizados solo están disponibles para los tipos de objeto Proyecto, Tarea, Problema y Usuario.

En un formulario personalizado con un salto de sección configurado con el permiso de edición limitada, si agrega uno de los otros tipos de objeto al formulario (Portfolio, Programa, Documento, Empresa, Registro de Facturación, Iteración, Gastos o Grupo), se le pedirá que cambie al permiso de edición, que es compatible tanto con ese tipo de objeto como con los tipos de objeto existentes en el formulario.

>[!INFO]
>
>**Ejemplo:** En un formulario personalizado asociado con el tipo de objeto Project , se configura un salto de sección con el permiso de edición limitada.
>
>El tipo de objeto Portfolio se agrega al formulario, lo que significa que la opción de permiso Editar limitado ya no está disponible para el salto de sección del formulario.
>
>Un mensaje en pantalla le pedirá que cambie al permiso de edición, que es la opción más similar a Edición limitada, y compatible tanto con el tipo de objeto Project como con el tipo de objeto de Portfolio.
