---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Añadir usuarios a Adobe Workfront Fusion mediante Adobe Admin Console
description: Puede añadir un usuario a Adobe Admin Console y asignarlo a Adobe Workfront Fusion o asignar un usuario existente de Adobe Admin Console a Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# Añadir usuarios a [!DNL Adobe Workfront Fusion] a través de [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Los procedimientos descritos en esta página se aplican únicamente a las organizaciones que se han incorporado al [!DNL Adobe Admin Console].
>
>Si su organización aún no se ha incorporado al [!DNL Adobe Admin Console], consulte [Adición de un usuario a una organización en [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado al [!DNL Adobe Admin Console], consulte [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Puede añadir un usuario a [!DNL Adobe Admin Console] y asígnelas a [!DNL Adobe Workfront Fusion]o asigne un usuario existente en la [!DNL Adobe Admin Console] hasta [!DNL Workfront Fusion].

Para ver un vídeo que describe [!DNL Workfront Fusion] en el [!DNL Adobe Admin Console], incluido cómo agregar usuarios, consulte [[!DNL Fusion] en Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL Workfront Fusion para automatización e integración de trabajo] </p> <p>[!UICONTROL Workfront Fusion for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] derechos de administrador</td> 
   <td>Debe ser [!UICONTROL Product Configuration Administrator] de [!DNL Adobe] productos para su organización.</td> 
  </tr>
  </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Requisitos previos

Antes de usar el [!DNL Admin Console] para [!DNL Workfront], debería recibir un correo electrónico que le invite a la consola.

1. Si es nuevo en [!DNL Adobe] y ha recibido un correo electrónico que le informa de que ahora tiene derechos de administración para gestionar [!DNL Adobe] y servicios para su organización, haga clic en el botón del correo electrónico para crear una [!DNL Adobe] y abra la [!DNL Admin Console].

   O

   Si ya tiene una cuenta de Adobe, vaya a [[!DNL Adobe Admin Console] página](https://adminconsole.adobe.com/).


## Añadir un nuevo usuario a [!DNL Adobe Admin Console] y [!DNL Workfront Fusion]

1. Desde el [[!DNL Adobe Admin Console] página](https://adminconsole.adobe.com/), seleccione la **[!UICONTROL Productos]** en la barra de navegación superior y, a continuación, seleccione la pestaña **[!DNL Workfront Fusion]** mosaico del producto.

   ![Fusion en Admin Console](assets/fusion-product-admin-console.png)

1. En la lista que se muestra, seleccione la organización en la que desea agregar un usuario.

   ![Instancia de Fusion en Admin Console](assets/fusion-instances-admin-console.png)

1. En la lista que se muestra, con la variable **[!UICONTROL Perfiles de producto]** pestaña seleccionada, haga clic en el nombre del [!DNL Workfront Fusion] [!UICONTROL Perfil del producto] vínculo.

   ![Perfil del producto de Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > No realice ningún cambio en [!UICONTROL Perfil del producto] sí mismo.

1. Con el **[!UICONTROL Usuarios]** pestaña seleccionada encima de la lista, haga clic en **[!UICONTROL Añadir usuario]**.

1. En el **[!UICONTROL Añadir usuarios a este perfil de producto]** , escriba la dirección de correo electrónico o el nombre del usuario que desea agregar y, a continuación, seleccione el usuario en la lista que aparece.

1. Haga clic en **[!UICONTROL Guardar]**.

   El usuario se crea en [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Opcional) Continúe en [Cambiar el nivel de acceso de un usuario en [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Cambio del nivel de acceso de un usuario en Workfront Fusion

### Cambie la función de un usuario a Admin

Para otorgar a un usuario un rol de administrador, debe realizarse lo siguiente en la [!DNL Adobe Admin Console].

1. En el [!DNL Workfront Fusion] [!UICONTROL Perfil del producto] página donde agregó al usuario, seleccione la **[!UICONTROL Administradores]** pestaña.

1. Clic **[!UICONTROL Añadir administrador]**.

1. En el **[!UICONTROL Añadir administradores de perfil de producto]** , escriba la dirección de correo electrónico o el nombre del usuario que desea agregar y, a continuación, seleccione el usuario en la lista que aparece.

1. Haga clic en **[!UICONTROL Guardar]**.

   Este usuario es ahora un administrador en [!DNL Workfront Fusion].

### Cambiar la función de un usuario a [!UICONTROL Miembro], [!UICONTROL Contable], o [!UICONTROL Desarrollador de aplicaciones].

[!UICONTROL Miembro], [!UICONTROL Contable], y [!UICONTROL Desarrollador de aplicaciones] Los roles de se gestionan dentro de [!DNL Workfront Fusion].

Para obtener instrucciones, consulte [Ver o editar roles de usuario](../organizations/manage-fusion-users.md#view-or-edit-user-roles) en el artículo [Administrar [!DNL Adobe Workfront Fusion] usuarios de su organización](../organizations/manage-fusion-users.md)

## Asigne un usuario existente en la [!DNL Adobe Admin Console] hasta [!DNL Workfront Fusion]

1. Empiece a editar el usuario como se describe en la sección &quot;Editar detalles del usuario&quot; del artículo [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) en el [!DNL Adobe Admin Console] documentación.

1. Añadir **[!DNL Adobe Workfront Fusion]** a los productos asignados al usuario.
