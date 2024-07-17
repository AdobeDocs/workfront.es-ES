---
product-previous: workfront-proof
product-area: documents;workfront-integrations
navigation-topic: basecamp
title: Integrar [!DNL Workfront Proof] con [!DNL Basecamp]
description: Si usas  [!DNL Basecamp] para la administración de proyectos, puedes ofrecerle a tu equipo de proyecto herramientas de revisión y aprobación más completas con [!DNL Workfront Proof].
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f6d5aef6-573d-4398-a057-ffea2e67288f
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Integrar [!DNL Workfront Proof] con [!DNL Basecamp]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Si usa [!DNL Basecamp] para la administración de proyectos, puede ofrecer al equipo del proyecto herramientas de revisión y aprobación más completas mediante [!DNL Workfront Proof].

## Explicación de la integración de [!DNL Basecamp] con [!DNL Workfront]

La integración con [!DNL Basecamp] permite a los usuarios ver, revisar y aprobar pruebas en [!DNL Basecamp]. Los usuarios pueden enviar pruebas a su cuenta de [!DNL Workfront Proof] y conectarlas con el proyecto [!DNL Basecamp]. Los revisores pueden realizar comentarios y tomar decisiones a través de [!DNL Basecamp] mediante la minirprueba incrustada en el mensaje de Basecamp.

Cuando se integra con [!DNL Workfront Proof], [!DNL Basecamp] tiene la siguiente funcionalidad de corrección:

* Los usuarios pueden revisar y aprobar las revisiones en [!DNL Basecamp Classic].
* Los usuarios tienen herramientas de revisión disponibles.
* Los equipos de revisión de proyecto reciben un mensaje en [!DNL Basecamp] con una mini prueba para su revisión y aprobación.
* Los usuarios pueden cambiar a una prueba de página completa para su revisión y aprobación.
* Los usuarios pueden agregar comentarios y marcas a las pruebas tanto de tamaño mini como completo.

  >[!NOTE]
  >
  >Una vez respondido un comentario, no se puede editar ni eliminar.

* Los revisores pueden responder a las marcas y realizadas por otros revisores.
* Se avisa a los usuarios cuando hay una nueva versión de la prueba disponible.
* Los usuarios que no sean [!DNL Workfront Proof] pueden trabajar en una revisión en [!DNL Basecamp].

La integración de [!DNL Workfront Proof] con [!DNL Basecamp] debe configurarse en dos niveles:

* Configurar [!DNL Basecamp] en [Configuración de la cuenta:](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Esto habilita la integración de Basecamp para toda la organización. Para obtener más información, consulte [Habilitar la integración de BaseCamp con [!DNL Workfront Proof]](#enabling-the-basecamp-integration-with-workfront-proof).

* Configurar [!DNL Basecamp] en [configuración personal](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings): Esto permite a los creadores y propietarios de pruebas conectarse a su cuenta personal de Basecamp y autorizar el acceso de [!DNL Workfront Proof]. Para obtener más información, consulte [Configuración personal](#configuring-personal-settings).

Puede integrar [!DNL Workfront] con [!DNL Basecamp] o [!DNL Basecamp Classic]. Cada versión de [!DNL Basecamp] usa una API diferente y, por lo tanto, requiere procedimientos de configuración diferentes.

Para obtener información sobre la configuración de [!DNL Basecamp Classic], consulte [Integración [!DNL Workfront Proof] con [!DNL Basecamp Classic].](https://support.workfront.com/knowledge/articles/115004234707/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004234707)

## Habilitando la integración de [!DNL Basecamp] con [!DNL Workfront Proof]

Como [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) o [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md), puede configurar la integración de [!DNL Basecamp] para toda la cuenta en [Configuración de la cuenta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings).

1. En [!UICONTROL Basecamp], recopile la siguiente información:

   * La URL de su cuenta de [!DNL Basecamp]
   * La dirección URL se encontró en la sección &quot;[!UICONTROL Mi información]&quot;

1. Cerrar sesión de [!DNL Basecamp].
1. Haga clic en **[!UICONTROL Configuración de la cuenta]** cerca de la esquina superior derecha.
1. Haga clic en la ficha **[!UICONTROL Integraciones]**.
1. En la sección **[!UICONTROL [!DNL Basecamp]]**, a la derecha de la integración de **[!UICONTROL [!DNL Basecamp]]**, haga clic en **[!UICONTROL Habilitar]**.

1. Junto a **[!UICONTROL [!DNL Basecamp]versión]**, verifique que **[!UICONTROL Classic versión]** sea la versión con la que está realizando la integración.

1. (Condicional) Si no se muestra ninguna dirección URL de [!DNL Basecamp], haz clic en **[!UICONTROL Editar]**, escribe la dirección URL de tu cuenta de [!DNL Basecamp], sin incluir &quot;http://&quot;, y luego haz clic en **[!UICONTROL Guardar]**.

1. En la esquina superior derecha de la ventana, haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración personal]**.

1. Haga clic en la ficha **[!UICONTROL Integraciones]**.
1. En **[!DNL Basecamp]**, a la derecha de **[!UICONTROL Integración con Basecamp]**, haga clic en **[!UICONTROL Habilitar]**.

1. En las opciones que aparecen, a la derecha de **[!UICONTROL [!DNL Basecamp]Token de API]**, haga clic en **[!UICONTROL Editar]**.

1. En el cuadro que aparece, escriba la dirección URL que se encuentra en la sección &quot;[!UICONTROL Mi información]&quot; de [!DNL Basecamp] y, a continuación, haga clic en **[!UICONTROL Guardar]**.\
   Una vez que integres [!DNL Workfront Proof] con [!DNL Basecamp], tus usuarios podrán establecer su configuración personal. Para obtener información sobre la configuración personal, consulte [Configuración personal](#configuring-personal-settings)

1. Si no puede habilitar la integración de [!DNL Basecamp], es posible que el id. de cuenta de [!DNL Workfront Proof] no sea el mismo que el id. de cuenta que usa en [!DNL Basecamp].
1. Una vez que integres [!DNL Workfront Proof] con [!DNL Basecamp], tus usuarios podrán establecer su configuración personal. Para obtener información sobre la configuración personal, consulte [Configuración personal](#configuring-personal-settings).

## Configuración personal

Después de configurar [Configuración de la cuenta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) para su organización, cada uno de los autores que cree o envíe pruebas debe establecer su [configuración personal.](https://support.workfront.com/hc/en-us/sections/115000921168-Personal-settings)

1. Vaya a **[!UICONTROL Configuración personal** **]**.

1. Abra la ficha **[!UICONTROL Integraciones]** (1).
1. Para habilitar la integración de [!DNL Basecamp], haga clic en **[!UICONTROL Habilitar]** (2).
1. Haga clic en **[!UICONTROL Conectarse a su cuenta de [!DNL Basecamp]]** (3).\
   ![Basecamp_personal_settings-integration.png](assets/basecamp-personal-settings-integration-350x174.png)

1. Inicie sesión en su cuenta de [!DNL Basecamp] (1).\
   ![Página_inicio_sesión_base.png](assets/basecamp-login-page-350x107.png)

1. Haz clic en **[!UICONTROL Sí, permitiré el acceso]** para autorizar el acceso de [!DNL Workfront Proof] a tu cuenta (2).\
   ![Página_autorización_base.png](assets/basecamp-authorization-page-350x173.png)

1. (Opcional) Cuando su integración personal esté activa (3), puede cambiar fácilmente entre sus cuentas de [!DNL Basecamp].

   1. Haciendo clic en **[!UICONTROL Cambiar [!DNL Basecamp] cuenta]** (4).\

      ![Basecamp_Switching_accounts__1_.png](assets/basecamp-switching-accounts--1--350x179.png)\
      La cuenta [!UICONTROL Switch Basecamp] le lleva a la página [!UICONTROL Configuración personal], donde puede elegir cuál de sus cuentas de [!DNL Basecamp] desea integrar con su cuenta de [!DNL Workfront Proof].

   1. Haga clic en **[!UICONTROL Volver a integrar con[!DNL Basecamp]]** (5) antes de elegir la cuenta de [!DNL Basecamp]\

      Esto actualiza la página [!UICONTROL Configuración personal] y muestra la lista más actualizada de [!DNL Basecamp] cuentas.

   1. Haga clic en **[!UICONTROL Integrar con esta cuenta]** para conectarla con [!DNL Workfront Proof].\

      ![Basecamp_Switching_accounts_2.png](assets/basecamp-switching-accounts-2-350x138.png)\
      Ahora puede agregar pruebas a [!DNL Basecamp] proyectos.
