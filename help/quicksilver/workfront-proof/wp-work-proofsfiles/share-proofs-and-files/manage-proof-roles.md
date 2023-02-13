---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Administrar funciones de prueba en [!DNL Workfront Proof]
description: Las funciones de prueba permiten conceder permisos a los usuarios limitados por el perfil de permisos configurado en su perfil de usuario. (Para obtener más información sobre los perfiles de permisos, consulte Perfiles de permisos de prueba en [!DNL Workfront Proof].)
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 1%

---

# Administrar funciones de prueba en [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

Las funciones de prueba permiten conceder permisos a los usuarios limitados por el perfil de permisos configurado en su perfil de usuario. (Para obtener más información sobre los perfiles de permisos, consulte [Perfiles de permisos de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Las funciones de prueba son diferentes a los perfiles de cuenta. El perfil de la cuenta se relaciona con el nivel de permiso general que tiene en la cuenta y afectará a los derechos que tiene sobre todas las pruebas de la cuenta, incluso las que no se han compartido explícitamente con usted.

Para obtener más información, consulte [Perfiles de permisos de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Acerca de las funciones de prueba

Las siguientes funciones de prueba se conceden a los usuarios para una prueba individual en el momento en que se invita al usuario a revisar la prueba:

* [Solo lectura](#read-only)
* [Revisor](#reviewer)
* [Aprobador](#approver)
* [Revisor y aprobador](#reviewer-approver)
* [Autor](#author)
* [Moderador](#moderator)

La función de prueba define qué acciones puede realizar un revisor en relación con esa prueba específica.

Por ejemplo, si es un revisor, se le pedirá que revise la prueba añadiendo marcas y comentarios. Si es un revisor y aprobador, se le pedirá que revise la prueba y que tome también una decisión al respecto.

Algunas funciones de prueba otorgan a un revisor derechos de edición en la prueba (incluso si su perfil de cuenta no lo tiene) y le permiten utilizar algunas funciones adicionales, como agregar acciones en los comentarios, crear nuevas versiones y agregar más revisores a la prueba.

Para obtener más información, consulte los siguientes artículos:

* [Usar acciones en comentarios de prueba](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Compartir una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Solo lectura

{#read-only}

![clear.png](assets/cleaner.png) Puede ver una prueba

![no.png](assets/no.png) No se pueden agregar marcas

![no.png](assets/no.png) No se pueden agregar comentarios

![no.png](assets/no.png) No se puede tomar una decisión

![no.png](assets/no.png) No se pueden eliminar los comentarios de otros

![no.png](assets/no.png) No tiene derechos de edición en la prueba

>[!NOTE]
>
>Si una carpeta se comparte con un usuario de [!DNL Workfront Proof], se les otorgarán automáticamente derechos de solo lectura a todos los elementos existentes y posteriormente agregados en la carpeta.

Para obtener más información, consulte [Compartir carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### Revisor {#reviewer}

![clear.png](assets/cleaner.png) Puede ver una prueba

![clear.png](assets/cleaner.png) Pueden agregar marcas

![clear.png](assets/cleaner.png) Puede agregar comentarios

![[!DNL cleaner].png](assets/cleaner.png) Puede editar sus propios comentarios si no hay respuestas

![no.png](assets/no.png) No se puede tomar una decisión

![no.png](assets/no.png) No se pueden editar ni eliminar los comentarios realizados por otros

![no.png](assets/no.png) No tiene derechos de edición en la prueba

### Aprobador {#approver}

![clear.png](assets/cleaner.png) Puede ver una prueba

![clear.png](assets/cleaner.png) Puede tomar una decisión

![no.png](assets/no.png) No se pueden agregar marcas

![no.png](assets/no.png) No se pueden agregar comentarios

![no.png](assets/no.png) No se pueden editar ni eliminar los comentarios realizados por otros

![no.png](assets/no.png) No tiene derechos de edición en la prueba

### Revisor y aprobador {#reviewer-approver}

![clear.png](assets/cleaner.png) Puede ver una prueba

![clear.png](assets/cleaner.png) Pueden agregar marcas

![clear.png](assets/cleaner.png) Puede agregar comentarios

![[!DNL cleaner].png](assets/cleaner.png) Puede editar sus propios comentarios si no hay respuestas

![clear.png](assets/cleaner.png) Puede tomar una decisión

![no.png](assets/no.png) No se pueden editar ni eliminar los comentarios realizados por otros

![no.png](assets/no.png) No tiene derechos de edición en la prueba

### Autor {#author}

![clear.png](assets/cleaner.png) Pueden agregar marcas

![clear.png](assets/cleaner.png) Puede agregar comentarios

![[!DNL cleaner].png](assets/cleaner.png) Puede editar sus propios comentarios si no hay respuestas

![clear.png](assets/cleaner.png) Puede tomar una decisión

![clear.png](assets/cleaner.png) Puede enviar nuevas versiones

![clear.png](assets/cleaner.png) Puede crear una copia de la prueba

![clear.png](assets/cleaner.png) Puede compartir la prueba con otras personas

![clear.png](assets/cleaner.png) Puede aplicar acciones en los comentarios

![clear.png](assets/cleaner.png) Puede resolver comentarios

![no.png](assets/no.png) No se pueden editar ni eliminar los comentarios realizados por otros

>[!NOTE]
>
>Esta función solo se puede asignar a usuarios de [!DNL Workfront Proof]

### Moderador {#moderator}

![clear.png](assets/cleaner.png) Pueden agregar marcas

![clear.png](assets/cleaner.png) Puede agregar comentarios

![[!DNL cleaner].png](assets/cleaner.png) Puede editar sus propios comentarios si no hay respuestas

![clear.png](assets/cleaner.png) Puede tomar una decisión

![clear.png](assets/cleaner.png) Puede enviar nuevas versiones

![clear.png](assets/cleaner.png) Se pueden agregar nuevos revisores

![clear.png](assets/cleaner.png) Puede aplicar acciones en los comentarios

![clear.png](assets/cleaner.png) Puede resolver comentarios

![clear.png](assets/cleaner.png) Pueden eliminar comentarios y respuestas sobre la prueba (realizados por ellos mismos o por otros)

* Al eliminar el primer comentario en un subproceso de comentario, se eliminará todo el subproceso.
* Al eliminar respuestas en el hilo de comentarios, solo se eliminará esa respuesta

![no.png](assets/no.png) No se pueden editar los comentarios realizados por otros

Esta función permite que la persona administre y modere los comentarios de prueba, lo que les da la oportunidad de mantener solo los comentarios relevantes en la prueba y eliminar los comentarios no relevantes.

>[!NOTE]
>
>Esta función solo se puede asignar a usuarios de [!DNL Workfront Proof].

## Asignación de funciones de prueba

Puede asignar funciones de prueba al crear pruebas nuevas, crear versiones nuevas de pruebas existentes o en pruebas existentes.

* [Nuevas pruebas](#new-proofs)
* [Nuevas versiones](#new-versions)
* [Pruebas existentes](#existing-proofs)

### Nuevas pruebas {#new-proofs}

Se pueden asignar funciones de prueba a los revisores en la variable [!UICONTROL Nueva prueba] durante el proceso de creación de la prueba (1).

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Nuevas versiones {#new-versions}

Al crear una Nueva versión de una prueba, se muestran automáticamente los revisores de la versión anterior (con la misma función que la versión anterior).

Puede editar las funciones de prueba aplicadas a los revisores al crear la nueva versión (1).

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Pruebas existentes {#existing-proofs}

Si desea cambiar la función de una persona en una prueba existente, puede hacerlo en la [!UICONTROL Detalles de la prueba] mediante la edición en línea de su función en la sección de flujo de trabajo (1):

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## Comprobación de funciones en el visualizador de pruebas

Puede comprobar la función de un revisor directamente desde el visor de pruebas (1) y editarlo (2) si es necesario.

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Funciones de prueba predeterminadas

Puede establecer la función de prueba predeterminada en la variable [!DNL Proofing Defaults] en su Configuración personal. Esto significa que, cuando se le agrega a una prueba, la función de prueba predeterminada se rellena automáticamente. Tenga en cuenta que esta función puede ser modificada en el nivel de prueba por un usuario con derechos de edición en una prueba.

>[!NOTE]
>
>Solo los usuarios con perfiles de administrador o administrador de facturación pueden cambiar los valores predeterminados de prueba para otros usuarios de su cuenta.

Para obtener más información, consulte [Ajustes personales en [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Creadores y propietarios

Los creadores y propietarios tienen derechos de edición completos en la prueba.

* [Creadores](#creators)
* [Propietarios](#owners)

### Creadores {#creators}

El creador de la prueba es la persona que carga la prueba en la primera instancia. El creador de pruebas se mostrará automáticamente en la lista de personas para la prueba (en su función predeterminada).

En el [!UICONTROL Nueva prueba] puede asignar una función de prueba diferente al creador de pruebas (que no sea su función predeterminada).

El creador de pruebas no se puede cambiar ni eliminar de una prueba.

### Propietarios {#owners}

De forma predeterminada, el Creador también es el Propietario de la prueba; sin embargo, el creador puede hacer que otra persona sea el propietario de la prueba al crear la prueba por primera vez (en la [!UICONTROL Nueva prueba] ).

Para cambiar el propietario en la página Nueva prueba :

1. Haga clic en el vínculo para cambiar que aparece junto al nombre del Creador.
1. Seleccione el nuevo propietario en el menú desplegable. (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

Una vez creada la prueba, aún es posible cambiar el propietario. Cualquier persona con derechos de edición en la prueba podrá cambiar la propiedad de la prueba a otro usuario a través del [!UICONTROL Detalles de la prueba] (consulte más abajo).

La capacidad de cambiar el propietario de una prueba es especialmente útil desde el punto de vista de la administración de flujos de trabajo. Permite que la persona responsable del proyecto se haga cargo de la propiedad de las pruebas, lo que les otorga derechos de edición sobre las pruebas y la capacidad de verlas en la variable [!UICONTROL Mis pruebas] vista.

Para cambiar el Propietario de la prueba mediante la variable [!UICONTROL Detalles de la prueba] página:

* Haga clic en el menú Acciones junto al nombre de la persona que desea que sea el propietario
* Select [!UICONTROL Convertir en propietario] en el menú desplegable.
* También puede hacer clic en el [!UICONTROL Propietario] junto a la imagen de prueba y elija el nuevo propietario en la lista desplegable mostrada.

Una vez hecho esto, la palabra &quot;Propietario&quot; aparecerá junto al nombre de esa persona.

>[!NOTE]
>
>Solo se puede convertir en propietario de una prueba a un usuario de la misma cuenta o cuenta de socio. Un usuario en una cuenta de socio solo puede ser propietario de una prueba cuando:
>
>* Existe una relación de socios configurada entre las cuentas. Para obtener más información, consulte [Cuentas de socio en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* No hay campos personalizados en la variable [!UICONTROL Nueva prueba] página.
>* La prueba no se ha asignado a una carpeta.
>* No se han aplicado etiquetas a la prueba.
>




Para delegar temporalmente la propiedad de prueba en [!DNL Workfront Proof], consulte [Designación de propietarios temporales de pruebas en [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
