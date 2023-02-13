---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Mover usuarios entre cuentas mediante [!DNL Workfront Proof]
description: Si es [!DNL Workfront Proof] administrador y tiene una o más cuentas satélite conectadas a su cuenta principal, puede mover los usuarios entre todas estas cuentas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# Mover usuarios entre cuentas mediante [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Si es [!DNL Workfront] Administrador de pruebas y tiene una o más cuentas satélite conectadas a su cuenta principal, puede mover los usuarios entre todas estas cuentas.

## Mover usuarios entre cuentas conectadas

1. Haga clic en **[!UICONTROL Configuración]** > **[!UICONTROL Configuración de la cuenta]**.

1. Abra el **[!UICONTROL Usuarios]** pestaña .
1. Haga clic en el **[!UICONTROL Mover usuario]** (1). ![Move_user2.png](assets/move-user2-350x95.png)

1. En el cuadro Mover usuario que aparece, confirme el usuario que desea mover (1).
1. Seleccione una cuenta de destino de la lista de cuentas conectadas (2).
1. Asigne el permiso de perfil (3) que este usuario debe tener en la nueva cuenta.
1. Seleccione un usuario (4) que deba hacerse cargo de los elementos que no se moverán.
Esto incluye los artículos que decidirá dejar en la cuenta antigua y los artículos que no se pueden mover (consulte [Elementos que no se pueden mover](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) más abajo).

1. Marque las casillas de verificación si desea mover las pruebas (5) y los archivos (6) junto con el usuario.
1. Cree un nombre para la carpeta (7) en la que se colocarán todos los elementos movidos en la nueva cuenta.
1. Haga clic en **[!UICONTROL Mover usuario]** (8) para iniciar el proceso.
   ![Mover_usuarios_pop-up.png](assets/moving-users-pop-up-350x380.png)

Si decide mover el usuario sin sus pruebas y archivos, esta acción se realizará de inmediato. Si elige mover al usuario junto con sus pruebas y archivos, el perfil del usuario se reasignará de inmediato, pero las pruebas y los archivos aparecerán gradualmente en la cuenta de destino, ya que esta operación requiere tiempo para transferir los datos.

Dependiendo del número de archivos y pruebas, el proceso de movimiento puede tardar desde unos minutos hasta unas pocas horas.

>[!NOTE]
>
>Si sospecha que el proceso tarda más de lo esperado o que las pruebas y/o archivos movidos no aparecen en la nueva cuenta, póngase en contacto con nuestro equipo de asistencia técnica.

## Elementos que no se pueden mover

### Carpetas creadas o en propiedad por el usuario movido

Debido a la naturaleza de los distintos permisos aplicados a las carpetas y su contenido (por ejemplo, pueden compartirse con otros usuarios y cuentas), no podemos mover estructuras de carpetas con el usuario.

Si el usuario movido es propietario de una carpeta, la propiedad se transfiere al usuario seleccionado (4) en la ventana emergente &quot;Mover usuario&quot;.

>[!NOTE]
>
>Si el usuario movido ha creado una carpeta, seguirá siendo su creador; solo se transferirá la propiedad. La carpeta permanecerá visible para el usuario movido en la barra lateral de su nueva cuenta. El usuario movido seguirá teniendo acceso de solo lectura a los elementos colocados dentro de estas carpetas.

Si no desea que el usuario movido mantenga estos permisos o si el usuario movido no desea ver sus carpetas antiguas en la cuenta antigua, la solución sería eliminar las carpetas de la siguiente manera:

1. Cree una nueva carpeta en la cuenta antigua.
1. Mueva todos los elementos de las carpetas del usuario movidas al recién creado.
1. Elimine todas las carpetas que queden del usuario movido.

### Conjuntos de versiones con diferentes propietarios

Si una prueba tiene unas pocas versiones y cada una de ellas es propiedad de un usuario diferente, las versiones que posee el usuario movido no se moverán a su lado. La propiedad de estas versiones se transferirá a otro usuario según su elección (4) en el cuadro Mover usuario . (Para obtener más información, consulte ).

>[!NOTE]
>
>Un usuario movido debe ser propietario de todas las versiones de prueba del conjunto para que la prueba se pueda mover.

### Grupos

Los grupos deberán ser recreados por el usuario movido en su nueva cuenta. Para obtener más información, consulte [Crear grupos de prueba usando [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### Vistas personalizadas

El usuario movido en su nueva cuenta deberá volver a crear las vistas personalizadas personales. Para obtener más información, consulte [Crear y administrar vistas personalizadas en [!DNL Workfront Proof] Prueba](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Campos personalizados

Los campos personalizados no se pueden mover y se perderán datos de campos personalizados, por lo que asegúrese de generar los informes sobre los elementos necesarios antes del movimiento.

### Plantillas de flujo de trabajo automatizadas

Es necesario volver a crear las plantillas de flujo de trabajo automatizadas en la nueva cuenta, pero las fases se conservarán en las pruebas movidas creadas con las plantillas.

### Acciones sobre los comentarios

Las acciones en Comentarios permanecerán en las pruebas, pero ya no será posible filtrarlas por ellas. La solución sería crear acciones coincidentes en la nueva cuenta y volver a marcar los comentarios con las nuevas acciones si es necesario.
