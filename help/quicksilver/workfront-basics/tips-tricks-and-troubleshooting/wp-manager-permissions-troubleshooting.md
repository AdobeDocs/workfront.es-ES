---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Solución de problemas de permisos del administrador de pruebas de Workfront
description: 'A continuación se muestran los perfiles de permisos disponibles en [!DNL Adobe] Workfront para probar usuarios: EDITE ME.'
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] Administrador de pruebas] solución de problemas de permisos

A continuación se muestran los perfiles de permisos disponibles en [!DNL Adobe Workfront] para probar a los usuarios:

* [!UICONTROL Administrador]
* [!UICONTROL Supervisor]
* [!UICONTROL Gerente]

<!--For detailed information about these options and how to configure them, see .-->

Al conceder un usuario [!UICONTROL Administrador] , la siguiente información de solución de problemas está disponible:

* **PROBLEMA:** Usuarios con [!UICONTROL Administrador] Los permisos de no pueden ver pruebas creadas por otros usuarios. En su lugar, ven la variable [!UICONTROL Acceso denegado] en el Navegador.

   ![](assets/access-denied-350x161.png)

   **SOLUCIÓN:** Usuarios con [!UICONTROL Administrador] Los permisos de deben agregarse explícitamente a las pruebas. Las pruebas siempre se deben crear mediante la variable [!UICONTROL Opciones de prueba avanzadas] y los usuarios siempre deben agregarse mediante esta opción.

* **PROBLEMA:** Usuarios con [!UICONTROL Administrador] Los permisos de no pueden añadir versiones de prueba a las pruebas creadas por otros usuarios (podrían enviar una prueba en el conjunto de documentos, pero las versiones NO se conectarían al conjunto original creado por otro usuario).\
   **SOLUCIÓN:** Usuarios con [!UICONTROL Administrador] Los permisos de pueden enviar las versiones a la prueba de otro usuario solo si el usuario con [!UICONTROL Administrador] permisos cuando se dan los dos casos siguientes:

   * Se agrega explícitamente a las pruebas
   * Establecer como [!UICONTROL Autores] (función de prueba) en las pruebas

* **PROBLEMA:** Usuarios con [!UICONTROL Administrador] Los permisos de no pueden editar comentarios de otros usuarios en una prueba que no son de su propiedad o que no han creado.\
   **SOLUCIÓN:** Si los usuarios con [!UICONTROL Administrador] Los permisos de no son propietarios de las pruebas, pero deben poder editar comentarios y añadirlos como [!UICONTROL Autores] (o [!UICONTROL Moderadores]).\
   Estos tres tipos de permisos están disponibles en [!DNL Workfront] para [!UICONTROL Planificador], [!UICONTROL Trabajador], [!UICONTROL Solicitante], [!UICONTROL Revisor] licencias de tipo . Administrador del sistema o administrador de usuarios en [!DNL Workfront] puede editar los perfiles de los usuarios y ajustar [!DNL Workfront Proof] permisos desde allí.
