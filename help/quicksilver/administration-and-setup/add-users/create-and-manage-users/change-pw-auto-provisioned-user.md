---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Cambiar la contraseña de un usuario aprovisionado automáticamente
description: Le recomendamos que cambie el nombre de usuario de un nuevo usuario a su dirección de correo de Workfront y que, a continuación, le permita cambiar su contraseña.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Cambiar la contraseña de un usuario aprovisionado automáticamente

Cuando crea usuarios mediante el aprovisionamiento automático, Adobe Workfront les asigna un GUID (identificador único global) para un nombre de usuario. Un GUID es una cadena única de números aleatorios y letras, por ejemplo, *5489cb430012526e1ea635e8c29f377f*.

A menudo, cuando un nuevo usuario intenta cambiar su contraseña temporal, escribe su dirección de correo electrónico para el nombre de usuario y recibe un error por un nombre de usuario incorrecto. Para que el usuario pueda cambiar su contraseña, debe introducir su nombre de usuario asignado por el sistema, que es un GUID.

Dado que los nombres de usuario GUID pueden ser difíciles de usar, se recomienda cambiar primero el nombre de usuario de un usuario a su dirección de correo de Workfront y, a continuación, permitirles cambiar su contraseña.

>[!TIP]
>
>Puede encontrar el GUID de un usuario de las siguientes maneras:
>
>* Vaya al perfil del usuario y copie el GUID de la dirección URL en el explorador.
>
>  Por ejemplo, en la dirección URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`, copiaría la cadena de números y letras entre las dos últimas barras diagonales: `61941ab1000af22d7104628efa1c738b`.
>
>  Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Cree un informe de usuario con una columna Usuario > GUID. Para obtener más información, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Consulte la API de Workfront.
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>O</p>
       <p>Actual: plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cambiar la contraseña de un usuario aprovisionado automáticamente

1. Determine el nombre de usuario GUID de un usuario pasando una solicitud de API, como se muestra en el siguiente ejemplo:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` donde *`<domain>`* es el dominio de su empresa y *`<ID of User>`* es el Workfront ID del usuario.

   Recibirá una respuesta similar a la siguiente:

   ![](assets/get-guid.png)

   El valor devuelto para &quot;nombre de usuario&quot; es el GUID del usuario.

1. Si utiliza su GUID como nombre de usuario, cambie la contraseña del usuario.

   Para obtener más información sobre cómo cambiar la contraseña, consulte [Restablecer la contraseña](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Si su organización utiliza un sistema SSO, solo un administrador del sistema de Workfront puede cambiar la contraseña de un usuario. Para obtener más información, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Con el usuario conectado a Workfront, vaya a:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. En el cuadro **Su dirección de correo electrónico de inicio de sesión**, verifique que la dirección de correo electrónico del usuario sea correcta y luego haga clic en **Actualizar cuenta**.

   ![](assets/guidusername-350x272.png)

   El nombre de usuario del usuario se cambia a su dirección de correo electrónico de Workfront.

>[!TIP]
>
>Para buscar el ID de un usuario:
>
>1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).
>
>1. Seleccione el usuario.
>
>   Se abre la página de perfil del usuario y se muestra su ID de usuario en la dirección URL.
>
