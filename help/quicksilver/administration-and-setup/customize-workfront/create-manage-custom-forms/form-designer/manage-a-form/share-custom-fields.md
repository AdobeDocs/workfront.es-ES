---
title: Configurar el uso compartido para campos y widgets personalizados
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: De forma predeterminada, cuando se añade un nuevo campo personalizado o widget a un formulario personalizado, cualquier usuario del sistema con acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y nombre. Puede cambiar esto controlando con quién se puede compartir.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
source-git-commit: a8e2558469d3abc355eb58f81658db3d1cfc7315
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 66%

---

# Configuración del uso compartido para campos y widgets personalizados

De forma predeterminada, cuando se añade un nuevo campo personalizado o widget a un formulario personalizado, cualquier usuario del sistema con acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y nombre. Puede cambiar esto controlando con quién se puede compartir.

Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

## Configure sharing a custom field or widget from the list of forms

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Click **Fields** to open the Fields area.
1. Select the item you want to configure sharing for, then click ![Share icon](assets/share-icon.png).
1. In the Custom Field Access box that displays, specify who you want to share the item with and how you want to share it:

   1. Near the lower-left corner of the **Custom Field Access** box, under **Give custom field access to**, start typing the name of a user, team, job role, group, or company you want to share the item with, then click the name when it appears.

      ![Custom Field Access box](assets/share-field-give-access-to.jpg)

   1. If you want to be more specific about how you want to share the item, click the drop-down list to the right of the name, then use any of the following options:

      ![Sharing options](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">View it</td> 
         <td> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to add the item to a custom form or share it with other users.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Manage it</td> 
         <td> <p>Allows access to edit the custom field and to see it in the Field Library and on the page where you build custom forms.</p> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to delete the item from the system or share it with other users.</p> </td> 
        </tr> 
       </tbody> 
      </table>   

1. (Optional) Repeat the previous step to add other names to the list and configure their options.
1. (Optional) Click the gear icon ![Settings icon](assets/gear-icon-settings.png) in the top-right corner if you want to choose a system-wide sharing option for the field.

   Not all of the following options display in this drop-down menu at the same time. For example, the second one displays only when one of the other two are selected.

   * **Make this editable system-wide so that everyone in Workfront can edit it** (the default option)

     When you add a custom field or widget and you don't limit sharing for it, everyone in the system who has access to custom forms can view it and edit its properties.
   
   * **Remove system-wide edit access**

     Limits access to only those whom you added to the list. 
   
   * **Make this visible system-wide so that everyone in Workfront can see it**

1. Click **Save**.

-->

## Configurar el uso compartido de un campo o widget personalizado

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Formularios personalizados**.
1. Para compartir desde la lista de formularios y campos:

   1. Haga clic en **Campos** para abrir el área Campos.
   1. Seleccione el campo que desea compartir y luego haga clic en ![icono Compartir](assets/share-icon.png).

1. Para compartir desde el diseñador de formularios:
   1. Abra un formulario personalizado o cree uno nuevo.
   1. En el diseñador de formularios, seleccione el campo que desee compartir y, a continuación, haga clic en **Compartir** en el área de edición de campos de la derecha.

1. En el cuadro para compartir, en **Conceder acceso al campo a**, empiece a escribir el nombre del usuario, equipo, rol, grupo, compañía o perfil empresarial con el que desea compartir el elemento y, a continuación, presione **Entrar** cuando se muestre el nombre.
1. Si desea ser más específico sobre cómo comparte el elemento, haga clic en el menú desplegable situado a la derecha del nombre y, a continuación, utilice cualquiera de las siguientes opciones:

   * **Ver**: haga clic en el icono de **Configuración avanzada** ![Configuración avanzada](assets/configure-options-icon.png) para especificar si desea que los usuarios puedan agregar el elemento a un formulario personalizado o compartirlo con otros usuarios.
   * **Administrar**: permite el acceso para editar el campo personalizado y verlo tanto en la biblioteca de campos como en el diseñador de formularios. Haga clic en el icono de **Configuración avanzada** ![Configuración avanzada](assets/configure-options-icon.png) para especificar si desea que los usuarios puedan eliminar el elemento del sistema o compartirlo con otros usuarios.

1. (Opcional) Repita los pasos del 5 al 6 para añadir otros nombres a la lista y configurar sus opciones.
1. (Opcional) Elija una opción de uso compartido en todo el sistema para el campo:

   * **Todos los usuarios del sistema pueden editar** (la opción predeterminada)

     Cuando se añade un campo o widget personalizado y no se limita el uso compartido, todos los usuarios del sistema que tengan acceso a los formularios personalizados pueden verlo y editar sus propiedades.

   * **Todos los usuarios del sistema pueden ver**

     Todas las personas del sistema que tengan acceso a los formularios personalizados pueden ver el campo, pero no editarlo.

   * **Solo las personas invitadas pueden tener acceso**

     Limita el acceso únicamente a las personas añadidas a la lista.

   ![Opciones de uso compartido](assets/share-field-in-designer.png)

1. Haga clic en **Guardar**.

## Acceso heredado a campos y widgets personalizados cuando se comparte un formulario personalizado

Cuando alguien comparte un formulario personalizado con un grupo, un rol, un equipo, una compañía o un perfil empresarial, los destinatarios heredan el acceso de Ver a cualquier campo personalizado y widget que esté en el formulario. Este nivel de acceso a los elementos del formulario se conserva siempre para que el formulario pueda funcionar para los destinatarios, tal y como lo concibió la persona que lo creó. Esto es así incluso para los destinatarios que tienen acceso de edición al formulario.

Puede averiguar quién ha heredado el acceso a un campo o widget personalizado y puede quitarle el acceso.

>[!NOTE]
>
>Si un destinatario tiene acceso de administración a un campo o widget personalizado en el formulario personalizado compartido, dicho acceso se conserva para el destinatario.

### Descubra quién ha heredado el acceso a un campo o widget personalizado {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Formularios personalizados**.
1. Haga clic en **Campos** y luego seleccione el campo, la imagen o el widget de acceso.
1. En el cuadro que se muestra, haga clic en **Permisos heredados** y vea los nombres que se muestran.
1. Haga clic en **Cancelar**.

### Eliminar el acceso a un campo o widget personalizado de un formulario personalizado que se haya compartido {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Si necesita eliminar el acceso a un campo o widget personalizado en un formulario personalizado que se compartió, debe anular el uso compartido del formulario. Para obtener instrucciones, consulte la sección [Quitar el acceso a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form) en el artículo [Compartir un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).


