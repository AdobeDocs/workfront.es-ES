---
title: Importar usuarios
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puede importar usuarios al sitio de Adobe Workfront sincronizando los usuarios desde un servicio de directorio de red (como Active Directory u otro directorio LDAP), o puede importar usuarios mediante un archivo de importación de hoja de cálculo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 1949a0bb213553f1f1f252c4382a90514fcd0b5b
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Importar usuarios

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

Puede importar usuarios mediante un archivo de importación de hoja de cálculo.

Antes de crear un nuevo usuario, asegúrese primero de que ha creado todos los objetos que desea asociar con el usuario. Por ejemplo, si no ha creado una programación, no puede asignarla al nuevo usuario y el campo que utiliza para asociarla no aparece en la pantalla Nuevo usuario.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p><b>Usuarios</b> en su nivel de acceso configurado en <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos <b>Administrador de usuarios</b> opciones activadas en <b>Ajuste la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si el usuario <b>Administrador (usuarios de grupo)</b> está habilitada, debe ser administrador de un grupo del que sea miembro el usuario.</p> <p>Para obtener más información sobre <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Concesión de acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Uso de un archivo de importación de hoja de cálculo para importar usuarios

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Haga clic en **Nuevo usuario** flecha desplegable y haga clic en **Importar usuarios**.

1. En el **Importar usuarios** , descargue el archivo de muestra y, a continuación, actualice el archivo de muestra para incluir la información personal del usuario.

   Cada fila incluye los siguientes campos:

   * **Nombre**
   * **Apellidos**
   * **Correo electrónico**

     Las direcciones de correo electrónico deben ser únicas.

   * **Nivel de acceso**

     Los niveles de acceso distinguen entre mayúsculas y minúsculas.

   * **Identificador de inicio de sesión SSO**

     Este campo se incluye únicamente si el SSO está activado en el sistema. Debe agregar el identificador de federación en este campo para cada usuario. Cuando crea un usuario desde la pestaña Personas, puede configurar una contraseña para el usuario si desea permitir que los usuarios inicien sesión sin SSO. Sin embargo, la función de importación no permite dejar en blanco el ID de INICIO DE SESIÓN SSO.

   * Asegúrese de que no haya espacios adicionales antes o después de la dirección de correo electrónico de un usuario.

   Cuando termine con una fila, debería tener este aspecto:

   ![import-new-users.png](assets/importing-new-users.png)

1. Guarde el archivo en una ubicación de la estación de trabajo.
1. Clic **Elegir archivo** en el **Importar usuarios** cuadro.

1. Desplácese hasta el archivo que ha guardado y selecciónelo.
1. (Opcional) Seleccione la **Enviar invitación por correo electrónico a este usuario** opción para enviar una invitación por correo electrónico al usuario, notificándole que se ha creado una cuenta de Workfront y pidiéndole que establezca su contraseña.

   Anule la selección de esta opción si desea establecer la contraseña del usuario.

1. Clic **Importar**.

   Recibirá un mensaje de confirmación en la parte superior de la pantalla que indica que el usuario se importó correctamente.
