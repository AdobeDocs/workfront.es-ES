---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Sincronización de usuarios entre Adobe Workfront y Workfront Proof
description: La información del usuario se sincroniza de Adobe Workfront a Workfront Proof; no se sincroniza de Workfront Proof a Workfront. Debido a esto, cada vez que cree o modifique usuarios, debe realizar esos cambios dentro de Workfront. No puede realizar cambios en los usuarios dentro de la prueba de Workfront.
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

La información del usuario se sincroniza de Adobe Workfront a Workfront Proof; no se sincroniza de Workfront Proof a Workfront. Debido a esto, cada vez que cree o modifique usuarios, debe realizar esos cambios dentro de Workfront. No puede realizar cambios en los usuarios dentro de la prueba de Workfront.

Las secciones siguientes proporcionan información sobre la sincronización de usuarios de Workfront a Workfront Proof:

## Información sincronizada

Workfront sincroniza la siguiente información de usuario con Workfront Proof:

* Nombre (el nombre y los apellidos del usuario)
* Dirección de correo electrónico

## Cuando se produce una sincronización

La información de usuario se sincroniza de Workfront a Workfront Proof en las siguientes circunstancias:

* La información de un usuario se actualiza en Workfront
* Se crea un usuario en Workfront

Dependiendo de si existe un usuario con la misma dirección de correo electrónico en la prueba de Workfront, se produce cualquiera de las siguientes situaciones:

* **Si no existe ningún usuario con un correo electrónico coincidente en Workfront Proof y**

   * **La prueba está habilitada para el usuario:** El usuario se crea como usuario en Workfront Proof.
   * **La prueba no está habilitada para el usuario:** El usuario se crea como un contacto en Workfront Proof.

* **Si existe un usuario con un correo electrónico coincidente en Workfront Proof:** La prueba está habilitada para ese usuario en Workfront (si no estaba habilitada) y la información se sincroniza entre los dos usuarios.

   Para obtener más información, consulte [Configuración del acceso de prueba de un usuario](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) en [Configuración del acceso de prueba de un usuario](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >Cuando existe un usuario con un correo electrónico coincidente, ya sea en su propio entorno de pruebas o en otro entorno, Workfront crea una dirección de correo electrónico con alias añadiendo el ID de cuenta del usuario como sufijo a su correo electrónico. Por ejemplo, *username+accountid@domain.com*. Los usuarios seguirán recibiendo notificaciones de prueba en caso de que se cree un correo electrónico con alias.
