---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Preparación para incorporar su organización a Adobe Admin Console
description: Dado que Adobe Workfront es un producto de Adobe, puede acceder a él a través de Adobe Admin Console. Esto le permite administrar Workfront junto con otras cuentas de Adobe y productos para los usuarios en un lugar central.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: a25eb28800ca8bbeeffedb521b3d72c8df71c697
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 96%

---

# Prepárese para incorporar su organización a la Adobe Admin Console

<!-- Audited: 12/2023 -->

Dado que Adobe Workfront es un producto de Adobe, puede acceder a él a través de Adobe Admin Console. Esto le permite administrar Workfront junto con otras cuentas de Adobe y productos para los usuarios en un lugar central.

Todos los clientes de Workfront se transferirán finalmente a la Adobe Admin Console. Una vez que la organización se ha trasladado a Adobe Admin Console, la autenticación de Workfront se administra mediante la consola. Preparar y dar este paso antes sienta las bases para una gestión eficiente del trabajo y posiciona a su organización para una innovación más rápida en el futuro

Para obtener una descripción general de la Adobe Admin Console, consulte [Información general sobre la Admin Console](https://helpx.adobe.com/es/enterprise/using/admin-console.html).

## Lista de comprobación de migración

Para garantizar que su organización pueda migrar a Adobe Admin Console, debe realizar las siguientes acciones.

1. Identifique la Adobe Admin Console donde desee añadir Workfront.

   * Si su organización no dispone de Adobe Admin Console o si no desea utilizar una existente, la asistencia de Workfront puede ayudarle a crear una nueva.

   * Si dispone de varias Adobe Admin Console y no está seguro de a cuál es más adecuado añadir Workfront, póngase en contacto con la asistencia técnica de Workfront.

1. Confirme con la asistencia de Workfront que desea utilizar una Adobe Admin Console existente o que desea crear una nueva.

1. Configure Identity Management en la Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Prepárese para hablar con la asistencia de Workfront y con su equipo de TI sobre las preferencias de autenticación, como el inicio de sesión único (SSO) o de otro tipo.

   Para obtener instrucciones, consulte la sección Identity Management de la [Guía de implementación para la Adobe Admin Console](https://helpx.adobe.com/es/enterprise/using/deployment-planning.html).

1. (Condicional) Si utiliza el inicio de sesión único, conecte la nueva Adobe Admin Console a su proveedor de SSO existente.

   Para obtener más información e instrucciones, consulte [Configurar una identidad](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Si su organización no utiliza el inicio de sesión único, los usuarios migrados a la Adobe Admin Console recibirán un correo electrónico para crear su cuenta y contraseña.

1. Asegúrese de que las direcciones de correo electrónico del usuario estén listas para la migración:

   1. Quitar los correos electrónicos duplicados de Workfront.

      Para obtener instrucciones, consulte [Actualizar las direcciones de correo electrónico de los usuarios existentes en su instancia de Workfront](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) en [Impedir usuarios duplicados](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      Si hay direcciones de correo electrónico duplicadas en su organización, el usuario representado por la dirección de correo electrónico con la última `lastLoginDate` se trasladará a la organización de la Adobe Admin Console. Se desactivarán todos los demás usuarios con esa dirección de correo electrónico.

      >[!NOTE]
      >
      >Dado que solo puede haber activo un usuario con una dirección de correo electrónico determinada a la vez, si necesita activar otro usuario con la misma dirección de correo electrónico que un usuario activo actualmente, primero debe desactivar el usuario activo antes de activar el otro usuario.

   1. (Condicional) Si utiliza integraciones de API personalizadas, confirme que esos usuarios dispongan de una dirección de correo electrónico válida a la que pueden acceder.

   1. (Opcional) Se recomienda desactivar los usuarios que ya no necesiten acceder a Workfront para que no se añadan a la Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Estas acciones con respecto a los correos electrónicos de los usuarios deben completarse antes de que su organización empiece a migrar a la Adobe Admin Console.

1. (Opcional) Actualice todas las integraciones personalizadas para utilizar OAuth2.

   Para obtener instrucciones sobre la configuración de integraciones de OAuth2, consulte [Crear aplicaciones de OAuth2 para integraciones de Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >Este paso es opcional, pero sumamente recomendable, ya que otras formas de autenticación y autorización de la API quedarán obsoletas en el futuro.

Una vez configurada la Adobe Admin Console con Workfront, puede utilizarla para crear los administradores del sistema de Workfront.

Para obtener más información, consulte [Administrar usuarios en Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Para obtener una lista de otras acciones que son diferentes según si su organización se ha incorporado a la Adobe Admin Console, consulte [Diferencias de administración basadas en la plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
