---
title: Importar usuarios
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Puede importar usuarios al sitio de Adobe Workfront sincronizando los usuarios desde un servicio de directorio de red (como Active Directory u otro directorio LDAP) o puede importar usuarios mediante un archivo de importación de hoja de cálculo.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 69%

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

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Debe tener uno de los siguientes elementos:</p> 
    <ul> 
     <li> <p>El nivel de acceso del administrador del sistema. </li> 
     <li> <p>Configuración de <b>usuarios</b> en su nivel de acceso configurado para el acceso de <b>Edición</b>, con <b>Crear</b> y al menos una de las dos opciones de <b>Administrador de usuarios</b> habilitadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si <b>Administrador de usuarios (usuarios de grupo)</b> está habilitado, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Uso de un archivo de importación de hoja de cálculo para importar usuarios

{{step-1-to-users}}

1. Haga clic en la flecha desplegable **Nuevo usuario** y, a continuación, haga clic en **Importar usuarios**.

1. En el cuadro **Importar usuarios** que aparece, descargue el archivo de muestra y, a continuación, actualice el archivo de muestra para que incluya su propia información personal de usuario.

   Cada fila incluye los siguientes campos:

   * **Nombre**
   * **Apellido**
   * **Dirección de correo electrónico**

     Las direcciones de correo electrónico deben ser únicas.

   * **Nivel de acceso**

     Los niveles de acceso distinguen entre mayúsculas y minúsculas.

   * **ID de inicio de sesión SSO**

     Este campo se incluye únicamente si el SSO está habilitado en el sistema. Debe añadir el ID de federación en este campo para cada usuario. Cuando crea un usuario desde la pestaña Personas, puede configurar una contraseña para el usuario si desea permitir que los usuarios inicien sesión sin SSO. Sin embargo, la función de importación no permite dejar en blanco el ID de inicio de sesión de SSO.

   * Asegúrese de que no haya espacios adicionales antes o después de la dirección de correo electrónico de un usuario.

   Cuando termine con una fila, debería tener este aspecto:

   ![importing-new-users.png](assets/importing-new-users.png)

1. Guarde el archivo en una ubicación de su estación de trabajo.
1. Haga clic en **Elegir archivo** en el cuadro **Importar usuarios**.

1. Desplácese hasta el archivo que ha guardado y selecciónelo.

<!--
1. (Optional) Select the **Send an invite email to this user** option to send an email invitation to the user, notifying them that a Workfront account has been created and prompting them to set their password.

   Deselect this option if you want to set the password for the user.

-->

1. Haga clic en **Importar**.

   Recibirá un mensaje de confirmación en la parte superior de la pantalla que indica que los usuarios se importaron correctamente.

>[!NOTE]
>
>Los usuarios se crean en un estado Desactivado y Pendiente de aprobación.
> 
>Si un usuario no abandona el estado de Desactivado y Aprobación pendiente en unos minutos, y una actualización de pantalla no elimina el distintivo de Aprobación pendiente, puede añadir el lote de usuarios directamente a Adobe Admin Console.
>
>Para obtener instrucciones, consulte [Administrar varios usuarios | Carga masiva de CSV](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) en la documentación de Adobe.
