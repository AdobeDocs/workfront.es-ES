---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Administrar  [!DNL Adobe Workfront Fusion] usuarios de su organización
description: Administrar  [!DNL Adobe Workfront Fusion] usuarios de su organización
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Administrar usuarios de [!DNL Adobe Workfront Fusion] en su organización

[!DNL Adobe Workfront Fusion] administradores pueden administrar los roles de usuario dentro de [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo], [!UICONTROL [!DNL Workfront Fusion] para automatización de trabajo]</p>
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> 
     <p>Debe ser administrador de [!DNL Workfront Fusion] para su organización.</p>
     <p>Debe ser administrador de [!DNL Workfront Fusion] para su equipo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ver o editar roles de usuario {#view}

Los administradores de [!DNL Adobe Workfront Fusion] pueden ver y actualizar los roles de usuario.

1. Cuando haya iniciado sesión como administrador de [!DNL Workfront Fusion], seleccione **[!UICONTROL Usuarios]** en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Detalles]** en la fila del usuario que desee ver.
1. (Opcional) Para actualizar la función del usuario, haga clic en el menú desplegable de la columna **[!DNL Role]** en la fila de la organización donde desea cambiar la función del usuario y, a continuación, seleccione la nueva función.

## Ver o editar los detalles del usuario {#view2}

[!DNL Adobe Workfront Fusion] administradores pueden ver y actualizar los detalles del usuario.

1. Cuando haya iniciado sesión como administrador de [!DNL Workfront Fusion], seleccione **[!UICONTROL Usuarios]** en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Detalles]** en la fila del usuario que desee ver.
1. (Opcional) Para actualizar los detalles del usuario, haga clic en **[!UICONTROL Opciones]** en la esquina superior derecha de la pantalla y seleccione **[!UICONTROL Cambiar detalles]**.

## Eliminar un usuario {#delete}

[!DNL Adobe Workfront Fusion] administradores pueden eliminar usuarios.

1. Cuando haya iniciado sesión como administrador de [!DNL Workfront Fusion], seleccione [!UICONTROL Usuarios] en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Detalles]** en la fila del usuario que desee ver.
1. (Opcional) Para actualizar los detalles del usuario, haga clic en **[!UICONTROL Opciones]** en la esquina superior derecha de la pantalla y, a continuación, seleccione **[!UICONTROL Eliminar]**.

### Consideraciones al eliminar un usuario en Workfront Fusion

* Cuando se elimina un usuario, se eliminan sus conexiones, claves y enlaces web. Cualquier escenario que pertenezca al usuario se transfiere al propietario de la organización. Las conexiones en estos casos deben actualizarse, ya que las conexiones que pertenecen al usuario ya no son válidas.
* Si el usuario eliminado es propietario de aplicaciones o plantillas públicas, estas se transfieren al propietario de la organización. Si no hay un Propietario de la organización, las aplicaciones o plantillas públicas se transfieren a otro usuario.
