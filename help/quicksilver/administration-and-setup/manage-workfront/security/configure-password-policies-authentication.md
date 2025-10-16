---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurar políticas de contraseña para autenticación
description: Como administrador de Adobe Workfront, puede configurar las opciones de políticas de contraseñas para personalizar la experiencia de autenticación en su sistema Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 99%

---

# Configurar políticas de contraseña para autenticación

{{important-admin-console-onboard}}

Como administrador de Adobe Workfront, puede configurar las opciones de políticas de contraseñas para personalizar la experiencia de autenticación en su sistema Workfront.

Le recomendamos que configure las preferencias de autenticación durante la implementación de Workfront y que solo las vuelva a consultar ocasionalmente después.

Próximamente se ofrecerán funcionalidades mejoradas de administración de contraseñas, o es posible que ya se encuentren disponibles para su organización. Utilice cualquiera de las siguientes secciones, en función de si su organización tiene acceso a la nueva experiencia de autenticación.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar autenticación (disponible para todos los clientes) {#configure-authentication-available-for-all-customers}

Las opciones de autenticación se muestran para todos los clientes. Próximamente se ofrecerán funcionalidades mejoradas de administración de contraseñas, o quizá ya se encuentren disponibles para su organización, tal como se describe en la sección [Configuración de la autenticación mejorada)](#configure-enhanced-authentication-coming-soon) en este artículo.

Para configurar las preferencias de autenticación:

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Autenticación**.

1. Seleccione cualquiera de los siguientes campos para establecer la configuración de autenticación de su organización:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Forzar a los usuarios a restablecer su contraseña cada <em>&lt;valor&gt;</em> días</td> 
      <td>Esto establece el lapso de tiempo para que los usuarios restablezcan su contraseña de Workfront. Esta opción está desactivada de forma predeterminada. Al habilitarla, puede elegir entre 30, 60, 90, 120, 180 días. El valor predeterminado es de 30 días.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">No permitir que los usuarios establezcan una contraseña igual a las anteriores <em>&lt;valor&gt;</em> contraseñas</td> 
      <td> <p>Este campo prohíbe a los usuarios reutilizar contraseñas para un número determinado de reinicios. De forma predeterminada, este campo está deshabilitado. Cuando lo habilita, puede establecer este valor en 5, 10 o 15 restablecimientos antes de que se pueda reutilizar una contraseña.</p> <p>Cuando se selecciona esta opción, los usuarios no pueden restablecer sus contraseñas más de una vez en un día determinado</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Si se introduce una contraseña incorrecta cinco veces consecutivas, se debe bloquear la cuenta <em> &lt;value&gt;</em> minutos: </td> 
      <td> <p>Seleccione cuánto tiempo se bloqueará a un usuario en Workfront después de introducir una contraseña incorrecta cinco veces consecutivas. De forma predeterminada, esta opción está habilitada y el tiempo de espera es de 10 minutos. Puede bloquear cuentas durante 10 minutos, 30 minutos, 1 hora, 8 horas o 24 horas. </p> <p>El restablecimiento manual de la contraseña del usuario anula este valor de espera predeterminado. <br>Los usuarios pueden restablecer sus propias contraseñas cuando estén bloqueados a través de la pantalla de inicio de sesión. Para obtener más información sobre cómo pueden restablecer su contraseña, si la han olvidado, consulte <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Restablecer la contraseña</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Las contraseñas deben contener al menos <em>&lt;valor&gt;</em> tipos de caracteres diferentes:</td> 
      <td> <p>Determina la seguridad de las contraseñas de usuario, ya que permite seleccionar el número de tipos de caracteres necesarios en las contraseñas.</p> <p>No se puede usar una palabra de diccionario reconocible como contraseña.<br>De manera predeterminada, Workfront requiere que las contraseñas contengan al menos 2 de los siguientes caracteres (también puede requerir que contengan 3 de estos caracteres para que sea una contraseña válida): </p> 
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

En esta sección se describe la experiencia de autenticación mejorada, que podría no estar aún disponible para su organización. Si su organización no se ha migrado a la nueva experiencia de autenticación, debe configurar las opciones de autenticación, tal como se describe en [Configurar autenticación (disponible para todos los clientes)](#configure-authentication-available-for-all-customers).

Para configurar las preferencias de autenticación mejorada:

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Autenticación mejorada**.
1. En el cuadro **Longitud de contraseña**, introduzca el número mínimo de caracteres necesarios para una contraseña válida.

   Workfront requiere al menos 6 caracteres.

1. (Opcional) En la sección **Requisitos de contraseña**, seleccione los tipos de caracteres necesarios en las contraseñas de usuario.

   Puede aumentar la seguridad de las contraseñas de usuario si requiere alguno o todos los tipos de caracteres en la sección Requisito de contraseña. Estas son las opciones disponibles:

   | Letras minúsculas | Requerir al menos una letra minúscula |
   |---|---|
   | Letras mayúsculas | Requerir al menos una letra mayúscula |
   | Números | Requerir al menos un número |
   | Caracteres especiales | Requerir al menos un carácter especial |

   {style="table-layout:auto"}

1. Haga clic en **Guardar**.
