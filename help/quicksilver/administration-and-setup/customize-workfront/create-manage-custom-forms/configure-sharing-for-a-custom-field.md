---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configure el uso compartido de campos personalizados y widgets con el generador de formularios heredado
description: De forma predeterminada, cuando se agrega un nuevo campo personalizado o widget a un formulario personalizado, cualquier persona en el sistema con acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y nombre. Puede cambiar esto controlando con quién se puede compartir.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: df6b1e4b362807025f3edb5298e8445c0d44ec69
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Configure el uso compartido de campos personalizados y widgets con el generador de formularios heredado

De forma predeterminada, cuando se agrega un nuevo campo personalizado o widget a un formulario personalizado, cualquier persona en el sistema con acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y nombre. Puede cambiar esto controlando con quién se puede compartir.

Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Agregar un campo personalizado a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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
   <p>o</p>
   <p>Actual: plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Configuración del uso compartido para un campo o widget personalizado

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Si está configurando el uso compartido de un campo o widget personalizado en la instancia de Workfront de su organización, haga lo siguiente:

   1. Clic **Campos** para abrir el área Campos.
   1. Seleccione el elemento para el que desea configurar el uso compartido y haga clic en ![Icono Compartir](assets/share-icon.png).

   O bien, si está configurando el uso compartido de un campo o widget personalizado en un formulario personalizado existente, haga lo siguiente:

   1. Seleccione el formulario personalizado y haga clic en ![Icono Editar](assets/edit-icon.png).
   1. En el área de edición del formulario de la derecha, seleccione el elemento para el que desea configurar el uso compartido.
   1. En el panel izquierdo, haga clic en **Compartir campo**.

1. En el **Acceso a campos personalizados** , especifique con quién desea compartir el elemento y cómo desea compartirlo:

   1. Cerca de la esquina inferior izquierda del **Acceso a campos personalizados** cuadro, debajo de **Conceder acceso a campo personalizado a**, empiece a escribir el nombre de un usuario, equipo, función del puesto, grupo o empresa con el que desee compartir el elemento y, a continuación, haga clic en el nombre cuando aparezca.

      ![](assets/share-field-give-access-to.jpg)

   1. Si desea ser más específico sobre cómo desea compartir el elemento, haga clic en la lista desplegable situada a la derecha del nombre y, a continuación, utilice cualquiera de las siguientes opciones:

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Verlo</td> 
         <td> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan utilizar su acceso para agregar el elemento a un formulario personalizado o compartirlo con otros usuarios.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Administrarlo</td> 
         <td> <p>Permite acceder para editar el campo personalizado y verlo en la biblioteca de campos y en la página donde se generan los formularios personalizados.</p> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan utilizar su acceso para eliminar el elemento del sistema o compartirlo con otros usuarios.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Opcional) Repita el paso anterior para agregar otros nombres a la lista y configurar sus opciones.
1. (Opcional) Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en la esquina superior derecha si desea elegir una opción de uso compartido para todo el sistema para el campo.

   No todas las opciones siguientes se muestran en este menú desplegable al mismo tiempo. Por ejemplo, el segundo solo se muestra cuando se selecciona uno de los otros dos.

   * **Convertirlo en editable en todo el sistema para que todos los usuarios de Workfront puedan editarlo** (la opción predeterminada)

     Cuando se agrega un campo o widget personalizado y no se limita el uso compartido, todos los usuarios del sistema que tengan acceso a los formularios personalizados pueden verlo y editar sus propiedades.

   * **Eliminar acceso de edición en todo el sistema**

     Limita el acceso únicamente a las personas agregadas a la lista.

   * **Convertirlo en visible en todo el sistema para que todos los usuarios de Workfront puedan verlo**

1. Clic **Guardar** o **Guardar + Cerrar**.

## Acceso heredado a campos y widgets personalizados cuando se comparte un formulario personalizado

Cuando alguien comparte un formulario personalizado con un grupo, una función del trabajo, un equipo o una empresa, los destinatarios heredan el acceso de Ver a cualquier campo personalizado y widget que esté en el formulario. Este nivel de acceso a los elementos del formulario siempre se conserva para que el formulario pueda funcionar para los destinatarios según lo previsto por la persona que lo creó. Esto ocurre incluso para los destinatarios que tienen acceso de edición al formulario.

Puede averiguar quién ha heredado el acceso a un campo o widget personalizado y puede quitar el acceso a él.

>[!NOTE]
>
>Si un destinatario tiene acceso de Administración a un campo o widget personalizado en el formulario personalizado compartido, ese acceso se conserva para el destinatario.

* [Descubra quién ha heredado el acceso a un campo o widget personalizado](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Eliminar el acceso a un campo o widget personalizado de un formulario personalizado que se haya compartido](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Descubra quién ha heredado el acceso a un campo o widget personalizado {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Clic **Campos**, luego seleccione el campo, la imagen o el widget de acceso.
1. En el cuadro que aparece, haga clic en **Permisos heredados** y vea los nombres que se muestran.
1. Clic **Cancelar**.

### Eliminar el acceso a un campo o widget personalizado de un formulario personalizado que se haya compartido {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Si necesita eliminar el acceso a un campo o widget personalizado en un formulario personalizado que se compartió, debe dejar de compartir el formulario. Para obtener instrucciones, consulte en la sección [Eliminar el acceso a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) en el artículo [Compartir un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
