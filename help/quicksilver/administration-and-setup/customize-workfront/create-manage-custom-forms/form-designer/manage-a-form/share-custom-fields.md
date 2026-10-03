---
title: Configurar el uso compartido para campos y widgets personalizados
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: De forma predeterminada, cuando se agrega un nuevo campo personalizado o widget a un formulario personalizado, cualquier persona en el sistema con acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y el nombre de la API. Puede cambiar esto controlando con quién se puede compartir.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
TQID: 'https://experienceleague.adobe.com/KyrIWEpIQQb-f8YODUPz3-RbP5wFww8Vu7Ffy33wUog'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ecee8b1aadd804a45ff0830e04e77981a3269cff
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 56%
---
# Configuración del uso compartido para campos y widgets personalizados

De forma predeterminada, cuando se agrega un nuevo campo personalizado o widget a un formulario personalizado, cualquier persona en el sistema con acceso a los formularios personalizados puede editar las propiedades de ese elemento, como su etiqueta y el nombre de la API. Puede cambiar esto controlando con quién se puede compartir.

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


