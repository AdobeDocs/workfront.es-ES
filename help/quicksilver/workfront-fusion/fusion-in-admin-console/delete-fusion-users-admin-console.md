---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Eliminar usuarios a través de Adobe Admin Console
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 0d989134-46c0-4637-b465-6fbe04258b8a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 76%

---

# Eliminar usuarios mediante la [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Eliminar usuarios mediante Adobe Admin Console](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/manage-users-and-teams/delete-users-admin-console.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

>[!IMPORTANT]
>
>La funcionalidad de este artículo solo está disponible si la instancia de su organización de [!DNL Adobe Workfront Fusion] se ha incorporado a [!DNL Adobe Business Platform].
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a [!DNL Adobe Business Platform], consulte [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

Puede eliminar un usuario únicamente de [!DNL Adobe Workfront Fusion], dejando el acceso a cualquier otro perfil de producto de [!DNL Adobe], o puede eliminar el usuario de la [!DNL Adobe Admin Console] por completo.

## Eliminar un usuario en [!DNL Adobe Workfront Fusion]

Para eliminar un usuario en [!DNL Adobe Workfront Fusion], debe desactivar el usuario a través de [!DNL Adobe Admin Console].

Un usuario se desactiva de la [!DNL Adobe Admin Console] cuando se da una de las siguientes circunstancias:

* El usuario se elimina de un producto o perfil de producto, y no se asigna a ningún otro producto o perfil de producto.
* El usuario se elimina de un grupo vinculado a un perfil de producto y no se incluye en ningún otro grupo vinculado a un perfil de producto.
* El usuario se elimina de un perfil de producto y no se asigna a otro perfil de producto.
* El usuario se elimina o desactiva en la organización que incluye Workfront Fusion.

  Para obtener instrucciones, consulte la sección &quot;Eliminar usuarios&quot; en [Administrar usuarios individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html?lang=es).

En [!DNL Workfront Fusion], la desactivación afecta al usuario de una de las siguientes maneras:

* Si el usuario está en una sola organización, se desactiva.
* Si el usuario se encuentra en más de una organización, se eliminará de la organización en la que se modificó el usuario en el [!DNL Adobe Admin Console].
* Para ver otras consideraciones al eliminar un usuario en [!DNL Workfront Fusion], consulte [Consideraciones al eliminar un usuario en [!DNL Workfront Fusion]](../../workfront-fusion/organizations/manage-fusion-users.md#consider)
