---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: box
title: Sincronizar carpetas de cuadro con [!DNL Workfront Proof]
description: Puede sincronizar una carpeta Box con una carpeta en Workfront Proof. Cada cambio que realice en los archivos de la carpeta Cuadro se reflejará en la Prueba de Workfront (por lo que cargará un nuevo archivo, agregará una nueva versión, cambiará el nombre de un archivo, etc.).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d85577f5-6aa0-40a3-a6e3-45555a3124db
source-git-commit: a6c79166c50af5bfe4c0341d003052179ce78373
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Sincronización [!DNL Box] Carpetas con [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Puede sincronizar un [!DNL Box] carpeta con una carpeta en [!DNL Workfront Proof]. Cada cambio que realice en los archivos de la carpeta Cuadro se reflejará en la Prueba de Workfront (por lo que cargará un nuevo archivo, agregará una nueva versión, cambiará el nombre de un archivo, etc.).

Para obtener más información sobre las carpetas, consulte [Administrar carpetas y su contenido en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

>[!NOTE]
>
>Solo usuarios con perfiles de [!UICONTROL Administradores] o superior pueden sincronizar carpetas. La variable [!DNL Box] usuario que carga el archivo en una carpeta sincronizada con [!DNL Workfront Proof], se convertirá en el propietario de la prueba creada en [!DNL Workfront Proof] (si son usuarios dentro de un mismo [!DNL Workfront Proof] cuenta). Si la variable [!DNL Box] el usuario es un usuario en un [!DNL Workfront Proof] o no tiene una cuenta con [!DNL Workfront Proof], la persona que creó la sincronización entre las carpetas pasará a ser la propietaria de la prueba. Para obtener más información, consulte *&quot;Edición de perfiles y permisos de usuario&quot;.*

Para sincronizar un [!DNL Box] carpeta con una carpeta en [!DNL Workfront Proof]:

1. En [!DNL Box] , vaya a la [!UICONTROL Todos los archivos y carpetas] página.
1. Haga clic en el **[!UICONTROL Más opciones]** situado junto a la carpeta con la que desea sincronizar [!DNL Workfront Proof] (1)
1. Select **[!UICONTROL Más acciones]** (2)
1. Haga clic en **[!UICONTROL Sincronizar con[!DNL Workfront Proof]]** (3)
1. En el [!UICONTROL Carpeta de sincronización] que aparece (si ha iniciado sesión en [!DNL Workfront Proof]), realice una de las siguientes acciones:

   * Haga clic en [!DNL Workfront Proof] nombre de la carpeta para sincronizarla con la carpeta correspondiente del cuadro (4).
   * Haga clic en **[!UICONTROL Nueva carpeta]** para crear una carpeta nueva en [!DNL Workfront Proof] (5).\

      ![folder_sync_2.jpg](assets/folder-sync-2-350x231.jpg)Si elige crear una carpeta nueva, se le pedirá que proporcione detalles sobre la carpeta nueva.

1. Haga clic en **[!UICONTROL Guardar]**.\
   La variable [!UICONTROL Detalles de carpeta] para la carpeta sincronizada se abre en [!DNL Workfront Proof]. Esta página contiene información sobre la carpeta.\
   Esta página también permite pausar y desactivar la sincronización. Si pone en pausa la sincronización, la carpeta ya no se actualizará con los cambios de [!DNL Box], pero la sincronización se puede reanudar en cualquier momento. Desactivar la sincronización significa que la conexión entre las carpetas está rota y que la sincronización tendría que restablecerse desde el [!DNL Box] cuenta.\
   La variable [!UICONTROL Detalles de carpeta] contiene la siguiente información y funciones en relación con su carpeta en [!DNL Box]:

   * **[!UICONTROL Pausar sincronización]**: La variable [!DNL Workfront Proof] la carpeta ya no se actualizará con los cambios de Cuadro. La sincronización se puede reanudar en cualquier momento (1).
   * **[!UICONTROL Desactivar sincronización de carpetas]**: Se ha perdido la conexión entre carpetas y la sincronización tendrá que configurarse de nuevo desde el [!DNL Box] cuenta (2).

   * Solo el usuario que inició la sincronización de carpetas puede desactivarla o ponerla en pausa. Para obtener más información, consulte  [Administrar carpetas y su contenido en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).
   * **Vaya a [!DNL Box] carpeta**: Si ha compartido la dirección URL de la carpeta (en la [!DNL Box] opciones de carpeta), esta opción estará disponible y le llevará directamente al [!DNL Box] carpeta (3).
   * **[!UICONTROL Detalles de sincronización de carpetas]**: Esta sección contiene información sobre la variable [!DNL Box] carpeta (4).
   * **[!UICONTROL [!DNL Box]vínculo de carpeta]**: Dirección URL de [!DNL Box] carpeta (5).
   * **[!UICONTROL Actividad]:** Muestra los registros de actividad de la variable [!DNL Workfront Proof] carpeta, aquí puede comprobar quién inició la sincronización de carpetas (6).
   * ![folder_details__1_.jpg](assets/folder-details--1--350x324.jpg)

>[!NOTE]
>
>* También puede sincronizar el [!DNL Box] de [!UICONTROL Opciones de carpeta] para abrir el Navegador.
>* Si tiene su propia marca [!DNL Workfront Proof] inicio de sesión, se le redirigirá a esa página en lugar de a la [!DNL Workfront Proof] página de inicio de sesión. Consulte los artículos incluidos en [Marcas](https://support.workfront.com/hc/en-us/sections/115000921208-Branding) si necesita más información.
>* Si ha activado la variable [!UICONTROL Inicio de sesión único (SSO)] en su [!DNL Workfront Proof] , se le dirigirá a la página de inicio de sesión de SSO y se le pedirá que introduzca sus credenciales de inicio de sesión de SSO, pero solo si está utilizando la misma dirección de correo electrónico para su [!DNL Box] cuenta y [!DNL Workfront Proof]. Si necesita más información, consulte [[!UICONTROL Inicio de sesión único] en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).
>* Si no utiliza la misma dirección de correo electrónico para ambas [!DNL Box] y su [!DNL Workfront Proof] tenga en cuenta que siempre se le dirigirá a la [!DNL Workfront Proof] página de inicio de sesión.
>



