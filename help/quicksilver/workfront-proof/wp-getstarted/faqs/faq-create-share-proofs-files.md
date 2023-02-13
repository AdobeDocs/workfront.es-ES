---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: 'Preguntas más frecuentes: Creación y uso compartido de pruebas y archivos'
description: Una prueba es un archivo estático, de audio o de vídeo que está disponible para su revisión en el visor de pruebas. Los revisores añadidos a una prueba tienen a su disposición un conjunto de herramientas para realizar comentarios y decisiones sobre la prueba.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: d5ffd576fcedf9b10dce5e5d5bd9245dd7f67ef8
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 0%

---

# Preguntas más frecuentes: Creación y uso compartido de pruebas y archivos

>[!IMPORTANT]
>
>Este artículo se refiere a la funcionalidad en el producto independiente [!DNL Workfront Proof]. Para obtener información sobre pruebas en el interior [!DNL Adobe Workfront], consulte [Prueba](../../../review-and-approve-work/proofing/proofing.md).

## ¿Qué es una prueba?

### Respuesta

Una prueba es un archivo estático, de audio o de vídeo que está disponible para su revisión en el visor de pruebas. Los revisores añadidos a una prueba tienen a su disposición un conjunto de herramientas para realizar comentarios y decisiones sobre la prueba.

## ¿Qué tipos de archivo se admiten?

### Respuesta

Las pruebas se pueden crear a partir de archivos estáticos, de audio y de vídeo. No puede cargar archivos de más de 4 GB. [!DNL Workfront] admite más de 150 tipos de archivo (consulte [Información general sobre los tipos de archivos de prueba compatibles y los límites de tamaño](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) para obtener una lista completa).

## ¿Cuál es la diferencia entre una prueba y un archivo?

### Respuesta

Al cargar un archivo en [!DNL Workfront Proof], el sistema almacena el archivo en su [!DNL Workfront Proof] cuenta. Cuando lo comparta, [!DNL Workfront Proof] envía un correo electrónico a los destinatarios con un vínculo en el que pueden hacer clic para descargar el archivo. Puede compartir cualquier tipo de archivo que desee.

Cuando crea una prueba a partir de un archivo que ha cargado en [!DNL Workfront Proof], puede hacer que el archivo esté disponible para su revisión en el visor de pruebas. Los revisores reciben un correo electrónico con un vínculo a la prueba. Cuando abren la prueba, ven la imagen de prueba y pueden agregar comentarios y tomar decisiones al respecto. Puede crear pruebas utilizando archivos de la lista de tipos de archivo admitidos. También puede crear pruebas utilizando direcciones URL para sitios web y otro contenido web.

Para obtener una lista completa de los tipos de archivo admitidos, consulte [Información general sobre los tipos de archivos de prueba compatibles y los límites de tamaño](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## ¿Cómo creo una prueba?

### Respuesta

Puede crear pruebas a partir de archivos estáticos, archivos de audio, archivos de vídeo y direcciones URL (consulte ).

Para crear una prueba en la cuenta, debe ser un usuario con el perfil de permiso correcto (consulte [[!UICONTROL Perfiles de permisos de prueba] en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Si carga varios archivos al mismo tiempo, crea varias pruebas que puede enviar al mismo grupo de revisores mediante un solo correo electrónico. Si su organización tiene un [!UICONTROL Empresa] o [!UICONTROL Sin límite] cuenta, puede combinar archivos en una sola prueba (consulte [Creación de una prueba de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)).

## ¿Qué son las funciones de prueba y las alertas de correo electrónico?

### Respuesta

Las funciones de prueba definen qué acciones debe realizar un revisor en una prueba. Existen diferentes opciones de función que puede utilizar para los revisores al crear una prueba, en función de si desea que puedan realizar comentarios, tomar decisiones, etc. Para obtener más información, consulte [Administrar funciones de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

Las alertas por correo electrónico actualizan a los revisores en el progreso de una prueba (son diferentes de las nuevas notificaciones de prueba y de prueba tardía). Puede seleccionar diferentes opciones para diferentes revisores, según la función de cada revisor en la prueba. Para obtener más información, consulte [Cree una prueba avanzada con un [!UICONTROL Flujo de trabajo automatizado]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## ¿Puedo crear una prueba a partir de varios archivos?

### Respuesta

La combinación de varios archivos en una sola prueba es una función disponible en [!UICONTROL Empresa] y [!UICONTROL Sin límite] planes de edición. Esta opción solo es posible para archivos estáticos, no para archivos de vídeo. Para obtener más información, consulte  [Creación de una prueba de varias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## ¿Puedo crear pruebas a partir de direcciones URL?

### Respuesta

Sí, puede crear pruebas a partir de sitios web y otro contenido web. Al añadir una URL para crear una prueba, puede especificar si desea una prueba estática o una prueba interactiva:

* En una prueba interactiva, los revisores pueden navegar e interactuar como lo harían normalmente con el sitio web u otro contenido web, como los anuncios con vídeo o audio de flujo continuo. [!DNL Flash] elementos de un anuncio, animaciones de HTML y banners interactivos. Para obtener más información, consulte [Crear una prueba de contenido interactivo en un archivo ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).
* Para una prueba estática, [!DNL Workfront] toma un conjunto de capturas de pantalla de las páginas y subpáginas que especifique. Los hipervínculos están activos en la prueba, por lo que puede probar si conducen o no al destino correcto. Para obtener más información, consulte [Creación de una prueba estática para un sitio web u otro contenido web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

Puede agregar varias direcciones URL a la vez si las separa con un espacio. Tenga en cuenta que la combinación solo está disponible en [!UICONTROL Empresa] y [!UICONTROL Sin límite] planes de edición.

## ¿Pueden las personas que no tienen un inicio de sesión crear pruebas en mi cuenta?

### Respuesta

Necesita credenciales de inicio de sesión para crear pruebas directamente en una [!DNL Workfront Proof] cuenta.

## ¿Qué significa compartir una prueba?

### Respuesta

Al compartir una prueba, los revisores pueden acceder a ella para que puedan añadir comentarios y marcas y tomar decisiones al respecto. Los revisores invitados acceden a las pruebas desde la notificación por correo electrónico que reciben. Los revisores con sus propios [!DNL Workfront Proof] la cuenta puede acceder a las pruebas en la [!UICONTROL Panel].

## ¿Cómo comparto una prueba?

### Respuesta

Cuando esté creando una prueba, puede agregar revisores en la variable [!UICONTROL Flujo de trabajo] de la sección [!UICONTROL Nueva prueba] página. Cuando la prueba esté lista, [!DNL Workfront Proof] envía un correo electrónico a los revisores que contienen un vínculo a la prueba.

Si tiene derechos suficientes sobre una prueba, puede utilizar el visualizador de pruebas, su [!UICONTROL Panel], o cualquiera de las vistas de lista para agregar revisores a una prueba existente (consulte [Compartir una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] Página en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

Añadir revisores es la forma más común de compartir pruebas. Si desea explorar otras opciones disponibles, consulte:

* [Compartir vínculos de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [Compartir la URL pública en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [Suscripción a una prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [Cree una prueba Mini en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## ¿Tiene que ser usuario para revisar una prueba?

### Respuesta

No. Revisores invitados (personas sin [!DNL Workfront Proof] credenciales de inicio de sesión) puede acceder a una prueba desde la notificación de correo electrónico de prueba que reciben. Puede compartir una prueba con tantos invitados como desee.

Es posible restringir el uso compartido de pruebas a personas con [!DNL Workfront Proof] credenciales de inicio de sesión. Esto añade otra capa de seguridad a sus pruebas. Para mejorar la seguridad, los administradores de sistemas de las organizaciones con [!UICONTROL Empresa] y [!UICONTROL Sin límite] planes pueden configurar este requisito para todas las pruebas creadas en la organización.

Para obtener más información sobre cómo exigir el inicio de sesión, consulte [seguridad de la prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

Si su organización requiere que los revisores firmen pruebas electrónicamente, lo que requiere que inicie sesión [!DNL Workfront Proof], los usuarios solo pueden compartir pruebas con usuarios registrados. Esta opción está disponible en [!UICONTROL Empresa] y [!UICONTROL Sin límite] planes de edición. Para obtener más información, consulte [Explicación de las firmas electrónicas en [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## ¿Puedo establecer una fecha límite para mis revisores?

### Respuesta

Puede establecer una fecha límite para una nueva prueba o una nueva versión de prueba al crear la prueba. Haga esto en la [!UICONTROL Flujo de trabajo] de la sección [!UICONTROL Nueva prueba] página. Si usa [!UICONTROL Flujo de trabajo automatizado], puede establecer una fecha límite diferente para cada etapa de la revisión.

También puede establecer o actualizar una fecha límite para una prueba existente mediante la variable [!UICONTROL Detalles de la prueba] página. Para obtener más información, consulte [Administrar detalles de prueba en [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## ¿Cómo puedo crear una nueva versión de mi prueba?

### Respuesta

Los revisores suelen solicitar cambios en sus comentarios en una prueba y desean ver una nueva versión de la prueba. Puede crear nuevas versiones de una prueba. [!DNL Workfront Proof] recuerda la configuración de la prueba de la versión anterior. Puede seguir editando esta configuración si necesita hacer algo como agregar o quitar revisores para la prueba.

Debe compartir cada versión con los revisores específicos que necesiten verla. Por ejemplo, si comparte solo la versión 3 con un revisor, esa persona no podrá ver las versiones 1 y 2. Los supervisores y administradores de la cuenta supervisan todos los proyectos de la cuenta para que puedan ver y editar todas las versiones de la prueba.

Para obtener más información, consulte .

## ¿Puedo compartir archivos con [!DNL Workfront Proof]?

### Respuesta

Sí. Si desea compartir algo con otras personas, pero no necesita que lo vean como una prueba (o si es un tipo de archivo que no sea compatible con [!DNL Workfront Proof]), puede cargarlo como un archivo en su [!DNL Workfront Proof] cuenta. Al igual que con las pruebas, puede organizar los archivos en carpetas, etiquetar archivos y agregar un mensaje personalizado al correo electrónico de notificación cuando comparta el archivo. Para obtener más información, consulte [Cargar archivos y contenido web a [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

Cuando los destinatarios reciben la notificación por correo electrónico sobre un archivo que está compartiendo, pueden descargar el archivo haciendo clic en el vínculo de la notificación.

[!DNL Workfront Proof] los usuarios pueden convertir archivos en pruebas después de guardarlos en su cuenta.

<!--Is there a limit-->
