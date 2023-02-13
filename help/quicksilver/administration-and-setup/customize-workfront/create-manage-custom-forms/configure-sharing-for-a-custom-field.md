---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Configuración del uso compartido para campos personalizados y widgets
description: De forma predeterminada, cuando se agrega un nuevo campo o widget personalizado a un formulario personalizado, cualquier usuario del sistema que tenga acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y nombre. Puede cambiar esto controlando con quién se puede compartir.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '943'
ht-degree: 2%

---

# Configuración del uso compartido para campos personalizados y widgets

De forma predeterminada, cuando se agrega un nuevo campo o widget personalizado a un formulario personalizado, cualquier usuario del sistema que tenga acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y nombre. Puede cambiar esto controlando con quién se puede compartir.

Para obtener información sobre los campos personalizados y las utilidades de los formularios personalizados, consulte [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Configuración del uso compartido para un campo o una utilidad personalizados

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Si está configurando el uso compartido para un campo o widget personalizado en la instancia de Workfront de su organización, haga lo siguiente:

   1. Haga clic en el **Campos** pestaña .
   1. Seleccione el elemento para el que desea configurar el uso compartido y, a continuación, haga clic en **Compartir**.

   O, si está configurando el uso compartido de un campo o widget personalizado en un formulario personalizado existente, haga lo siguiente:

   1. Seleccione el formulario personalizado y haga clic en **Editar**.
   1. En el área de edición de formularios de la derecha, seleccione el elemento para el que desea configurar el uso compartido.
   1. En el panel izquierdo, haga clic en **Campo Compartir**.


1. En el **Acceso a campos personalizados** que se muestra, especifique con quién desea compartir el elemento y cómo desea compartirlo:

   1. Cerca de la esquina inferior izquierda del **Acceso a campos personalizados** en **Proporcionar acceso de campo personalizado a**, empiece a escribir el nombre de un usuario, equipo, función de trabajo, grupo o empresa con el que desee compartir el elemento y, a continuación, haga clic en el nombre cuando aparezca.

      ![](assets/share-field-give-access-to.jpg)

   1. Si desea ser más específico sobre cómo desea compartir el elemento, haga clic en la lista desplegable a la derecha del nombre y, a continuación, utilice cualquiera de las siguientes opciones:

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
         <td> <p>Permite editar el campo personalizado y verlo en la Biblioteca de campos y en la página donde se generan formularios personalizados.</p> <p>Puede hacer clic en <strong>Configuración avanzada</strong> para especificar si desea que el usuario o los usuarios puedan utilizar su acceso para eliminar el elemento del sistema o compartirlo con otros usuarios.</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. (Opcional) Repita el paso anterior para agregar otros nombres a la lista y configurar sus opciones.
1. (Opcional) Haga clic en el icono de engranaje ![](assets/gear-icon-settings.png) en la esquina superior derecha si desea elegir una opción de uso compartido en todo el sistema para el campo .

   No todas las opciones siguientes aparecen en este menú desplegable al mismo tiempo. Por ejemplo, el segundo solo se muestra cuando se selecciona uno de los otros dos.

   * **Haga que esto se pueda editar en todo el sistema para que todos en Workfront puedan editarlo** (la opción predeterminada)

      Cuando agrega un campo o widget personalizado y no limita el uso compartido para él, todos los miembros del sistema que tengan acceso a formularios personalizados pueden verlo y editar sus propiedades.

   * **Eliminar acceso de edición en todo el sistema**

      Limita el acceso solo a aquellos a los que añadió a la lista.

   * **Hacer esto visible en todo el sistema para que cualquier usuario de Workfront lo pueda ver**

1. Haga clic en **Guardar** o **Guardar + Cerrar**.

## Acceso heredado a campos personalizados y utilidades cuando se comparte un formulario personalizado

Cuando alguien comparte un formulario personalizado con un grupo, una función de trabajo, un equipo o una empresa, los destinatarios heredan Ver acceso a cualquier campo y widget personalizados que haya en el formulario. Este nivel de acceso a esos elementos del formulario siempre se conserva para que el formulario pueda funcionar para los destinatarios según lo previsto por la persona que lo creó. Esto ocurre incluso en los destinatarios que tienen acceso de edición al formulario.

Puede averiguar quién ha heredado el acceso a un campo o widget personalizado y puede eliminar el acceso a él.

>[!NOTE]
>
>Si un destinatario tiene acceso de gestión a un campo o widget personalizado del formulario personalizado compartido, ese acceso se retiene para el destinatario.

* [Averigüe quién ha heredado el acceso a un campo o widget personalizado](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [Eliminar el acceso a un campo o widget personalizado en un formulario personalizado compartido](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### Averigüe quién ha heredado el acceso a un campo o widget personalizado {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Haga clic en el **Campos** y, a continuación, seleccione el campo, la imagen o el widget de acceso.
1. En el cuadro que aparece, haga clic en **Permisos heredados** y vea los nombres que aparecen.
1. Haga clic en **Cancelar**.

### Eliminar el acceso a un campo o widget personalizado en un formulario personalizado compartido {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Si necesita quitar el acceso a un campo o widget personalizado en un formulario personalizado compartido, debe dejar de compartir el formulario. Para obtener instrucciones, consulte la sección [Eliminación del acceso a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare) en el artículo [Compartir un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
