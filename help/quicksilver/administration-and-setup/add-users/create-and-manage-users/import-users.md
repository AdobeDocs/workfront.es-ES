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
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# Importar usuarios

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para obtener instrucciones sobre la edición del perfil de un usuario en Adobe Admin Console, consulte la sección &quot;Agregar usuarios&quot; en el artículo [Usuarios de carga masiva](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) o póngase en contacto con su administrador de Adobe Admin Console.
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Puede importar usuarios mediante un archivo de importación de hoja de cálculo.

Antes de crear un usuario nuevo, asegúrese de que ha creado todos los objetos que desea asociar al usuario. Por ejemplo, si no ha creado una programación, no puede asignarla al nuevo usuario y el campo que utiliza para asociar una programación al nuevo usuario no aparece en la pantalla Nuevo usuario.

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
   <td> <p>Debe tener una de las siguientes opciones:</p> 
    <ul> 
     <li> <p>Nivel de acceso del administrador del sistema. Para obtener más información, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>. </p> </li> 
     <li> <p><b>Usuarios</b> en el nivel de acceso configurado para <b>Editar</b> acceso, con <b>Crear</b> y al menos uno de los dos <b>Administrador de usuarios</b> opciones activadas en <b>Ajustar la configuración</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>De estas dos opciones, si es Usuario <b>Administración (usuarios del grupo)</b> está activada, debe ser administrador de grupo de un grupo al que pertenezca el usuario.</p> <p>Para obtener más información sobre la variable <b>Usuarios</b> configuración en un nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acceso a los usuarios</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Uso de un archivo de importación de hoja de cálculo para importar usuarios

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).

1. Haga clic en el **Nuevo usuario** flecha desplegable y, a continuación, haga clic en **Importar usuarios**.

1. En el **Importar usuarios** que aparece, descargue el archivo de muestra y, a continuación, actualice el archivo de muestra para incluir la información personal de su propio usuario.

   Cada fila incluye los siguientes campos:

   * **Nombre**
   * **Apellido**
   * **Dirección de correo electrónico**

      Las direcciones de correo electrónico deben ser únicas.

   * **Nivel de acceso**

      Los niveles de acceso distinguen entre mayúsculas y minúsculas.

   * **Identificador de inicio de sesión SSO**

      Este campo se incluye únicamente si SSO está habilitado en el sistema. Debe agregar el ID de federación en este campo para cada usuario. Cuando crea un usuario desde la ficha Personas , puede configurar una contraseña para el usuario si desea permitir que los usuarios inicien sesión sin SSO. Sin embargo, la función de importación no permite dejar en blanco el ID de inicio de sesión de SSO.

   * Asegúrese de que no existan espacios adicionales antes o después de la dirección de correo electrónico de un usuario.

   Cuando haya terminado con una fila, debería tener este aspecto:

   ![import-new-users.png](assets/importing-new-users.png)

1. Guarde el archivo en una ubicación de la estación de trabajo.
1. Haga clic en **Elegir archivo** en el **Importar usuarios** en la ventana

1. Busque y seleccione el archivo que guardó.
1. (Opcional) Seleccione el **Enviar un correo electrónico de invitación a este usuario** para enviar una invitación por correo electrónico al usuario, notificándoles que se ha creado una cuenta de Workfront y pidiéndoles que establezcan su contraseña.

   Anule la selección de esta opción si desea establecer la contraseña del usuario.

1. Haga clic en **Importar**.

   Recibirá un mensaje de confirmación en la parte superior de la pantalla de que el usuario se ha importado correctamente.
