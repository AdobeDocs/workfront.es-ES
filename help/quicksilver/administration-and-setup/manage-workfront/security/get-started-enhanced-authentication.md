---
title: Introducción a la autenticación mejorada
description: Oculto de la búsqueda y de la navegación izquierda
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 3%

---

# Introducción a la autenticación mejorada

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront está cambiando la administración del sistema de usuarios y contraseñas. Estos cambios se implementarán en una versión por fases llamada **Autenticación mejorada** experiencia. La autenticación mejorada ofrece a los usuarios una experiencia de inicio de sesión más coherente y segura en todos los productos y servicios de Workfront.

La siguiente tabla proporciona detalles sobre la funcionalidad actual y futura:

>[!IMPORTANT]
>
>La mayoría de los clientes utilizan actualmente la autenticación heredada y algunos utilizan la autenticación mejorada 1.0.
> 
>Para comprobar qué tipo de autenticación está utilizando actualmente, vaya a *your_domain*.my.workfront.com/login. Si se le redirige a /auth/login, está utilizando la autenticación mejorada 1.0.
> 
>Si se le redirige a https://login-a-xx.workfront.com/, donde &quot;xx&quot; podría ser EE. UU. (Estados Unidos), UE (Europa) o GCP (Google Cloud Platform) según su ubicación o plataforma, utilizará la autenticación mejorada 2.0.
>
>Todos los clientes pasarán a la autenticación mejorada 2.0 a finales de 2021.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Función</strong> </p> </th> 
   <th><strong>Autenticación heredada</strong> </th> 
   <th><strong>Autenticación mejorada 1.0</strong> </th> 
   <th> <p>Autenticación mejorada 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Opciones de inicio de sesión</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Habilite un solo nombre de usuario para utilizarlo en todos los productos y servicios de Workfront, incluidos aprendizaje, asistencia y otros</p> </td> 
   <td>No disponible</td> 
   <td> <p>No disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir el uso de la misma dirección de correo electrónico en todas las instancias de Workfront</p> </td> 
   <td> <p>✓</p> <p>Disponible desde la versión 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponible desde la versión 2019.3</p> </td> 
   <td> <p>✓</p> <p>Disponible desde la versión 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Las direcciones de correo electrónico no distinguen entre mayúsculas y minúsculas</p> </td> 
   <td> <p>✓</p> <p>Disponible desde la versión 2019.3</p> </td> 
   <td> <p>✓</p> <p>Varios usuarios no pueden tener la misma dirección de correo electrónico si la dirección solo difiere según el caso. </p> </td> 
   <td> <p>✓</p> <p>Varios usuarios no pueden tener la misma dirección de correo electrónico si la dirección solo difiere según el caso. </p> <p>Se notificará a los administradores de Workfront a finales de 2019 para que empiecen a corregir direcciones de correo electrónico duplicadas.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Opciones de administración de contraseñas</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Instigar un correo electrónico de restablecimiento de contraseña para un usuario como administrador de Workfront</p> </td> 
   <td> <p>No disponible </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Establecer una contraseña temporal para un usuario como administrador de Workfront</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>No planificado</p> <p>Esta funcionalidad no es una práctica recomendada de seguridad</p> </td> 
   <td> <p>No planificado</p> <p>Esta funcionalidad no es una práctica recomendada de seguridad</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Requisitos de política de contraseñas</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Requerir que los usuarios restablezcan las contraseñas después de un periodo de tiempo determinado</p> </td> 
   <td>✓</td> 
   <td> <p>No planificado</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Restringir a los usuarios el uso de una contraseña anterior </p> </td> 
   <td>✓</td> 
   <td>No planificado </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Protéjase contra intentos incorrectos de introducción de contraseñas </p> </td> 
   <td> <p>✓ </p> <p>Bloquea la cuenta tras cinco intentos incorrectos de introducción de contraseña. El tiempo de espera necesario después de que el administrador de Workfront haya configurado el bloqueo</p> </td> 
   <td> <p>✓</p> <p>El tiempo de espera aumenta exponencialmente después de cada contraseña incorrecta sucesiva en función de las prácticas recomendadas del sector; el administrador de Workfront no puede configurar el tiempo requerido</p> </td> 
   <td> <p>✓</p> <p>Utiliza un algoritmo de bloqueo que bloquea de forma proactiva una variedad de comportamientos sospechosos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Requiere una combinación de minúsculas, mayúsculas, números y caracteres especiales</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Mayor flexibilidad a la hora de elegir requisitos específicos</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Establecer una longitud mínima de contraseña </p> </td> 
   <td> No disponible </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>Compatibilidad con el Protocolo de inicio de sesión único</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Admite integraciones SSO compatibles con los protocolos Active Directory y LDAP</p> </td> 
   <td> ✓ </td> 
   <td> <p> Obsoleto</p> <p>Los sistemas Active Directory, Azure y LDAP deben utilizar SAML 2.0</p> </td> 
   <td> <p>Obsoleto</p> <p>Los sistemas Active Directory, Azure y LDAP se pueden configurar con SAML 2.0 cifrado o OpenID Connect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Admite protocolos SSO compatibles con SAML 2.0 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Admite protocolos de conexión Open ID</p> </td> 
   <td> <p>No disponible</p> </td> 
   <td> <p>No disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Configure la página de inicio de sesión de Workfront para que redirija siempre a la página de inicio de sesión del proveedor de identidad </p> </td> 
   <td> Habilitado de forma predeterminada y no se puede deshabilitar</td> 
   <td> <p>✓</p> <p>El administrador de Workfront puede configurar la página de inicio de sesión para redirigir a la página de inicio de sesión del proveedor de identidad o puede configurar un botón o botones de inicio de sesión.</p> </td> 
   <td> <p>✓</p> <p> Los administradores de Workfront pueden configurar la página de inicio de sesión para redirigir a la página de inicio de sesión del proveedor de identidad o pueden configurar botones de inicio de sesión.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permitir que cada instancia habilite varios proveedores de SSO</p> </td> 
   <td> <p>N/D</p> </td> 
   <td> <p>No planificado</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Compatibilidad con entorno</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Un solo nombre de usuario y contraseña para los entornos de vista previa</p> </td> 
   <td> <p>No disponible</p> </td> 
   <td> <p>No disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Un solo nombre de usuario y contraseña para entornos de zona protegida</p> </td> 
   <td> <p>No disponible</p> </td> 
   <td> <p>No disponible</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
