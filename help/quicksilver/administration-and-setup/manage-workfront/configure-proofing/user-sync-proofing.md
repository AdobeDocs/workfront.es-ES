---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Sincronización de usuarios entre Adobe Workfront y Workfront Proof
description: La información del usuario se sincroniza de Adobe Workfront a Workfront Proof, no de Workfront Proof a Workfront. Por esta razón, cada vez que cree o modifique usuarios, deberá realizar dichos cambios en Workfront. No puede realizar cambios en los usuarios dentro de Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Sincronización de usuarios entre Adobe Workfront y Workfront Proof

La información del usuario se sincroniza de Adobe Workfront a Workfront Proof, no de Workfront Proof a Workfront. Por esta razón, cada vez que cree o modifique usuarios, deberá realizar dichos cambios en Workfront. No puede realizar cambios en los usuarios dentro de Workfront Proof.

Las secciones siguientes proporcionan información sobre la sincronización de usuarios de Workfront a Workfront Proof:

## Información que se sincroniza

Workfront sincroniza la siguiente información de usuario con Workfront Proof:

* Nombre (el nombre y los apellidos del usuario)
* Dirección de correo electrónico

## Cuando se produce la sincronización

La información del usuario se sincroniza de Workfront a Workfront Proof en las siguientes circunstancias:

* La información de un usuario se actualiza en Workfront
* Se crea un usuario en Workfront

Dependiendo de si existe un usuario con la misma dirección de correo electrónico en Workfront Proof, se producirá cualquiera de las siguientes situaciones:

* **Si no existe ningún usuario con un correo electrónico que coincida en Workfront Proof y**

   * **La revisión está habilitada para el usuario:** El usuario se crea como usuario en Workfront Proof.
   * **No se ha habilitado la revisión para el usuario:** El usuario se ha creado como contacto en Workfront Proof.

* **Si existe un usuario con un correo electrónico coincidente en Workfront Proof:** La revisión está habilitada para ese usuario en Workfront (si aún no lo estaba) y la información se sincroniza entre los dos usuarios.

  Para obtener más información, consulte [Configurar el acceso de revisión de un usuario](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) en [Configurar el acceso de revisión de un usuario](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Cuando existe un usuario con un correo electrónico coincidente, en su propio o en otro entorno de revisión, Workfront crea una dirección de correo electrónico con un alias agregando el ID de cuenta del usuario como sufijo a su correo electrónico. Por ejemplo, *username+accountid@domain.com*. Los usuarios seguirán recibiendo notificaciones de prueba en el caso de que se cree un correo electrónico de alias.
