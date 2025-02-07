---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Cambiar la contraseña de un usuario aprovisionado automáticamente
description: Le recomendamos que cambie el nombre de usuario del usuario nuevo a su dirección de correo de Workfront y que, a continuación, le permita cambiar la contraseña.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 95%

---

# Cambiar la contraseña de un usuario aprovisionado automáticamente

Al crear usuarios mediante el aprovisionamiento automático, Adobe Workfront les asigna un GUID (identificador único global) para un nombre de usuario. Un GUID es una cadena única de números y letras aleatorios, por ejemplo, *5489cb430012526e1ea635e8c29f377f*.

A menudo, cuando un nuevo usuario intenta cambiar su contraseña temporal, escribe su dirección de correo electrónico para el nombre de usuario y recibe un error por usar un nombre de usuario incorrecto. Para que el usuario pueda cambiar su contraseña, debe introducir el nombre de usuario asignado por el sistema, que es un GUID.

Dado que los nombres de usuario GUID pueden ser difíciles de utilizar, se recomienda cambiar primero el nombre de usuario del usuario a su dirección de correo de Workfront y, a continuación, permitirle cambiar la contraseña.

>[!TIP]
>
>Puede encontrar el GUID de un usuario de las siguientes maneras:
>
>* Vaya al perfil del usuario y copie el GUID de la URL en el explorador.
>
>  Por ejemplo, en la URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`, copiaría la cadena de números y letras situada entre las dos últimas barras diagonales: `61941ab1000af22d7104628efa1c738b`.
>
>  Para obtener más información, consulte [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Crear un informe de usuario con una columna Usuario > GUID. Para obtener más información, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
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
   <td role="rowheader">Plan de Adobe Workfront</td> 
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
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Cambiar la contraseña de un usuario aprovisionado automáticamente

1. Determine el nombre de usuario GUID de un usuario pasando una solicitud de API, como se muestra en el siguiente ejemplo:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` donde *`<domain>`* es el dominio de su compañía y *`<ID of User>`* es el ID de Workfront del usuario.

   Recibirá una respuesta similar a la siguiente:

   ![Obtener GUID](assets/get-guid.png)

   El valor devuelto para “nombre de usuario” es el GUID del usuario.

1. Si utiliza el GUID del usuario como nombre de usuario, cambie la contraseña del usuario.

   Para obtener más información sobre cómo cambiar la contraseña, consulte [Restablecer la contraseña](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Si su organización utiliza un sistema SSO, solo un administrador del sistema de Workfront puede cambiar la contraseña de un usuario. Para obtener más información, consulte [Información general sobre el inicio de sesión único en Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Con el usuario con sesión iniciada en Workfront, vaya a:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. En el cuadro **Su dirección de correo electrónico de inicio de sesión**, verifique que la dirección de correo electrónico del usuario sea correcta y luego haga clic en **Actualizar cuenta**.

   ![Username](assets/guidusername-350x272.png)

   El nombre de usuario del usuario se cambia a su dirección de correo electrónico de Workfront.

>[!TIP]
>
>Para buscar el ID de un usuario:
>
>1. Haga clic en el icono **Menú principal** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, luego haga clic en **Usuarios** ![Icono de usuarios](assets/users-icon-in-main-menu.png).
>
>1. Seleccione el usuario.
>
>   Se abre la página de perfil del usuario y se muestra su ID de usuario en la URL.
>
