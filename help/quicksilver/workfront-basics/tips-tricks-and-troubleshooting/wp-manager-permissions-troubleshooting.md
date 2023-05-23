---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Solución de problemas de permisos de Workfront Proof Manager
description: Los perfiles de permiso disponibles en [!DNL Adobe] Workfront para revisar usuarios es Administrator, Supervisor y Manager.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 114d306d99ae9ba0a18abd63a6137ad0568ab202
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] Administrador de revisiones] permisos resolución de problemas

A continuación se muestran los perfiles de permiso disponibles en [!DNL Adobe Workfront] para usuarios de revisión:

* [!UICONTROL Administrador]
* [!UICONTROL Supervisor]
* [!UICONTROL Gerente]

<!--For detailed information about these options and how to configure them, see .-->

Al conceder a un usuario [!UICONTROL Gerente] Para obtener más información sobre la solución de problemas, consulte:

* **PROBLEMA:** Usuarios con [!UICONTROL Gerente] Los permisos de no pueden ver las pruebas creadas por otros usuarios. En su lugar, ven el [!UICONTROL Acceso denegado] pantalla.

   ![](assets/access-denied-350x161.png)

   **SOLUCIÓN:** Usuarios con [!UICONTROL Gerente] Los permisos de se deben añadir explícitamente a las pruebas. Las pruebas siempre deben crearse mediante la variable [!UICONTROL Opciones avanzadas de revisión] y los usuarios siempre se deben añadir mediante esta opción.

* **PROBLEMA:** Usuarios con [!UICONTROL Gerente] Los permisos de no pueden agregar versiones de prueba a las pruebas creadas por otros usuarios (podrían enviar una prueba en el conjunto de documentos, pero las versiones NO estarían conectadas al conjunto original creado por otro usuario).\
   **SOLUCIÓN:** Usuarios con [!UICONTROL Gerente] Los permisos de solo pueden enviar las versiones a la revisión de otro usuario si el usuario con [!UICONTROL Gerente] permisos cuando se cumplen las dos condiciones siguientes:

   * Añadido explícitamente a las pruebas
   * Establecer como [!UICONTROL Autores] (función de prueba) en las pruebas

* **PROBLEMA:** Usuarios con [!UICONTROL Gerente] Los permisos de no pueden editar comentarios de otros usuarios sobre una prueba que no son de su propiedad o que no han creado.\
   **SOLUCIÓN:** Si los usuarios con [!UICONTROL Gerente] Los permisos de no son propietarios de las pruebas, pero deben poder editar los comentarios y agregarlos como [!UICONTROL Autores] (o [!UICONTROL Moderadores]).\
   Estos tres tipos de permisos están disponibles en [!DNL Workfront] para [!UICONTROL Planificador], [!UICONTROL Trabajador], [!UICONTROL Solicitante], [!UICONTROL Revisor] escribir licencias. Administrador del sistema o Administrador de usuarios en [!DNL Workfront] Puede editar los perfiles de los usuarios y ajustar [!DNL Workfront Proof] permisos desde allí.
