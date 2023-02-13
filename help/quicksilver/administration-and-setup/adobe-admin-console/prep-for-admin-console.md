---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Preparación para incorporar su organización a Adobe Admin Console
description: Como Adobe Workfront es un producto de Adobe, puede acceder a él a través de Adobe Admin Console. Esto le permite administrar Workfront junto con otras cuentas de Adobe y productos para sus usuarios en un lugar central.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Preparación para incorporar su organización a Adobe Admin Console

Como Adobe Workfront es un producto de Adobe, puede acceder a él a través de Adobe Admin Console. Esto le permite administrar Workfront junto con otras cuentas de Adobe y productos para sus usuarios en un lugar central.

Todos los clientes de Workfront se trasladarán finalmente a Adobe Admin Console. Una vez que su organización se traslade a Adobe Admin Console, la autenticación de Workfront se administra mediante Adobe Admin Console. Preparar y hacer este movimiento antes sienta las bases para la eficiencia en la gestión del trabajo y posiciona a su organización para una innovación más rápida en el futuro

Para obtener una descripción general de Adobe Admin Console, consulte [Información general del Admin Console](https://helpx.adobe.com/es/enterprise/using/admin-console.html).

## Lista de comprobación de migración

Para asegurarse de que su organización puede migrar a Adobe Admin Console, debe realizar las siguientes acciones

1. Identifique el Adobe Admin Console en el que desee agregar Workfront.

   * Si su organización no tiene un Adobe Admin Console existente o si no desea utilizar un Adobe Admin Console existente, el Soporte técnico de Workfront puede ayudarle a crear uno nuevo.

   * Si tiene varios Admin Console de Adobe y no está seguro de cuál es el más adecuado para agregar Adobe Workfront, póngase en contacto con el servicio de asistencia técnica de Workfront.

1. Confirme con el Soporte técnico de Workfront que desea utilizar un Adobe Admin Console existente o que ha creado uno nuevo.

1. Configure la administración de identidades en Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Prepárese para hablar con el servicio de asistencia técnica de Workfront y con su equipo de TI sobre las preferencias de autenticación, como el inicio de sesión único (SSO) o el no inicio de sesión único (SSO).

   Para obtener instrucciones, consulte la sección Identity Management de la Guía de implementación para Adobe Admin Console (https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Condicional) Si utiliza el inicio de sesión único, conecte el nuevo Adobe Admin Console a su proveedor de SSO existente

   Para obtener más información e instrucciones, consulte [Configuración de identidad](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Si su organización no utiliza el inicio de sesión único, los usuarios migrados a Adobe Admin Console recibirán un correo electrónico para crear su cuenta y contraseña.

1. Asegúrese de que las direcciones de correo electrónico de los usuarios estén listas para la migración:

   1. Eliminación de correos electrónicos duplicados de Workfront

      Para obtener instrucciones, consulte Actualización de las direcciones de correo electrónico de los usuarios existentes en la instancia de Workfront en Impedir que se dupliquen los usuarios.

      Si hay direcciones de correo electrónico duplicadas en su organización, el usuario representado por la dirección de correo electrónico con la más reciente `lastLoginDate` se moverá a la organización de Adobe Admin Console. Cualquier otro usuario con esa dirección de correo electrónico se desactivará.

      >[!NOTE]
      >
      >Dado que solo un usuario con una dirección de correo electrónico determinada puede estar activo a la vez, si necesita activar otro usuario con la misma dirección de correo electrónico que un usuario activo actualmente, primero debe desactivar el usuario activo actualmente antes de activar el usuario desactivado.

   2. (Condicional) Si está utilizando integraciones de API personalizadas, confirme que esos usuarios tienen una dirección de correo electrónico válida a la que pueden acceder.

   3. (Opcional) Recomendamos desactivar los usuarios que ya no necesiten acceder a Workfront, de modo que no se agreguen a Adobe Admin Console.
   >[!IMPORTANT]
   >
   >Estas acciones relacionadas con los correos electrónicos de los usuarios deben completarse antes de que la organización empiece a pasar a Adobe Admin Console.

1. (Opcional) Actualice todas las integraciones personalizadas para utilizar OAuth2.

   Para obtener instrucciones sobre la configuración de integraciones de OAuth2, consulte [Creación de aplicaciones OAuth2 para integraciones de Workfront](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   La creación de integraciones de OAuth2 solo está disponible en la nueva experiencia de Workfront.

   >[!NOTE]
   >
   >Este paso es opcional, pero muy recomendable, ya que otras formas de autenticación y autorización de API quedarán obsoletas en el futuro.

Una vez que el Adobe Admin Console esté configurado con Workfront, puede utilizarlo para administrar a los usuarios.

Para obtener más información, consulte [Administrar usuarios en Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Para obtener una lista de otras acciones diferentes en función de si su organización ha sido incorporada a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
