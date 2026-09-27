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
TQID: 'https://experienceleague.adobe.com/oHi8YTmAgh3KY1xfh6psNCLr4Gng0iniB3LUqbBzcOw'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 97%
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

  * **La revisión está habilitada para el usuario:** el usuario se crea como usuario en Workfront Proof.
  * **No se ha habilitado la revisión para el usuario:** el usuario se ha creado como contacto en Workfront Proof.

* **Si existe un usuario con un correo electrónico coincidente en Workfront Proof:** la revisión está habilitada para ese usuario en Workfront (si aún no lo estaba) y la información se sincroniza entre los dos usuarios.

  Para obtener más información, consulte [Configurar el acceso de revisión de un usuario](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) en [Configurar el acceso de revisión de un usuario](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Cuando existe un usuario con un correo electrónico coincidente, en su propio entorno de revisión o en otro, Workfront crea un alias de dirección de correo electrónico añadiendo el ID de cuenta del usuario como sufijo a su correo electrónico. Por ejemplo, *nombredeusuario+accountid@domain.com*. Los usuarios seguirán recibiendo notificaciones de prueba en el caso de que se cree un correo electrónico de alias.
