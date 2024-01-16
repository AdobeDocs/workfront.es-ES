---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Administración de funciones de prueba en [!DNL Workfront Proof]
description: Las funciones de prueba permiten conceder permisos a usuarios limitados por el perfil de permiso configurado en su perfil de usuario.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# Administración de funciones de prueba en [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Este artículo hace referencia a la funcionalidad del producto independiente [!DNL Workfront Proof]. Para obtener información sobre la revisión dentro de [!DNL Adobe Workfront], consulte [Revisión](../../../review-and-approve-work/proofing/proofing.md).

Las funciones de prueba permiten conceder permisos a usuarios limitados por el perfil de permiso configurado en su perfil de usuario. (Para obtener más información sobre los perfiles de permisos, consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Las funciones de prueba son diferentes de los perfiles de cuenta. El perfil de su cuenta se relaciona con el nivel de permiso general que tiene en su cuenta y afectará los derechos que tiene sobre todas las pruebas de su cuenta, incluso aquellas que no se hayan compartido explícitamente con usted.

Para obtener más información, consulte [Perfiles de permisos de revisión en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Acerca de los roles de prueba

Las siguientes funciones de prueba se otorgan a los usuarios para una prueba individual en el momento en que se invita al usuario a revisar la prueba:

* [Solo lectura](#read-only)
* [Revisor](#reviewer)
* [Aprobador](#approver)
* [Revisor y aprobador](#reviewer-approver)
* [Autor](#author)
* [Moderador](#moderator)

La función de prueba define qué acciones puede realizar un revisor en relación con esa prueba específica.

Por ejemplo, si es un revisor, se le pedirá que revise la prueba añadiendo marcas y comentarios. Si es un revisor y aprobador, se le pedirá que revise y que tome una decisión sobre la prueba.

Ciertas funciones de prueba otorgan a un revisor derechos de edición sobre la prueba (incluso si su perfil de cuenta no lo hace) y les permiten utilizar algunas funciones adicionales, como añadir acciones en comentarios, crear nuevas versiones y añadir más revisores a la prueba.

Para obtener más información, consulte los siguientes artículos:

* [Uso de acciones en comentarios de prueba](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Uso compartido de una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Solo lectura

{#read-only}

![clean.png](assets/cleaner.png) Puede ver una prueba

![no.png](assets/no.png) No se pueden agregar marcas

![no.png](assets/no.png) No se pueden agregar comentarios

![no.png](assets/no.png) No se puede tomar una decisión

![no.png](assets/no.png) No se pueden eliminar los comentarios de otros usuarios

![no.png](assets/no.png) No tiene derechos de edición en la prueba

>[!NOTE]
>
>Si una carpeta se comparte con un usuario de [!DNL Workfront Proof], se les otorgarán automáticamente derechos de solo lectura a todos los elementos existentes y añadidos posteriormente en la carpeta.

Para obtener más información, consulte [Compartir carpetas en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### Revisor {#reviewer}

![clean.png](assets/cleaner.png) Puede ver una prueba

![clean.png](assets/cleaner.png) Puede agregar marcas

![clean.png](assets/cleaner.png) Puede añadir comentarios

![[!DNL cleaner].png](assets/cleaner.png) Puede editar sus propios comentarios si no hay respuestas

![no.png](assets/no.png) No se puede tomar una decisión

![no.png](assets/no.png) No se pueden editar ni eliminar los comentarios realizados por otros usuarios

![no.png](assets/no.png) No tiene derechos de edición en la prueba

### Aprobador {#approver}

![clean.png](assets/cleaner.png) Puede ver una prueba

![clean.png](assets/cleaner.png) Puede tomar una decisión

![no.png](assets/no.png) No se pueden agregar marcas

![no.png](assets/no.png) No se pueden agregar comentarios

![no.png](assets/no.png) No se pueden editar ni eliminar los comentarios realizados por otros usuarios

![no.png](assets/no.png) No tiene derechos de edición en la prueba

### Revisor y aprobador {#reviewer-approver}

![clean.png](assets/cleaner.png) Puede ver una prueba

![clean.png](assets/cleaner.png) Puede agregar marcas

![clean.png](assets/cleaner.png) Puede añadir comentarios

![[!DNL cleaner].png](assets/cleaner.png) Puede editar sus propios comentarios si no hay respuestas

![clean.png](assets/cleaner.png) Puede tomar una decisión

![no.png](assets/no.png) No se pueden editar ni eliminar los comentarios realizados por otros usuarios

![no.png](assets/no.png) No tiene derechos de edición en la prueba

### Autor {#author}

![clean.png](assets/cleaner.png) Puede agregar marcas

![clean.png](assets/cleaner.png) Puede añadir comentarios

![[!DNL cleaner].png](assets/cleaner.png) Puede editar sus propios comentarios si no hay respuestas

![clean.png](assets/cleaner.png) Puede tomar una decisión

![clean.png](assets/cleaner.png) Puede enviar nuevas versiones

![clean.png](assets/cleaner.png) Puede crear una copia de la prueba

![clean.png](assets/cleaner.png) Puede compartir la prueba con otras personas

![clean.png](assets/cleaner.png) Puede aplicar acciones en los comentarios

![clean.png](assets/cleaner.png) Puede resolver comentarios

![no.png](assets/no.png) No se pueden editar ni eliminar los comentarios realizados por otros usuarios

>[!NOTE]
>
>Esta función solo se puede asignar a usuarios de [!DNL Workfront Proof].

### Moderador {#moderator}

![clean.png](assets/cleaner.png) Puede agregar marcas

![clean.png](assets/cleaner.png) Puede añadir comentarios

![[!DNL cleaner].png](assets/cleaner.png) Puede editar sus propios comentarios si no hay respuestas

![clean.png](assets/cleaner.png) Puede tomar una decisión

![clean.png](assets/cleaner.png) Puede enviar nuevas versiones

![clean.png](assets/cleaner.png) Se pueden agregar nuevos revisores

![clean.png](assets/cleaner.png) Puede aplicar acciones en los comentarios

![clean.png](assets/cleaner.png) Puede resolver comentarios

![clean.png](assets/cleaner.png) Puede eliminar comentarios y respuestas sobre la prueba (realizados por ellos mismos o por otros)

* Si se elimina el primer comentario de un hilo de comentarios, se eliminará todo el hilo
* Al eliminar las respuestas en el hilo de comentarios, solo se eliminará esa respuesta

![no.png](assets/no.png) No se pueden editar los comentarios de otros usuarios

Esta función permite a la persona administrar y moderar los comentarios de la prueba, lo que le da la oportunidad de mantener solo comentarios relevantes sobre la prueba y eliminar comentarios no relevantes.

>[!NOTE]
>
>Esta función solo se puede asignar a usuarios de [!DNL Workfront Proof].

## Asignación de funciones de prueba

Puede asignar funciones de prueba al crear nuevas pruebas, al crear versiones nuevas de pruebas existentes o en pruebas existentes.

### Nuevas pruebas {#new-proofs}

Se pueden asignar funciones de prueba a los revisores en la [!UICONTROL Nueva revisión] página durante el proceso de creación de la prueba (1).

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Nuevas versiones {#new-versions}

Al crear una nueva versión de una prueba, se muestran automáticamente los revisores de la versión anterior (con la misma función que la versión anterior).

Puede editar las funciones de prueba aplicadas a los revisores al crear la nueva versión (1).

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Pruebas existentes {#existing-proofs}

Si desea cambiar la función de una persona en una prueba existente, puede hacerlo en la [!UICONTROL Detalles de revisión] editar en línea su función en la sección de flujo de trabajo (1).

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## Comprobación de funciones en el visualizador de pruebas

Puede comprobar la función de un revisor directamente desde el Visualizador de pruebas (1) y editarlo (2) si es necesario.

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Funciones de prueba predeterminadas

Puede establecer su función de prueba predeterminada en la variable [!DNL Proofing Defaults] en su Configuración personal. Esto significa que, cuando se le añada a una prueba, la función de prueba predeterminada se rellenará automáticamente. Tenga en cuenta que un usuario con derechos de edición sobre una prueba puede cambiar esta función en el nivel de prueba.

>[!NOTE]
>
>Solo los usuarios con perfiles de Administrador o Administrador de facturación pueden cambiar los valores predeterminados de revisión para otros usuarios de su cuenta.

Para obtener más información, consulte [Configuración personal en [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Creadores y propietarios

Los creadores y propietarios tienen derechos de edición completos sobre la prueba.

### Creadores {#creators}

El creador de la prueba es la persona que carga la prueba en primer lugar. El creador de la prueba se muestra automáticamente en la lista de personas de la prueba (en su función predeterminada).

En el [!UICONTROL Nueva revisión] página puede asignar una función de prueba diferente al creador de la prueba (que no sea su función predeterminada).

El creador de la prueba no se puede cambiar ni eliminar de una prueba.

### Propietarios {#owners}

De forma predeterminada, el Creador también es el Propietario de la prueba; sin embargo, puede convertir a otra persona en el Propietario de la prueba al crear inicialmente la prueba (en la [!UICONTROL Nueva revisión] página).

Para cambiar el propietario en la página Nueva prueba:

1. Haga clic en el vínculo de cambio que aparece junto al nombre del creador.
1. Seleccione el nuevo propietario en el menú desplegable. (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

Una vez creada la prueba, aún es posible cambiar el propietario. Cualquier persona con derechos de edición en la prueba podrá cambiar la propiedad de la prueba a otro usuario a través de [!UICONTROL Detalles de revisión] (ver más abajo).

La capacidad de cambiar el propietario de una prueba es especialmente útil desde el punto de vista de la administración del flujo de trabajo. Permite a la persona responsable del proyecto asumir la propiedad de las pruebas, lo que les otorga derechos de edición sobre las pruebas y la capacidad de verlas en la [!UICONTROL Mis pruebas] vista.

Para cambiar el propietario de la prueba mediante el [!UICONTROL Detalles de revisión] página:

* Haga clic en el menú Acciones junto al nombre de la persona que desea convertir en propietario.
* Seleccionar [!UICONTROL **Convertir en propietario**] en el menú desplegable.
* También puede hacer clic en la variable [!UICONTROL **Propietario**] junto a la imagen de prueba y elija el nuevo propietario en la lista desplegable que se muestra.

Una vez hecho esto, se mostrará la palabra &quot;Propietario&quot; junto al nombre de esa persona.

>[!NOTE]
>
>Solo un usuario de la misma cuenta o una cuenta de socio puede convertirse en propietario de una prueba. Un usuario de una cuenta de socio puede convertirse en propietario de una prueba solo cuando:
>
>* Existe una relación de socio configurada entre las cuentas. Para obtener más información, consulte [Cuentas de socio en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* No hay campos personalizados en [!UICONTROL Nueva revisión] página.
>* La revisión no se ha asignado a una carpeta.
>* No se han aplicado etiquetas a la prueba.

Para delegar temporalmente la propiedad de la prueba en [!DNL Workfront Proof], consulte [Designación de propietarios de prueba temporales en [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
