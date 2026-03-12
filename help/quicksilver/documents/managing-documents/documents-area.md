---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: El área Documentos
description: En el área Documentos puede organizar, administrar y ver los metadatos de los documentos cargados en Adobe Workfront. También puede ver la decisión de la revisión.
author: Courtney
feature: Digital Content and Documents
exl-id: 64612345-d1ce-41db-939b-3af30d1c6a51
source-git-commit: abff7d82c89992e2e494aae13c9eb20868259b54
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 43%

---

# El área Documentos

En el área Documentos puede organizar, administrar y ver los metadatos de los documentos cargados en Adobe Workfront. También puede ver la decisión de la revisión.

Actualmente, Workfront tiene dos versiones del área Documentos: el área de documentos heredados y el área de documentos nuevos. La versión que utilice su organización depende de si su organización utiliza almacenamiento de Workfront heredado o almacenamiento empresarial. Para obtener más información acerca de estos tipos de almacenamiento, vea [Información general sobre el almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Área de documentos heredados

Existen dos tipos de áreas de Documentos. Las funciones y la funcionalidad son las mismas para ambas:

* **Área de documentos de un programa, portafolio, proyecto, tarea o problema:** muestra todos los documentos a los que tiene acceso para un proyecto, tarea o problema en particular. Para acceder a esta área, haga clic en **Documentos** ![Icono de documentos](assets/document-icon-12x14.png) en el panel izquierdo mientras ve un proyecto, tarea o problema.

* **Área de documentos globales:** muestra todos los documentos a los que tiene acceso en Workfront. Para obtener acceso a esta área, haga clic en **Documentos** ![Icono de documentos](assets/document-icon.png) en el menú principal ![Icono del menú principal](assets/main-menu-icon.png).

Para obtener información sobre cómo subir documentos en Workfront, consulte [Añadir documentos a Adobe Workfront desde el sistema de archivos](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).


El área de documentos registra un recuento de los siguientes elementos:

* Carpetas de Workfront
* Archivos cargados desde el sistema de archivos
* Archivos añadidos a Workfront desde integraciones
* Experience Manager Assets vinculados

### Panel de resumen

Al seleccionar un documento en el área de documentos, puede utilizar el Resumen de la derecha para ver los detalles del documento, administrar las actualizaciones y aprobaciones del documento, ver las versiones del documento y agregar y editar Forms personalizado para el documento.

Si la revisión está configurada para el documento, la sección Detalles incluye información como la fecha de vencimiento de la revisión y el progreso actual de la revisión.

Puede hacer clic en el encabezado Detalles para ir al área completa Detalles del documento cuando necesite toda la información sobre un documento.

![Área de documentos](assets/documents-area-v2-350x199.png)

Para obtener información sobre el resumen, consulte [Resumen de la información general de documentos](../../documents/managing-documents/summary-for-documents.md).

### Decisión de revisión

Una vez que se toma una decisión de la revisión, esta aparece en la lista de documentos.

![Decisión de revisión en la lista de documentos](assets/proof-decision---doc-list-350x168.png)

### Carpetas

En un proyecto, tarea o problema en el que se hayan cargado documentos, puede configurar carpetas para organizar los documentos. Para obtener más información, consulte [Crear carpetas de documentos](../../documents/organizing-documents/create-documents-folder.md).

En el área de Documentos global, puede configurar dos tipos de carpetas para organizar los documentos a los que tiene acceso:

* **Carpetas inteligentes:** muestra solo los documentos que desea ver. Para obtener más información, consulte [Crear y administrar carpetas inteligentes](../../documents/organizing-documents/create-manage-smart-folders.md).

* **Mis carpetas:** organice los documentos como desee. Para obtener más información, consulte [Crear carpetas de documentos](../../documents/organizing-documents/create-documents-folder.md).

### Detalles del documento ampliados

La página Detalles del documento ofrece una versión más completa de los Detalles del documento en el Resumen de la derecha.

## Nueva área de documento

>[!NOTE]
>
>El área de documentos globales no está disponible en la experiencia de área de nuevos documentos. Solo puede acceder a documentos de programas, portafolios, proyectos, tareas o problemas.

### Uso del panel de resumen

Al seleccionar un documento en el área de documentos, puede utilizar el Panel de resumen de la derecha para ver los detalles del documento, agregar y editar formularios personalizados adjuntos, crear y administrar flujos de trabajo de aprobación, ver versiones del documento y más.

#### Revisar y aprobar con Frame.io

Puede revisar y aprobar documentos en el área de nuevos documentos con el visor Frame.io.

Para obtener más información, consulte [Introducción a la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Administrar versiones

Puede cargar nuevas versiones de un documento en el área de nuevos documentos. Al cargar una nueva versión, se conserva la versión anterior y se puede acceder a ella desde el Panel de resumen. Las versiones se nombran automáticamente con la fecha y la hora de la carga, pero se puede cambiar el nombre según sea necesario.

También puede iniciar un nuevo flujo de trabajo de aprobación para una versión específica de un documento.

#### Ver historial de documentos

Puede ver el historial de un documento en el área de documentos nuevos. El historial incluye los siguientes tipos de información:

* Cuando se cargó el documento
* Cuando se cargaron las nuevas versiones
* Cuando se iniciaron los flujos de trabajo de aprobación para el documento
* Y más

### Carpetas de nivel de sistema para permisos de documento

Workfront crea automáticamente una carpeta de nivel de sistema cuando se carga el primer documento en una tarea o un problema. Estas carpetas heredan los permisos de la tarea o del problema y son visibles en el área de documentos de nivel de proyecto. Todos los documentos cargados en esa tarea o problema se almacenan en esa carpeta y heredan los permisos de ella. Esta es la forma principal en que se administran los permisos para los documentos en el área de nuevos documentos. Para obtener más información, consulte [Permisos de objeto e información general de nivel de acceso para el modelo de almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).