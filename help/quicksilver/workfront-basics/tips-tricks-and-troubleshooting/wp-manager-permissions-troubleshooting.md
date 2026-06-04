---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Solución de problemas de permisos de Workfront Proof Manager
description: Los perfiles de permiso disponibles en  [!DNL Adobe] Workfront para los usuarios de revisión son Administrador, Supervisor y Gerente.
feature: Get Started with Workfront
auhor: Courtney
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
TQID: https://experienceleague.adobe.com/JIdpxOQhSJGhnwl8iqZgeJ8esHq-Bb8x8HJuEJysxRI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 100%

---

# Resolución de problemas de permisos de [!UICONTROL [!DNL Workfront] Proof Manager]

A continuación se muestran los perfiles de permiso disponibles en [!DNL Adobe Workfront] para los usuarios de revisión:

* [!UICONTROL Administrador]
* [!UICONTROL Supervisor]
* [!UICONTROL Gerente]

<!--For detailed information about these options and how to configure them, see .-->

Al conceder permisos como [!UICONTROL Gerente] a un usuario, está disponible la siguiente información para solucionar problemas:

* **PROBLEMA:** los usuarios con permisos como [!UICONTROL Gerente] no pueden ver las pruebas creadas por otros usuarios. Alternativamente, verán la pantalla [!UICONTROL Acceso denegado].

  ![](assets/access-denied-350x161.png)

  **SOLUCIÓN:** los usuarios con permisos como [!UICONTROL Gerente] deben añadirse explícitamente a las pruebas. Las pruebas siempre se deben crear a través de la ventana [!UICONTROL Opciones de revisión avanzadas] y los usuarios siempre se deben añadir a través de esta opción.

* **PROBLEMA:** los usuarios con permisos como [!UICONTROL Gerenter] no pueden añadir versiones de prueba a las pruebas creadas por otros usuarios (podrían potencialmente enviar una prueba en el conjunto de documentos, pero las versiones NO se conectarían al conjunto original creado por otro usuario).\
   **SOLUCIÓN:** los usuarios con permisos como [!UICONTROL Gerente] pueden enviar las versiones a la prueba de otro usuario solamente si el usuario con permisos como [!UICONTROL Gerente] cumple ambos de los supuestos siguientes:

   * Se han añadido explícitamente a las pruebas
   * Se han establecido como [!UICONTROL Autores] (función de prueba) en las pruebas

* **PROBLEMA:** los usuarios con permisos como [!UICONTROL Gerente] no pueden editar los comentarios de otros usuarios sobre una prueba que no es de su propiedad o que no han creado.\
   **SOLUCIÓN:** si los usuarios con permisos como [!UICONTROL Gerente] no son propietarios de las pruebas, pero deberían poder editar los comentarios, añádalos como [!UICONTROL Autores] (o [!UICONTROL Moderadores]).\
   Estos tres tipos de permisos están disponibles en [!DNL Workfront] para las licencias de tipo [!UICONTROL Planificador], [!UICONTROL Trabajador], [!UICONTROL Solicitante], [!UICONTROL Revisor]. El administrador del sistema o el administrador de usuarios de [!DNL Workfront] pueden editar los perfiles de los usuarios y ajustar los permisos de [!DNL Workfront Proof] desde allí.
