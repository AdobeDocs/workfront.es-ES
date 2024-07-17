---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Error: Los usuarios de SSO no pueden iniciar sesión en  [!DNL Adobe Workfront] debido a varios errores"
description: Cuando reciba un error de inicio de sesión acerca del inicio de sesión único federado, su combinación de nombre de usuario y contraseña o su acceso a  [!DNL Workfront], the problem might be that your [!DNL Workfront] instancia utiliza SSO y está intentando iniciar sesión con una dirección URL incorrecta. Asegúrese de iniciar sesión con la URL correcta sin nada después de ".com".
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Error: Los usuarios de SSO no pueden iniciar sesión en [!DNL Adobe Workfront] debido a varios errores

## Problema

No puedo iniciar sesión en [!DNL Workfront] y recibí uno de los siguientes errores:

* No puede acceder a [!DNL Workfront] a través de esta pantalla de inicio de sesión. [!DNL Workfront] está configurado para el inicio de sesión único federado con SAML 2.0. Póngase en contacto con el administrador de [!DNL Workfront].
* La combinación de nombre de usuario y contraseña no es correcta. Asegúrese de que no tenga activa la tecla de mayúsculas y vuelva a intentarlo.
* No cuenta con acceso a [!DNL Workfront]. Póngase en contacto con el administrador de [!DNL Workfront] para obtener un nombre de usuario y una contraseña.

## Solución

La instancia de [!DNL Workfront] utiliza SSO y está intentando iniciar sesión a través de una dirección URL incorrecta. Asegúrese de iniciar sesión con la URL correcta sin nada después de &quot;.com&quot;

>[!TIP]
>
>Elimine los marcadores existentes que tengan direcciones URL no válidas.
