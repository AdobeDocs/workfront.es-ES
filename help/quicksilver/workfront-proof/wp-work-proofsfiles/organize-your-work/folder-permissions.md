---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Comprender los permisos de carpeta en  [!DNL Workfront Proof]
description: Si una persona tiene permiso para ver un elemento de una carpeta, también puede ver la carpeta en sí. Sin embargo, solo pueden ver los elementos de la carpeta que se han compartido explícitamente con ellos.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 15%

---

# Comprender los permisos de carpeta en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Si una persona tiene permiso para ver un elemento de una carpeta, también puede ver la carpeta en sí. Sin embargo, solo pueden ver los elementos de la carpeta que se han compartido explícitamente con ellos.

## Carpetas públicas

Si una carpeta es pública, los usuarios de la cuenta (excepto los observadores y los usuarios normales) pueden ver el nombre de la carpeta en la barra lateral izquierda.

El perfil de permisos también afecta a los derechos que tiene sobre las carpetas públicas:

| **Perfil/ Acción** | **Ver todos los elementos de la carpeta** | **Ver elementos compartidos explícitamente con ellos** | **Agregar elementos** | **Eliminar elementos** | **Agregar subcarpetas** | **Eliminar subcarpetas** | **Editar detalles de la carpeta** |
|---|---|---|---|---|---|---|---|
| **Creador** | Sí | Sí | Sí | Sí | Sí | Sí | Sí |
| **Administrador de facturación** | Sí | Sí | Sí | Sí | Sí | Sí | Sí |
| **Administrador** | Sí | Sí | Sí | Sí | Sí | Sí | Sí |
| **Supervisor** | Sí | Sí | Sí | Sí | Sí | Sí | Sí |
| **Responsable** | No | Sí | Sí | No | Sí | No | Sí |
| **Observador** | No | Sí | No | No | No | No | No |

{style="table-layout:auto"}

Si la carpeta pública es propiedad de un administrador, este puede eliminar la carpeta raíz y las subcarpetas.

Para obtener más información, consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Carpetas privadas

Si una carpeta es privada, los demás usuarios de la misma cuenta no podrán ver el nombre de la carpeta en la barra lateral izquierda a menos que la carpeta o los elementos de la carpeta se hayan compartido explícitamente con ellos o que tengan un perfil de Supervisor, Administrador o Administrador de facturación:

| **Perfil/ Acción** | **Ver todos los elementos de la carpeta** | **Ver elementos compartidos explícitamente con ellos** | **Agregar elementos** | **Eliminar elementos** | **Agregar subcarpetas** | **Eliminar subcarpetas** | **Editar detalles de la carpeta** |
|---|---|---|---|---|---|---|---|
| **Creador** | Sí | Sí | Sí | Sí | Sí | Sí | Sí |
| **Administrador de facturación** | Sí | Sí | Sí | Sí | Sí | Sí | Sí |
| **Administrador** | Sí | Sí | Sí | Sí | Sí | Sí | Sí |
| **Supervisor** | Sí | Sí | Sí | Sí | Sí | Sí | Sí |
| **Responsable** | No | Sí | No | No | No | No | No |
| **Observador** | No | Sí | No | No | No | No | No |

{style="table-layout:auto"}

Si, por ejemplo, desea que el administrador del proyecto y sus equipos solo vean carpetas específicas, el administrador del proyecto puede configurar una carpeta privada y luego compartirla con usuarios específicos.

Al compartir una carpeta privada, puede decidir si desea que los administradores puedan crear, editar y eliminar elementos de carpeta.

Puede establecerlo individualmente para cada persona en la página Nueva carpeta y cambiarlo en la sección [!UICONTROL Compartido con] de la página Detalles de la carpeta. Para obtener más información, vea [Crear carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) y [Administrar carpetas y su contenido en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Si una carpeta privada se comparte con un usuario o Observador, tendrán acceso de solo lectura a todos los elementos de la carpeta. Para obtener más información, vea [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) y [Compartir carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Si una carpeta principal es privada, todas las subcarpetas también lo serán. No puede tener una subcarpeta pública bajo una carpeta principal privada. Sin embargo, puede tener una subcarpeta privada debajo de una carpeta principal pública.
>* El creador y el propietario de la carpeta siempre tendrán acceso a ella y no se podrán eliminar.
>* Solo el creador y el propietario de la carpeta privada pueden eliminar la carpeta.

