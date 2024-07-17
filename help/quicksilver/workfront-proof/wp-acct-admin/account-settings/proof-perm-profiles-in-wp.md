---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Perfiles de permisos de revisión en Workfront Proof
description: Como administrador de Workfront o de Workfront Proof, puede asignar un perfil de permisos de pruebas a un usuario para especificar las capacidades de prueba que tendrá el usuario para todas las pruebas del sistema. Para obtener información sobre la configuración del perfil de permisos de pruebas de un usuario, consulte Configuración del perfil de permisos de pruebas de un usuario en Workfront Proof
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1764'
ht-degree: 0%

---

# Perfiles de permisos de revisión en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], vea [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Como administrador de [!DNL Workfront] o [!DNL Workfront Proof], puede asignar un perfil de permisos de revisión a un usuario para especificar las capacidades de revisión que tendrá el usuario para todas las revisiones del sistema. Para obtener información acerca de cómo configurar el perfil de permisos de pruebas de un usuario, vea [Configurar el perfil de permisos de pruebas de un usuario en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>También puede hacer lo siguiente:
>
>* Conceder a los usuarios funciones específicas en pruebas individuales. Para obtener más información acerca de los roles de prueba, consulte [Administrar roles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Cree perfiles personalizados para los usuarios de su organización. Para obtener más información, vea [Configurar perfiles personalizados en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>

La siguiente tabla muestra los permisos disponibles con cada Perfil de permisos de prueba.

| **Elementos propios** |  |  |  |  | **Elementos de otros usuarios** |  |  | **Administrador** | **Facturación** |
|---|---|---|---|---|---|---|---|---|---|
|   | **Agregar** | **Vista** | **Editar** | **Eliminar** | **Vista** | **Editar** | **Eliminar** | **Editar y eliminar** | **Editar** |
| Administrador de facturación | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| Administrador | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| Supervisor | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| Gerente | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| Observador |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Visitante |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style="table-layout:auto"}

Tenga en cuenta lo siguiente sobre las funciones y los permisos:

* Los permisos de perfil asignados están relacionados únicamente con los usuarios y elementos de su propia cuenta. La excepción se produce en el caso de las cuentas satélite, en las que el administrador y el administrador de facturación de las cuentas principales (hub) pueden acceder y administrar la configuración y la facturación de esas cuentas desde el nivel de cuenta hub.
* Los administradores y administradores de facturación pueden eliminar usuarios. Esto solo se puede hacer en Configuración de cuenta.
* Cuando los administradores de facturación y los administradores ven las pruebas que son propiedad de otros usuarios en su cuenta, los ven con la función de revisor.
* Con la función Solo lectura, los administradores de facturación y los administradores pueden acceder a las pruebas en carpetas compartidas con ellos o en carpetas creadas por ellos.

Las secciones siguientes describen cada perfil y los permisos asociados con el perfil en una configuración estándar de [!DNL Workfront Proof]:

* [Administrador de facturación](#billing-administrator)
* [Administrador](#administrator)
* [Supervisor](#supervisor)
* [Responsable](#manager)
* [Observador](#observer)
* [Visitante](#visitor)
* [Invitado](#guest)

## Administrador de facturación {#billing-administrator}

Los administradores de facturación tienen acceso a la [configuración de la cuenta en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] Página de facturación](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) y tienen los permisos siguientes:

![](assets/cleaner2.png)Puede generar pruebas, cargar archivos y crear carpetas. Para obtener más información, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Cargar archivos y contenido web en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) y [Crear carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Pueden ver, editar y eliminar sus propias pruebas y archivos.

![](assets/cleaner2.png)Puede ver, editar y eliminar pruebas y archivos creados por todos los usuarios de la organización.

![](assets/cleaner2.png)Puede eliminar las carpetas públicas de otros usuarios. Para obtener más información, consulte [Administrar carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Tiene derechos de edición en todas las pruebas creadas en la cuenta.

![](assets/cleaner2.png)Se puede establecer como propietario de Dropzone. Para obtener más información, consulte [Configurar la Dropzone en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Puede acceder a la página de facturación y editar los detalles de facturación. Para obtener más información, consulte [La [!DNL Workfront Proof] página de facturación](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)Puede acceder a la página Configuración de la cuenta y editar los detalles de la cuenta. Para obtener más información, consulte [Configuración de la cuenta en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Puede vaciar la papelera. Para obtener más información, vea [Restaurar y vaciar la papelera en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Puede agregar, editar y eliminar usuarios.

![](assets/cleaner2.png)Puede crear grupos y agregar nuevos contactos.

![](assets/cleaner2.png)Puede eliminar contactos.

![](assets/cleaner2.png)Puede editar pruebas si no hay respuestas en ellas.

![](assets/no2.png)No se pueden editar las respuestas de revisión.

![](assets/no2.png)No se pueden eliminar las carpetas privadas de otros usuarios. Para obtener más información, consulte [Administrar carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Para obtener información acerca de la configuración de la cuenta, vea [Configuración de la cuenta en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Para obtener información sobre facturación, consulte [La [!DNL Workfront Proof] página de facturación](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Administrador {#administrator}

Los administradores tienen acceso a [Configuración de la cuenta](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings) y tienen los permisos siguientes:

![](assets/cleaner2.png)Puede crear pruebas, cargar archivos y crear carpetas. Para obtener más información, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Cargar archivos y contenido web en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) y [Crear carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Pueden ver, editar y eliminar las pruebas y los archivos que han creado.

![](assets/cleaner2.png)Puede ver, editar y eliminar pruebas y archivos creados por todos los usuarios de la organización.

![](assets/cleaner2.png)Puede eliminar las carpetas públicas de otros usuarios. Para obtener más información, consulte [Administrar carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Tiene derechos de edición en todas las pruebas creadas en la cuenta.

![](assets/cleaner2.png)Se puede establecer como propietario de Dropzone. Para obtener más información, consulte [Configurar la Dropzone en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Puede acceder a la página Configuración de la cuenta y editar los detalles de la cuenta. Para obtener más información, consulte [Configuración de la cuenta en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Puede vaciar la papelera. Para obtener más información, vea [Restaurar y vaciar la papelera en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Puede agregar, editar y eliminar usuarios.

![](assets/cleaner2.png)Puede crear grupos y agregar nuevos contactos.

![](assets/cleaner2.png)Puede eliminar contactos.

![](assets/cleaner2.png)Puede editar pruebas si no hay respuestas en ellas.

![](assets/no2.png)No se pueden editar las respuestas de revisión.

![](assets/no2.png)No se pueden eliminar las carpetas privadas de otros usuarios. Para obtener más información, consulte [Administrar carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)No se puede acceder a la página Facturación ni editar los detalles de facturación. Para obtener más información, consulte [La [!DNL Workfront Proof] página de facturación](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisor {#supervisor}

Los supervisores tienen los siguientes permisos:

![](assets/cleaner2.png)Puede crear pruebas, cargar archivos y crear carpetas. Para obtener más información, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Cargar archivos y contenido web en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) y [Crear carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Pueden ver, editar y eliminar sus propias pruebas y archivos creados.

![](assets/cleaner2.png)Puede ver, editar y eliminar pruebas y archivos creados por todos los usuarios de la organización.

![](assets/cleaner2.png)Puede eliminar las carpetas públicas de otros usuarios. Para obtener más información, consulte [Administrar carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Tiene derechos de edición en todas las pruebas creadas en la cuenta.

![](assets/cleaner2.png)Se puede establecer como propietario de Dropzone. Para obtener más información, consulte [Configurar la Dropzone en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Puede crear grupos y agregar nuevos contactos.

![](assets/cleaner2.png)Puede eliminar contactos.

![](assets/cleaner2.png)Puede editar pruebas si no hay respuestas en ellas.

![](assets/no2.png)No se pueden editar las respuestas de revisión.

![](assets/no2.png)No se pueden eliminar las carpetas privadas de otros usuarios. Para obtener más información, consulte [Carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)No se puede obtener acceso a la página Facturación o a la configuración de la cuenta. Para obtener más información, consulte [La [!DNL Workfront Proof] página de facturación](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) y [Configuración de la cuenta en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)No se pueden agregar, editar ni eliminar usuarios.

![](assets/no2.png)No se puede vaciar la papelera. Para obtener más información, vea [Restaurar y vaciar la papelera en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Gerente {#manager}

Los responsables tienen los siguientes permisos:

![](assets/cleaner2.png)Puede crear pruebas, cargar archivos y crear carpetas. Para obtener más información, consulte [Generar pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Cargar archivos y contenido web en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) y [Crear carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Pueden ver, editar y eliminar sus propias pruebas y archivos que crean o son de su propiedad.

![](assets/cleaner2.png)Puede ver, revisar y aprobar pruebas de otros usuarios que se han compartido explícitamente con ellos (derechos de solo lectura para todo lo que hay en una carpeta compartida). Para obtener más información, consulte [Administrar roles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Puede crear grupos y agregar un nuevo contacto.

![](assets/no2.png)No se pueden ver, editar ni eliminar pruebas ni archivos creados por otros usuarios de la organización.

![](assets/no2.png)No se pueden editar pruebas o respuestas.

![](assets/no2.png)No se pueden eliminar las carpetas privadas de otros usuarios. Para obtener más información, consulte [Administrar carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)No se pueden eliminar las carpetas públicas de otros usuarios. Para obtener más información, consulte [Administrar carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)No se puede obtener acceso a la página Facturación o a la configuración de la cuenta. Para obtener más información, consulte [La [!DNL Workfront Proof] página de facturación](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) y [Configuración de la cuenta en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)No se puede establecer como propietario de Dropzone. Para obtener más información, consulte [Configurar la Dropzone en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)No se puede vaciar la papelera. Para obtener más información, vea [Restaurar y vaciar la papelera en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)No se pueden agregar, editar ni eliminar usuarios.

![](assets/no2.png)No se pueden eliminar contactos.

### Observador {#observer}

Los observadores tienen los siguientes permisos:

![](assets/cleaner2.png)Puede ver, revisar y aprobar pruebas de otros usuarios que se han compartido explícitamente con ellos (derechos de solo lectura para todo lo que hay en una carpeta compartida). Para obtener más información, consulte [Administrar roles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Puede ver los archivos que se han compartido explícitamente con ellos.

![](assets/cleaner2.png) puede ver contactos y grupos

![](assets/no2.png)No se pueden crear pruebas, cargar archivos ni crear carpetas. Para obtener más información, consulte [Cargar archivos y contenido web a [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)No se pueden ver, editar ni eliminar pruebas ni archivos creados por otros usuarios de la organización.

![](assets/no2.png)No se pueden editar pruebas o respuestas.

![](assets/no2.png)No se puede eliminar ningún elemento creado en la organización.

![](assets/no2.png)No se puede obtener acceso a la página Facturación o a la configuración de la cuenta. Para obtener más información, consulte [La [!DNL Workfront Proof] página de facturación](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) y [Configuración de la cuenta en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)No se puede establecer como propietario de Dropzone. Para obtener más información, consulte [Configurar la Dropzone en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)No se puede vaciar la papelera. Para obtener más información, vea [Restaurar y vaciar la papelera en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)No se pueden agregar, editar ni eliminar usuarios.

![](assets/no2.png)No se pueden crear grupos ni agregar nuevos contactos.

![](assets/no2.png)No se pueden eliminar contactos.

>[!NOTE]
>
>Los menús y las funciones disponibles para los observadores son limitados.
>
>* Los observadores no ven el menú Encabezado ni el menú Nuevo verde en su panel
>* Los observadores no ven los siguientes vínculos en su Configuración: Configuración de cuenta, Facturación
>

### Visitante {#visitor}

Los visitantes tienen los siguientes permisos:

![](assets/cleaner2.png)Puede ver, revisar y aprobar pruebas de otros usuarios que se han compartido explícitamente con ellos (derechos de solo lectura para todo lo que hay en una carpeta compartida). Para obtener más información, consulte [Administrar roles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Puede ver los archivos que se han compartido explícitamente con ellos.

![](assets/no2.png) No se pueden ver contactos y grupos

![](assets/no2.png)No se pueden crear pruebas, cargar archivos ni crear carpetas. Para obtener más información, consulte [Cargar archivos y contenido web a [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)No se pueden ver, editar ni eliminar pruebas ni archivos creados por otros usuarios de la organización.

![](assets/no2.png)No se pueden editar pruebas o respuestas.

![](assets/no2.png)No se puede eliminar ningún elemento creado en la organización.

![](assets/no2.png)No se puede obtener acceso a la página Facturación o a la configuración de la cuenta. Para obtener más información, consulte [La [!DNL Workfront Proof] página de facturación](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) y [Configuración de la cuenta en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)No se puede establecer como propietario de Dropzone. Para obtener más información, consulte [Configurar la Dropzone en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)No se puede vaciar la papelera. Para obtener más información, vea [Restaurar y vaciar la papelera en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)No se pueden agregar, editar ni eliminar usuarios.

![](assets/no2.png)No se pueden crear grupos ni agregar nuevos contactos.

![](assets/no2.png)No se pueden eliminar contactos.

>[!NOTE]
>
>Los menús y las funciones disponibles para los visitantes son limitados.
>
>* Los visitantes no ven el menú Encabezado ni el menú Nuevo verde en su panel
>* Los visitantes no ven los siguientes vínculos en su configuración: Configuración de cuenta, Facturación
>

### Invitado {#guest}

El perfil Invitado se utiliza para dar acceso a las pruebas a los revisores que no tienen su propia cuenta de Workfront Proof. Los huéspedes pueden acceder a las pruebas compartidas con ellos directamente a través de sus notificaciones personales por correo electrónico.

![](assets/cleaner2.png)Pueden ver, revisar y aprobar pruebas que se compartan explícitamente con ellos.

![](assets/cleaner2.png)Puede ver los archivos que se han compartido explícitamente con ellos.

![](assets/no2.png)No se puede obtener acceso al panel.

![](assets/no2.png)No se pueden compartir carpetas con ellos. Para obtener más información, consulte [Administrar carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)No se puede agregar como autores o moderadores a las pruebas. Para obtener más información, consulte [Administrar roles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Los invitados no son usuarios de Workfront Proof, por lo que no pueden ver todas las pruebas compartidas con ellos en su propio panel.

## Editar el perfil de permiso de revisión de un usuario

Los administradores y administradores de facturación pueden editar los perfiles de permiso de todos los usuarios de la cuenta.

1. Para buscar el usuario que desea editar, realice una de las siguientes acciones:

   * Vaya a **[!UICONTROL Configuración de la cuenta]** y luego haga clic en la ficha **[!UICONTROL Usuarios]**.

   * Vaya a la página **[!UICONTROL Contactos]**.

1. Haga clic en el nombre del usuario cuyos permisos desee editar. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Haga clic en el menú desplegable **[!UICONTROL Perfil de permisos]** y seleccione un nuevo perfil de permisos. :

   ![Captura de pantalla_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   Los perfiles de permisos son Administrador, Supervisor, Responsable y Observador.

1. Haga clic en cualquier lugar fuera del menú para guardar.

>[!NOTE]
>
>Los administradores no pueden asignar el perfil Administrador de facturación. Puede encontrar una lista de cambios de perfil en los siguientes registros:
>
>* Registros de actividad de la cuenta
>* El registro de perfil del usuario (accesible solo para ese usuario)
>

Para obtener más información sobre los registros de actividad, consulte [Explicación de la [!DNL Workfront Proof] pista de auditoría de actividad](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
