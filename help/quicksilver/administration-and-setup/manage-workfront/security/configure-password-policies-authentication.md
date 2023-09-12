---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurar directivas de contraseña para la autenticación
description: Como administrador de Adobe Workfront, puede configurar las opciones de la directiva de contraseñas para personalizar la experiencia de autenticación en su sistema Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 970cc86b00dc1afe0473ac3a387e7ce47e4a2433
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Configurar directivas de contraseña para la autenticación

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede configurar las opciones de la directiva de contraseñas para personalizar la experiencia de autenticación en su sistema Workfront.

Le recomendamos que configure las preferencias de autenticación durante la implementación de Workfront y que solo las vuelva a consultar ocasionalmente más tarde.

Próximamente se ofrecerán funcionalidades mejoradas de administración de contraseñas, o es posible que ya se encuentren disponibles para su organización. Utilice cualquiera de las siguientes secciones, en función de si su organización tiene acceso a la nueva experiencia de autenticación.

## Requisitos de acceso

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
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar autenticación (disponible para todos los clientes) {#configure-authentication-available-for-all-customers}

Las opciones de autenticación se muestran para todos los clientes. Próximamente se ofrecerán funcionalidades mejoradas de administración de contraseñas, o quizá ya se encuentren disponibles para su organización, tal como se describe en la sección [Configurar autenticación mejorada)](#configure-enhanced-authentication-coming-soon) en este artículo.

Para configurar las preferencias de autenticación:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Clic **Sistema** > **Autenticación**.

1. Seleccione cualquiera de los siguientes campos para establecer la configuración de autenticación de su organización:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Forzar a los usuarios a restablecer su contraseña cada <em>&lt;value&gt;</em> días</td> 
      <td>Esto establece el lapso de tiempo para que los usuarios restablezcan su contraseña de Workfront. Esta opción está desactivada de forma predeterminada. Al activarla, puede elegir entre 30, 60, 90, 120, 180 días. El valor predeterminado es de 30 días.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">No permitir que los usuarios establezcan una contraseña igual a las anteriores <em>&lt;value&gt;</em> contraseñas</td> 
      <td> <p>Este campo prohíbe a los usuarios reutilizar contraseñas para un número determinado de reinicios. De forma predeterminada, este campo está deshabilitado. Cuando lo habilita, puede establecer este valor en 5, 10 o 15 restablecimientos antes de que se pueda reutilizar una contraseña.</p> <p>Cuando se selecciona esta opción, los usuarios no pueden restablecer sus contraseñas más de una vez en un día determinado</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Si se introduce una contraseña incorrecta cinco veces consecutivas, se debe bloquear la cuenta durante <em>&lt;value&gt;</em> minutos: </td> 
      <td> <p>Seleccione cuánto tiempo se bloqueará a un usuario en Workfront después de introducir una contraseña incorrecta cinco veces consecutivas. De forma predeterminada, esta opción está habilitada y el tiempo de espera es de 10 minutos. Puede bloquear cuentas durante 10 minutos, 30 minutos, 1 hora, 8 horas o 24 horas. </p> <p>El restablecimiento manual de la contraseña del usuario anula este valor de espera predeterminado. <br>Los usuarios pueden restablecer sus propias contraseñas cuando están bloqueados a través de la pantalla de inicio de sesión. Para obtener más información sobre cómo pueden restablecer su contraseña, si la olvidaron, consulte <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Restablecer la contraseña</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Las contraseñas deben contener al menos <em>&lt;value&gt;</em> diferentes tipos de caracteres:</td> 
      <td> <p>Determina la seguridad de las contraseñas de usuario, ya que permite seleccionar el número de tipos de caracteres necesarios en las contraseñas.</p> <p>No se puede usar una palabra de diccionario reconocible como contraseña.<br>De forma predeterminada, Workfront requiere que haya al menos 2 de los siguientes caracteres en las contraseñas (también puede requerir que 3 de estos caracteres estén presentes para una contraseña válida): </p> 
       <ul> 
        <li>Caracteres en mayúsculas</li> 
        <li>Caracteres en minúsculas</li> 
        <li>Números</li> 
        <li>Símbolos</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

## Configuración de la autenticación mejorada{#configure-enhanced-authentication-coming-soon}

En esta sección se describe la experiencia de autenticación mejorada, que podría no estar aún disponible para su organización. Si su organización no se ha migrado a la nueva experiencia de autenticación, debe configurar los ajustes de autenticación, tal como se describe en [Configurar autenticación (disponible para todos los clientes)](#configure-authentication-available-for-all-customers).

Para configurar las preferencias de autenticación mejorada:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Clic **Sistema** > **Autenticación mejorada**.
1. En el **Longitud de contraseña** , introduzca el número mínimo de caracteres necesarios para una contraseña válida.

   Workfront requiere al menos 6 caracteres.

1. (Opcional) En el **Requisitos de contraseña** , seleccione los tipos de caracteres requeridos en las contraseñas de usuario.

   Puede aumentar la seguridad de las contraseñas de usuario si requiere alguno o todos los tipos de caracteres en la sección Requisito de contraseña. Estas son las opciones disponibles:

   | Letras minúsculas | Requerir al menos una letra minúscula |
   |---|---|
   | Letras mayúsculas | Requerir al menos una letra mayúscula |
   | Números | Requerir al menos un número |
   | Caracteres especiales | Requiere al menos un carácter especial |

   {style="table-layout:auto"}

1. Haga clic en **Guardar**.
