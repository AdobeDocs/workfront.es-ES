---
title: Configurar el uso compartido para campos y widgets personalizados
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: De forma predeterminada, cuando se agrega un nuevo campo personalizado o widget a un formulario personalizado, cualquier persona en el sistema con acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y nombre. Puede cambiar esto controlando con quién se puede compartir.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 1%

---

# Configuración del uso compartido para campos y widgets personalizados

De forma predeterminada, cuando se agrega un nuevo campo personalizado o widget a un formulario personalizado, cualquier persona en el sistema con acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y nombre. Puede cambiar esto controlando con quién se puede compartir.

Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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

+++

## Configure el uso compartido de un campo o widget personalizado desde la lista de formularios

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Haga clic en **Campos** para abrir el área Campos.
1. Seleccione el elemento para el que desea configurar el uso compartido y, a continuación, haga clic en ![Icono de compartir](assets/share-icon.png).
1. En el cuadro Acceso a campos personalizados que aparece, especifique con quién desea compartir el elemento y cómo desea compartirlo:

   1. Cerca de la esquina inferior izquierda del cuadro **Acceso a campos personalizados**, en **Dar acceso a campos personalizados a**, empiece a escribir el nombre de un usuario, equipo, rol, grupo o compañía con el que desee compartir el elemento y, a continuación, haga clic en el nombre cuando aparezca.

      ![Cuadro de acceso a campo personalizado](assets/share-field-give-access-to.jpg)

   1. Si desea ser más específico sobre cómo desea compartir el elemento, haga clic en la lista desplegable situada a la derecha del nombre y, a continuación, utilice cualquiera de las siguientes opciones:

      ![Opciones de uso compartido](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">Verlo</td> 
         <td> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan usar su acceso para agregar el elemento a un formulario personalizado o compartirlo con otros usuarios.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Administrarlo</td> 
         <td> <p>Permite acceder para editar el campo personalizado y verlo en la biblioteca de campos y en la página donde se generan los formularios personalizados.</p> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan usar su acceso para eliminar el elemento del sistema o compartirlo con otros usuarios.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Opcional) Repita el paso anterior para agregar otros nombres a la lista y configurar sus opciones.
1. (Opcional) Haga clic en el icono de engranaje ![Icono de configuración](assets/gear-icon-settings.png) en la esquina superior derecha si desea elegir una opción de uso compartido en todo el sistema para el campo.

   No todas las opciones siguientes se muestran en este menú desplegable al mismo tiempo. Por ejemplo, el segundo solo se muestra cuando se selecciona uno de los otros dos.

   * **Haga que esto se pueda editar en todo el sistema para que todos los usuarios de Workfront puedan editarlo** (la opción predeterminada)

     Cuando se agrega un campo o widget personalizado y no se limita el uso compartido, todos los usuarios del sistema que tengan acceso a los formularios personalizados pueden verlo y editar sus propiedades.

   * **Quitar acceso de edición en todo el sistema**

     Limita el acceso únicamente a las personas agregadas a la lista.

   * **Haga esto visible en todo el sistema para que todos los usuarios de Workfront puedan verlo**

1. Haga clic en **Guardar**.

## Configurar el uso compartido de un campo o widget personalizado desde el diseñador de formularios

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Abra un formulario personalizado o cree uno nuevo.
1. En el diseñador de formularios, seleccione el elemento para el que desea configurar el uso compartido y, a continuación, haga clic en **Compartir** en el área de edición de campos de la derecha.
1. En el cuadro que aparece, en **Conceder acceso a formulario personalizado a**, empiece a escribir el nombre del usuario, equipo, rol, grupo o compañía con el que desea compartir el elemento y, a continuación, presione **Entrar** cuando se muestre el nombre.
1. Si desea ser más específico sobre cómo comparte el elemento, haga clic en el menú desplegable situado a la derecha del nombre y, a continuación, utilice cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Verlo</td> 
        <td> <p>Haga clic en <strong>Configuración avanzada</strong> para especificar si desea que los usuarios puedan agregar el elemento a un formulario personalizado o compartirlo con otros usuarios.</p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Administrarlo</td> 
        <td> <p>Permite acceder para editar el campo personalizado y verlo tanto en la biblioteca de campos como en el diseñador de formularios.</p> <p>Haga clic en <strong>Configuración avanzada</strong> para especificar si desea que los usuarios puedan eliminar el elemento del sistema o compartirlo con otros usuarios.</p> </td> 
       </tr> 
     </tbody> 
    </table>

1. (Opcional) Repita los pasos 5-6 para añadir otros nombres a la lista y configurar sus opciones.
1. (Opcional) Elija una opción de uso compartido en todo el sistema para el campo:

   * **Todos los usuarios del sistema pueden editar** (la opción predeterminada)

     Cuando se agrega un campo o widget personalizado y no se limita el uso compartido, todos los usuarios del sistema que tengan acceso a los formularios personalizados pueden verlo y editar sus propiedades.

   * **Todos los usuarios del sistema pueden ver**
   * **Solo las personas invitadas pueden acceder**

     Limita el acceso únicamente a los que agregó a la lista.

   ![Opciones de uso compartido](assets/share-field-in-designer.png)

1. Haga clic en **Guardar**.

## Acceso heredado a campos y widgets personalizados cuando se comparte un formulario personalizado

Cuando alguien comparte un formulario personalizado con un grupo, una función del trabajo, un equipo o una empresa, los destinatarios heredan el acceso de Ver a cualquier campo personalizado y widget que esté en el formulario. Este nivel de acceso a los elementos del formulario siempre se conserva para que el formulario pueda funcionar para los destinatarios según lo previsto por la persona que lo creó. Esto ocurre incluso para los destinatarios que tienen acceso de edición al formulario.

Puede averiguar quién ha heredado el acceso a un campo o widget personalizado y puede quitar el acceso a él.

>[!NOTE]
>
>Si un destinatario tiene acceso de Administración a un campo o widget personalizado en el formulario personalizado compartido, ese acceso se conserva para el destinatario.

### Descubra quién ha heredado el acceso a un campo o widget personalizado {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Haga clic en **Campos** y luego seleccione el campo, la imagen o el widget de acceso.
1. En el cuadro que se muestra, haga clic en **Permisos heredados** y vea los nombres que se muestran.
1. Haga clic en **Cancelar**.

### Eliminar el acceso a un campo o widget personalizado de un formulario personalizado que se haya compartido {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Si necesita eliminar el acceso a un campo o widget personalizado en un formulario personalizado que se compartió, debe dejar de compartir el formulario. Para obtener instrucciones, consulte la sección [Quitar el acceso a un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form-from-the-list-of-forms) en el artículo [Compartir un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
