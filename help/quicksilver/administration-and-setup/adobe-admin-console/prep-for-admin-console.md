---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Prepárese para incorporar su organización a Adobe Admin Console
description: Como Adobe Workfront es un producto de Adobe, puede acceder a él a través de Adobe Admin Console. Esto le permite administrar Workfront junto con otras cuentas de Adobe y productos para los usuarios en un lugar central.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Prepárese para incorporar su organización a Adobe Admin Console

<!-- Audited: 12/2023 -->

Como Adobe Workfront es un producto de Adobe, puede acceder a él a través de Adobe Admin Console. Esto le permite administrar Workfront junto con otras cuentas de Adobe y productos para los usuarios en un lugar central.

Todos los clientes de Workfront se transferirán finalmente a Adobe Admin Console. Una vez que la organización se ha trasladado a Adobe Admin Console, la autenticación de Workfront se administra mediante la consola. Preparar y realizar este movimiento antes sienta las bases para una gestión eficiente del trabajo y posiciona a su organización para una innovación más rápida en el futuro

Para obtener una descripción general de Adobe Admin Console, consulte [Resumen del Admin Console](https://helpx.adobe.com/es/enterprise/using/admin-console.html).

## Lista de comprobación de migración

Para garantizar que su organización pueda migrar a Adobe Admin Console, debe realizar las siguientes acciones.

1. Identifique la Adobe Admin Console donde desee agregar Workfront.

   * Si su organización no tiene un Adobe Admin Console Adobe Admin Console existente o si no desea utilizar uno existente, el Soporte de Workfront puede ayudarle a crear uno nuevo.

   * Si tiene varios Admin Console de Adobe y no está seguro de cuál es el más adecuado para agregar Workfront a, póngase en contacto con el Soporte técnico de Workfront.

1. Confirme con el Soporte de Workfront que desea utilizar un Adobe Admin Console existente o que desea crear uno nuevo.

1. Configure la administración de identidades en Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Prepárese para hablar con el Soporte de Workfront y con su equipo de TI sobre las preferencias de autenticación, como el inicio de sesión único (SSO) o no SSO.

   Para obtener instrucciones, consulte la sección Identity Management del [Guía de implementación para Adobe Admin Console](https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Condicional) Si utiliza el inicio de sesión único, conecte el nuevo Adobe Admin Console a su proveedor de SSO existente.

   Para obtener más información e instrucciones, consulte [Configurar identidad](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Si su organización no utiliza el inicio de sesión único, los usuarios migrados a Adobe Admin Console recibirán un correo electrónico para crear su cuenta y contraseña.

1. Asegúrese de que las direcciones de correo electrónico del usuario estén listas para la migración:

   1. Elimine los correos electrónicos duplicados de Workfront.

      Para obtener instrucciones, consulte [Actualizar las direcciones de correo electrónico de los usuarios existentes en la instancia de Workfront](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) in [Impedir usuarios duplicados](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      Si hay direcciones de correo electrónico duplicadas en su organización, el usuario representado por la dirección de correo electrónico con el más reciente. `lastLoginDate` se moverán a la organización de Adobe Admin Console. Se desactivarán todos los demás usuarios con esa dirección de correo electrónico.

      >[!NOTE]
      >
      >Dado que solo puede estar activo un usuario con una dirección de correo electrónico determinada a la vez, si necesita activar otro usuario con la misma dirección de correo electrónico que un usuario activo actualmente, primero debe desactivar el usuario activo antes de activar el usuario desactivado.

   1. (Condicional) Si utiliza integraciones de API personalizadas, confirme que esos usuarios tienen una dirección de correo electrónico válida a la que pueden acceder.

   1. (Opcional) Se recomienda desactivar los usuarios que ya no necesiten acceder a Workfront para que no se añadan a Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Estas acciones con respecto a los correos electrónicos de los usuarios deben completarse antes de que su organización empiece a pasar a Adobe Admin Console.

1. (Opcional) Actualice todas las integraciones personalizadas para utilizar OAuth2.

   Para obtener instrucciones sobre la configuración de integraciones de OAuth2, consulte [Creación de aplicaciones de OAuth2 para integraciones de Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >Este paso es opcional, pero muy recomendable, ya que otras formas de autenticación y autorización de la API quedarán obsoletas en el futuro.

Una vez configurado el Adobe Admin Console con Workfront, puede utilizarlo para administrar los usuarios.

Para obtener más información, consulte [Administración de usuarios en Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Para obtener una lista de otras acciones que son diferentes en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
