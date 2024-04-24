---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Agregar un salto de sección a un formulario personalizado con el generador de formularios heredado
description: Puede agrupar los campos y widgets personalizados en un formulario personalizado en secciones con encabezados. Esto resulta útil para presentar una experiencia organizada a los usuarios que rellenan el formulario. Además, si necesita limitar el acceso a determinados campos personalizados y widgets a determinados usuarios, puede colocarlos en una sección y, a continuación, conceder acceso a la sección únicamente a esos usuarios.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: 28961cda48ce4eec84ed272e660be6ba938be370
workflow-type: tm+mt
source-wordcount: '1238'
ht-degree: 0%

---

# Agregar un salto de sección a un formulario personalizado con el generador de formularios heredado

Puede agrupar los campos y widgets personalizados en un formulario personalizado en secciones con encabezados. Esto resulta útil para presentar una experiencia organizada a los usuarios que rellenan el formulario. Además, si necesita limitar el acceso a determinados campos personalizados y widgets a determinados usuarios, puede colocarlos en una sección y, a continuación, conceder acceso a la sección únicamente a esos usuarios.

Por ejemplo, si necesita realizar el seguimiento de información confidencial que solo los administradores del sistema deben poder ver o editar, puede crear un salto de sección con permisos de Solo administración y colocar los campos confidenciales en esa sección.

La configuración de acceso que seleccione para una sección está directamente vinculada a los permisos que los usuarios tienen en el objeto de Workfront donde está adjunto el formulario personalizado. Puede ocultar o mostrar una sección en función de si el usuario tiene acceso para ver, contribuir o administrar ese objeto. O puede establecer una sección en Solo administrador para que solo los usuarios con un nivel de acceso de administrador del sistema puedan acceder a ella.

Para obtener información sobre los permisos de los objetos, consulte [Información general sobre los permisos de uso compartido en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Agregar un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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
   <td role="rowheader"> <p>plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p></td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Creación y configuración del acceso a una sección de un formulario personalizado

1. Comience a crear o editar un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Agregue campos y widgets personalizados al formulario, tal como se describe en [Agregar un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. Mientras sigue creando o editando el formulario personalizado, en la **Añadir un campo** pestaña, haga clic en **Salto de sección**.

   ![](assets/click-section-break.jpg)

1. En el **Configuración de campo** pestaña, configure las opciones que desee para la sección:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima de la sección. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba texto si desea explicar a los usuarios para qué sirve la sección. Esto se muestra debajo de la etiqueta de la sección en el formulario personalizado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Agregar lógica</p></td> 
      <td><p>Utilice la lógica de visualización para especificar si la sección debe mostrarse en el formulario, en función de las selecciones que realicen los usuarios en los campos personalizados de opción múltiple al rellenar el formulario.</p><p><strong>NOTA:</strong> Si se les ha aplicado lógica de visualización a todos los campos individuales bajo un salto de sección y, como resultado de la lógica, todos ellos están ocultos, toda la sección estará oculta en el formulario personalizado. Esto sucederá incluso si la lógica de visualización no se aplica al salto de sección.</p><p>Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Agregar lógica de visualización y saltar lógica a un formulario personalizado</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Conceder acceso</p> </td> 
      <td> <p> Seleccione los permisos que necesitan los usuarios en un objeto donde se adjunta el formulario personalizado para ver esta sección y editar sus valores de campo.
       <p>Los siguientes permisos están disponibles en <b>Los usuarios con este acceso al objeto pueden ver valores de campo</b>:</p> 
         <ul>
          <li><strong>Ver</strong>: vea los permisos del objeto</li>
          <li><p><b>Edición limitada</b>: (disponible solo si el objeto es un proyecto, una tarea, un problema o un usuario):</p> 
          <p>Permite a los usuarios contribuir al objeto si se trata de un proyecto, una tarea o un problema.</p>
          <p>Permite a los usuarios editar el perfil o poseer el permiso de perfil para el objeto si es un usuario.</p></li> 
          <li><b>Editar</b>: administre permisos al objeto </li> 
          <li><b>Solo administrador</b>: nivel de acceso del administrador del sistema</li> 
         </ul> </li> 
        <p>Los siguientes permisos están disponibles en <b>Los usuarios con este acceso al objeto pueden editar valores de campo</b>: </p> 
         <ul> 
          <li> <p><b>Edición limitada</b>: (disponible solo si el objeto es un proyecto, una tarea, un problema o un usuario):</p> 
           <p>Si el objeto es un proyecto, una tarea o un problema, este permiso permite a los usuarios contribuir al objeto</p>
          <p>Si el objeto es un usuario, este permiso permite a los usuarios editar el perfil o poseer el permiso de perfil para el objeto.</p> 
          <li><b>Editar</b>: administre permisos al objeto </li> 
          <li><b>Solo administrador</b>: nivel de acceso del administrador del sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Para obtener información sobre los permisos de los objetos, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre los permisos de uso compartido en objetos</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Los usuarios sin los permisos especificados aquí no pueden ver los campos y widgets personalizados en la sección. </p> <p>Esto también se aplica si se muestran los valores de los campos en los informes o si se utilizan en campos calculados en los informes en modo de texto.</p> </li>
       <li><p>Para formularios personalizados de solicitud/problema: si se necesita acceso de visualización para ver los campos en el salto de sección, pero se necesita acceso de administrador para editar los campos, los usuarios que no sean administradores no podrán ver la sección y todos sus campos cuando rellenen el formulario. Una vez creada la solicitud, los usuarios con acceso de visualización pueden ver los campos en la sección.</p></li>
       <li> <p>La asociación de varios tipos de objetos con el formulario puede cambiar los permisos de visualización y edición disponibles en estos pasos. Para obtener más información, consulte <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Cómo pueden afectar varios tipos de objetos a los permisos de salto de sección en un formulario personalizado</a> en este artículo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Arrastre o agregue al menos un campo o widget personalizado a la nueva sección.

   Es necesario antes de guardar la sección.

1. Clic **Listo**.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras crea un formulario personalizado para guardar los cambios y mantener el formulario abierto.

1. Si desea seguir creando el formulario personalizado de otras formas, consulte uno de los siguientes artículos:

   * [Agregar un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Añadir datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Colocar campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar lógica de visualización y saltar lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Previsualización y cumplimentación de un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

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

El permiso Editar de forma limitada para saltos de sección de formulario personalizados solo está disponible para los tipos de objeto Proyecto, Tarea, Problema y Usuario.

En un formulario personalizado con un salto de sección configurado con el permiso Editar de forma limitada, si agrega uno de los demás tipos de objetos al formulario (Portfolio, Programa, Documento, Empresa, Registro de facturación, Iteración, Gasto o Grupo), se le pedirá que cambie al permiso Editar, que es compatible tanto con ese tipo de objeto como con los tipos de objeto existentes en el formulario.

>[!INFO]
>
>**Ejemplo:** En un formulario personalizado asociado al tipo de objeto Proyecto, se configura un salto de sección con el permiso Editar de forma limitada.
>
>Se agrega el tipo de objeto Portfolio al formulario, lo que significa que la opción Editar de forma limitada ya no está disponible para el salto de sección del formulario.
>
>Un mensaje en pantalla le pedirá que cambie al permiso Editar, que es la opción más similar a Edición limitada y compatible tanto con el tipo de objeto Proyecto como con el tipo de objeto Portfolio.

