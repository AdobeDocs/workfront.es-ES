---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Administrar [!DNL Adobe Workfront Fusion] usuarios de su organización
description: Administrar [!DNL Adobe Workfront Fusion] usuarios de su organización
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Administrar [!DNL Adobe Workfront Fusion] usuarios de su organización

[!DNL Adobe Workfront Fusion] los administradores pueden administrar las funciones de usuario dentro de [!DNL Workfront Fusion].

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
    <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>Workfront Fusion para automatización e integración del trabajo,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> 
     <p>Debe ser [!DNL Workfront Fusion] administrador de su organización.</p>
     <p>Debe ser [!DNL Workfront Fusion] administrador de su equipo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Ver o editar funciones de usuario {#view}

[!DNL Adobe Workfront Fusion] los administradores pueden ver y actualizar las funciones de usuario.

1. Cuando haya iniciado sesión como [!DNL Workfront Fusion] administrador, seleccione **[!UICONTROL Usuarios]** en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Detalles]** en la fila del usuario que desea ver.
1. (Opcional) Para actualizar la función del usuario, haga clic en el menú desplegable del **[!DNL Role]** en la fila de la organización en la que desea cambiar la función del usuario y, a continuación, seleccione la nueva función.

## Ver o editar detalles del usuario {#view2}

[!DNL Adobe Workfront Fusion] los administradores pueden ver y actualizar los detalles del usuario.

1. Cuando haya iniciado sesión como [!DNL Workfront Fusion] administrador, seleccione **[!UICONTROL Usuarios]** en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Detalles]** en la fila del usuario que desea ver.
1. (Opcional) Para actualizar los detalles del usuario, haga clic en **[!UICONTROL Opciones]** en la esquina superior derecha de la pantalla, seleccione **[!UICONTROL Detalles del cambio]**.

## Eliminar un usuario {#delete}

[!DNL Adobe Workfront Fusion] los administradores pueden eliminar usuarios.

1. Cuando haya iniciado sesión como [!DNL Workfront Fusion] administrador, seleccione [!UICONTROL Usuarios] en el panel de navegación izquierdo.
1. Haga clic en **[!UICONTROL Detalles]** en la fila del usuario que desea ver.
1. (Opcional) Para actualizar los detalles del usuario, haga clic en **[!UICONTROL Opciones]** en la esquina superior derecha de la pantalla, seleccione **[!UICONTROL Eliminar]**.

### Consideraciones al eliminar un usuario en Workfront Fusion

* Cuando se elimina un usuario, se eliminan las conexiones, claves y enlaces web del usuario. Todos los escenarios pertenecientes al usuario se transfieren al propietario de la organización. Las conexiones en estos escenarios deben actualizarse, ya que las conexiones pertenecientes al usuario ya no son válidas.
* Si el usuario eliminado es propietario de aplicaciones o plantillas públicas, las aplicaciones o plantillas públicas se transfieren al propietario de la organización. Si no hay un propietario de organización, las aplicaciones o plantillas públicas se transfieren a otro usuario.
