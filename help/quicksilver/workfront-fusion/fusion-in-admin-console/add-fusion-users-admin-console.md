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
source-git-commit: b7ceec2750ded516cae20d12b991b8fec94c6029
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 1%

---

# Agregar usuarios a [!DNL Adobe Workfront Fusion] mediante [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Los procedimientos descritos en esta página sólo se aplican a las organizaciones que se han incorporado a [!DNL Adobe Admin Console].
>
>Si su organización aún no se ha incorporado a [!DNL Adobe Admin Console], consulte [Agregar un usuario a una organización en [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a [!DNL Adobe Admin Console], vea [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Puede agregar un usuario a [!DNL Adobe Admin Console] y asignarlo a [!DNL Adobe Workfront Fusion], o asignar un usuario existente en [!DNL Adobe Admin Console] a [!DNL Workfront Fusion].

Para ver un vídeo que describe [!DNL Workfront Fusion] en [!DNL Adobe Admin Console], incluyendo cómo agregar usuarios, consulte [[!DNL Fusion] en Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

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
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] derechos de administrador</td> 
   <td>Debe ser [!UICONTROL Product Configuration Administrator] de [!DNL Adobe] productos para su organización.</td> 
  </tr>
  </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

&#42;&#42;Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Requisitos previos

Antes de usar [!DNL Admin Console] para [!DNL Workfront], debería recibir un mensaje de correo electrónico que le invite a la consola.

1. Si es nuevo en [!DNL Adobe] y ha recibido un mensaje de correo electrónico que le informa de que ahora tiene derechos de administración para administrar el software y los servicios de [!DNL Adobe] para su organización, haga clic en el botón del mensaje de correo electrónico para crear una cuenta de [!DNL Adobe] y abrir [!DNL Admin Console].

   O

   Si ya tiene una cuenta de Adobe, vaya a la [[!DNL Adobe Admin Console] página](https://adminconsole.adobe.com/).


## Agregar un nuevo usuario a [!DNL Adobe Admin Console] y a [!DNL Workfront Fusion]

1. En la [[!DNL Adobe Admin Console] página](https://adminconsole.adobe.com/), seleccione la ficha **[!UICONTROL Productos]** en la barra de navegación superior y, a continuación, seleccione el mosaico de producto **[!DNL Workfront Fusion]**.

   ![Fusión en el Admin Console](assets/fusion-product-admin-console.png)

1. En la lista que se muestra, seleccione la organización en la que desea agregar un usuario.

   ![Instancia de Fusion en el Admin Console](assets/fusion-instances-admin-console.png)

1. En la lista que se muestra, con la ficha **[!UICONTROL Perfiles de producto]** seleccionada, haga clic en el nombre del vínculo [!DNL Workfront Fusion] [!UICONTROL Perfil de producto].

   ![Perfil de producto de Workfront Fusion](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > No realice ningún cambio en el propio [!UICONTROL Perfil del producto].

1. Con la ficha **[!UICONTROL Usuarios]** seleccionada encima de la lista, haga clic en **[!UICONTROL Agregar usuario]**.

1. En el cuadro **[!UICONTROL Agregar usuarios a este perfil de producto]**, escriba la dirección de correo electrónico o el nombre del usuario que desea agregar y, a continuación, seleccione el usuario en la lista que aparece.

1. Haga clic en **[!UICONTROL Guardar]**.

   Se crea el usuario en [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Opcional) Continúe con [Cambiar el nivel de acceso de un usuario en [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Cambio del nivel de acceso de un usuario en Workfront Fusion

### Cambie la función de un usuario a Admin

Se debe otorgar al usuario un rol de administrador en [!DNL Adobe Admin Console].

1. En la página [!DNL Workfront Fusion] [!UICONTROL Perfil de producto] donde agregó al usuario, seleccione la pestaña **[!UICONTROL Administradores]**.

1. Haga clic en **[!UICONTROL Agregar administrador]**.

1. En el cuadro **[!UICONTROL Agregar administradores de perfiles de producto]**, escriba la dirección de correo electrónico o el nombre del usuario que desea agregar y, a continuación, seleccione el usuario en la lista que aparece.

1. Haga clic en **[!UICONTROL Guardar]**.

   Este usuario es ahora un administrador en [!DNL Workfront Fusion].

### Cambie la función de un usuario a [!UICONTROL Miembro], [!UICONTROL Contable] o [!UICONTROL Desarrollador de aplicaciones].

Los roles de [!UICONTROL Miembro], [!UICONTROL Contable] y [!UICONTROL Desarrollador de aplicaciones] se administran dentro de [!DNL Workfront Fusion].

Para obtener instrucciones, consulte [Ver o editar los roles de usuario](../organizations/manage-fusion-users.md#view-or-edit-user-roles) en el artículo [Administrar [!DNL Adobe Workfront Fusion] usuarios de su organización](../organizations/manage-fusion-users.md)

## Asignar un usuario existente en [!DNL Adobe Admin Console] a [!DNL Workfront Fusion]

Puede añadir un usuario existente a un equipo en Fusion. Esto se gestiona dentro de Fusion.

Para obtener instrucciones, consulte [Agregar un usuario a un equipo](/help/quicksilver/workfront-fusion/organizations/add-user-to-an-organization.md#add-a-user-to-a-team) en el artículo Agregar un usuario a una organización o equipo en Adobe Workfront Fusion.
