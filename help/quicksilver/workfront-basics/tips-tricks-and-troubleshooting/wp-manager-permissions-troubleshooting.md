---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Solución de problemas de permisos de Workfront Proof Manager
description: Los perfiles de permiso disponibles en  [!DNL Adobe] Workfront para los usuarios de revisión son Administrator, Supervisor y Manager.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront] administrador de pruebas] permisos resolución de problemas

A continuación se muestran los perfiles de permiso disponibles en [!DNL Adobe Workfront] para los usuarios de revisión:

* [!UICONTROL Administrador]
* [!UICONTROL Supervisor]
* [!UICONTROL Responsable]

<!--For detailed information about these options and how to configure them, see .-->

Al conceder permisos al usuario [!UICONTROL Manager], está disponible la siguiente información para solucionar problemas:

* **PROBLEMA:** Los usuarios con permisos de [!UICONTROL Manager] no pueden ver las pruebas creadas por otros usuarios. Alternativamente, verá la pantalla [!UICONTROL Acceso denegado].

  ![](assets/access-denied-350x161.png)

  **SOLUCIÓN:** Los usuarios con permisos de [!UICONTROL Manager] deben agregarse explícitamente a las pruebas. Las pruebas siempre se deben crear a través de la ventana [!UICONTROL Advanced proofing options] y los usuarios siempre se deben agregar a través de esta opción.

* **PROBLEMA:** Los usuarios con permisos de [!UICONTROL Manager] no pueden agregar versiones de prueba a las pruebas creadas por otros usuarios (podrían enviar una prueba en el conjunto de documentos, pero las versiones NO estarían conectadas al conjunto original creado por otro usuario).\
   **SOLUCIÓN:** Los usuarios con permisos de [!UICONTROL Manager] pueden enviar las versiones a la revisión de otro usuario solamente si el usuario con permisos de [!UICONTROL Manager] tiene los dos siguientes:

   * Añadido explícitamente a las pruebas
   * Definir como [!UICONTROL autores] (función de prueba) en las pruebas

* **PROBLEMA:** Los usuarios con permisos de [!UICONTROL Manager] no pueden editar los comentarios de otros usuarios sobre una prueba que no son de su propiedad o que no crearon.\
   **SOLUCIÓN:** Si los usuarios con permisos de [!UICONTROL Manager] no son propietarios de las pruebas, pero deberían poder editar los comentarios, agréguelos como [!UICONTROL autores] (o [!UICONTROL moderadores]).\
   Estos tres tipos de permisos están disponibles en [!DNL Workfront] para las licencias de tipo [!UICONTROL Planner], [!UICONTROL Worker], [!UICONTROL Requester], [!UICONTROL Reviewer]. El administrador del sistema o el administrador de usuarios de [!DNL Workfront] pueden editar los perfiles de los usuarios y ajustar los permisos de [!DNL Workfront Proof] desde allí.
