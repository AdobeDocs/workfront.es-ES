---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Error: Los usuarios de SSO no pueden iniciar sesión en [!DNL Adobe Workfront] Debido a varios errores'
description: Cuando reciba un error de inicio de sesión sobre el inicio de sesión único federado, su combinación de nombre de usuario y contraseña o su acceso a [!DNL Workfront], the problem might be that your [!DNL Workfront] instancia utiliza SSO y está intentando iniciar sesión con una dirección URL incorrecta. Asegúrese de que está iniciando sesión utilizando la dirección URL correcta sin nada después de ".com".
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 92936761-cda3-41ab-88b1-ec1cac3900d4
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 13%

---

# Error: Los usuarios de SSO no pueden iniciar sesión en [!DNL Adobe Workfront] Debido a varios errores

## Problema

No puedo iniciar sesión en [!DNL Workfront] y ha recibido uno de los siguientes errores:

* Lo sentimos, no puedes acceder [!DNL Workfront] a través de esta pantalla de inicio de sesión. [!DNL Workfront] está configurado para el inicio de sesión único federado con SAML 2.0. Póngase en contacto con su [!DNL Workfront] administrador.
* Esa combinación de nombre de usuario y contraseña no es correcta.  Compruebe que no tenga activa la tecla de mayúsculas.
* Lamentablemente no cuenta con acceso a [!DNL Workfront]. Póngase en contacto con su [!DNL Workfront] para obtener un nombre de usuario y una contraseña.

## Solución

Su [!DNL Workfront] instancia utiliza SSO y está intentando iniciar sesión a través de una dirección URL incorrecta. Asegúrese de que está iniciando sesión utilizando la dirección URL correcta sin nada después de &quot;.com&quot;

>[!TIP]
>
>Elimine los marcadores existentes que tengan direcciones URL no válidas.
