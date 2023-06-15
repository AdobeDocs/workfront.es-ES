---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Eliminar usuarios a través de Adobe Admin Console
description: Puede eliminar un usuario de Adobe Workfront Fusion solamente, dejando el acceso a cualquier otro perfil de producto de Adobe, o puede eliminar el usuario de Adobe Admin Console por completo.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Eliminar usuarios mediante el [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>La funcionalidad de este artículo solo está disponible si la instancia de su organización de [!DNL Adobe Workfront Fusion] se ha incorporado al [!DNL Adobe Business Platform].
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado al [!DNL Adobe Business Platform], consulte [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

Puede quitar un usuario de [!DNL Adobe Workfront Fusion] solo, dejando acceso a cualquier otro [!DNL Adobe] perfiles de producto, o bien puede eliminar el usuario de [!DNL Adobe Admin Console] totalmente.

## Eliminar un usuario en [!DNL Adobe Workfront Fusion]

Para eliminar un usuario en [!DNL Adobe Workfront Fusion], debe desactivar el usuario a través del [!DNL Adobe Admin Console].

Se desactiva un usuario del [!DNL Adobe Admin Console] cuando se aplique una de las siguientes condiciones:

* El usuario se mueve de un perfil de producto y no se asigna a ningún otro perfil de producto.
* El usuario se elimina de un grupo vinculado a un perfil de producto y no se incluye en ningún otro grupo vinculado a un perfil de producto.
* El usuario se elimina de un perfil de producto y no se asigna a otro perfil de producto.
* El usuario se elimina o desactiva en la organización que incluye Workfront Fusion.

  Para obtener instrucciones, consulte la sección &quot;Eliminar usuarios&quot; en [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html).

Entrada [!DNL Workfront Fusion]Sin embargo, la desactivación afecta al usuario de una de las siguientes maneras:

* Si el usuario está en una sola organización, se desactiva.
* Si el usuario está en más de una organización, se eliminará de la organización en la que se modificó el usuario en la [!DNL Adobe Admin Console].
* Por otras consideraciones al eliminar un usuario en [!DNL Workfront Fusion], consulte [Consideraciones al eliminar un usuario en [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
