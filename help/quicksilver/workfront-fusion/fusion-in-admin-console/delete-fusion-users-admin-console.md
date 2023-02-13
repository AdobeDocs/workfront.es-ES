---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Eliminar usuarios a través de Adobe Admin Console
description: Puede eliminar un usuario solo de Adobe Workfront Fusion, dejando acceso a cualquier otro perfil de producto de Adobe, o puede eliminarlo del Adobe Admin Console por completo.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
hidefromtoc: true
source-git-commit: 137165deb0c0e9172224e810c82bc651bb0adfc0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Eliminar usuarios a través de [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>La funcionalidad de este artículo solo está disponible si la instancia de [!DNL Adobe Workfront Fusion] se ha incorporado a la variable [!DNL Adobe Business Platform].
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado al [!DNL Adobe Business Platform], consulte [Diferencias de administración basadas en plataformas ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

Puede quitar un usuario de [!DNL Adobe Workfront Fusion] solo, dejando acceso a cualquier otro [!DNL Adobe] perfiles de producto, o puede quitar el usuario del [!DNL Adobe Admin Console] completamente.

## Eliminar un usuario en [!DNL Adobe Workfront Fusion]

Para eliminar un usuario en [!DNL Adobe Workfront Fusion], debe desactivar el usuario a través del [!DNL Adobe Admin Console].

Un usuario se desactiva de la función [!DNL Adobe Admin Console] cuando se aplique una de las siguientes condiciones:

* El usuario se elimina de un producto o perfil de producto y no se asigna a ningún otro producto o perfil de producto.
* El usuario se elimina de un grupo vinculado a un perfil de producto y no se incluye en ningún otro grupo vinculado a un perfil de producto.
* El usuario se elimina de un perfil de producto y no se asigna a otro perfil de producto.
* El usuario se elimina o desactiva en la organización que incluye Workfront Fusion.

   Para obtener instrucciones, consulte la sección &quot;Eliminar usuarios&quot; en [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

En [!DNL Workfront Fusion], la desactivación afecta al usuario de una de las siguientes maneras:

* Si el usuario está en una sola organización, se desactiva.
* Si el usuario está en más de una organización, se elimina de la organización al usuario de la que se modificó en la [!DNL Adobe Admin Console].
* Para otras consideraciones al eliminar un usuario en [!DNL Workfront Fusion], consulte [Consideraciones al eliminar un usuario en [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
