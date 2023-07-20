---
title: 23.3 Mejoras en la integración
description: 23.3 Mejoras en la integración
author: Lisa
feature: Product Announcements
source-git-commit: 29ef11a804cbb7e8da9ddac13bf51de7aa50db53
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 0%

---

# 23.3 Mejoras en la integración

Esta página describe todas las mejoras realizadas en la integración con la versión 23.3 de. Estas mejoras estaban disponibles en el entorno de producción con la versión 23.3 del 20 y 21 de julio de 2023.

Para ver una lista de todos los cambios disponibles en este punto del ciclo de la versión 23.3, consulte [Información general de la versión 23.3](/help/quicksilver/product-announcements/product-releases/23.3-release-activity/23-3-release-overview.md).

## Nueva integración de G Suite ya disponible

Una nueva integración de G Suite ya está disponible en Google Marketplace. La nueva integración se autentica con OAuth2 y reemplaza la integración anterior.

La integración anterior de G Suite ya no se utiliza y se desinstalará automáticamente.

Para obtener instrucciones sobre cómo instalar la nueva integración, consulte [Instalar [!DNL Adobe Workfront for G Suite]](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

Para obtener más información sobre Workfront para G Suite, consulte [Workfront para G Suite](/help/quicksilver/workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md).

## Las integraciones de Adobe Creative Cloud ahora admiten varios usuarios asignados

La integración de Adobe Creative Cloud ahora admite la capacidad de elegir entre &quot;Listo con mi parte&quot; y &quot;Completado&quot; (o &quot;Resuelto&quot;) cuando una tarea o un problema tiene varios usuarios asignados.

Anteriormente, la integración permitía a los usuarios marcar una tarea como realizada, sin especificar &quot;Listo con mi parte&quot; O &quot;Completado&quot;/&quot;Resuelto&quot;.

Para aprovechar esta funcionalidad, descargue e instale los complementos más recientes de Workfront para Creative Cloud.

Para obtener más información sobre la funcionalidad, consulte [Marcar los elementos de trabajo como completados mediante el complemento Adobe Workfront](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-complete.md).

Para obtener información sobre la instalación de los complementos de Workfront para Creative Cloud, consulte [Instalación del complemento de Adobe Workfront para aplicaciones de Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

## Ver y administrar las notificaciones de Workfront desde los complementos de Workfront para Creative Cloud

Para facilitarle la recepción de las notificaciones que necesita, hemos hecho posible ver y administrar las notificaciones de Workfront sin salir de Adobe Creative Cloud. Ahora puede ver las notificaciones y acceder a los elementos de trabajo y comentarios relacionados con ellas directamente desde la ventana del complemento de Workfront dentro de la aplicación de Creative Cloud.

Anteriormente, las notificaciones solo estaban disponibles en Workfront y por correo electrónico.

Para aprovechar esta funcionalidad, descargue e instale los complementos más recientes de Workfront para Creative Cloud.

Para obtener más información, consulte [Ver y administrar [!DNL Adobe Workfront] notificaciones de Adobe Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-notifications.md).

Para obtener información sobre la instalación de los complementos de Workfront para Creative Cloud, consulte [Instalación del complemento de Adobe Workfront para aplicaciones de Creative Cloud](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md).

<!--

## Improved experience when moving a document to a linked folder with drag and drop

We've added some transparency to the process of dragging and dropping a document into a linked folder. Now, the document that you moved to a linked folder remains in the document list until it has fully moved. The document options are disabled, but you can still open the document for view while it is moving. When the document has completed the transfer, it disappears from the document list, because it is now fully located in the linked folder.

Previously, documents would immediately disappear from the document list, before they had finished moving to the linked folder.

For more information, see [Link documents from external applications](/help/quicksilver/documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

-->

## Crear automáticamente carpetas vinculadas a Adobe Experience Manager Assets al crear un proyecto

Con el nuevo flujo de trabajo Crear carpeta vinculada para la integración de Adobe Experience Manager, puede configurar la integración con una ruta a una carpeta de Recursos de Adobe Experience Manager. Cuando se agrega la integración a una plantilla de proyecto, los proyectos creados a partir de la plantilla crearán automáticamente una subcarpeta vinculada en Experience Manager Assets en la carpeta especificada.

Anteriormente, la creación de carpetas vinculadas requería una acción por parte del usuario.

Esta funcionalidad solo está disponible con una integración de Adobe Experience Manager as a Cloud Service en Workfront. Esto no está disponible en el conector mejorado de Adobe Experience Manager.

Para obtener más información, consulte [Uso de flujos de trabajo en la integración de Experience Manager Assets](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/use-aem-workflows.md).

## Asignación de valores de campo de Workfront a etiquetas en Experience Manager Assets

Ahora puede categorizar y encontrar recursos rápidamente en función de los datos de Workfront. Puede asignar estos datos como parte de la configuración de metadatos en la integración de Workfront para Experience Manager Assets.

Anteriormente, la asignación de datos de Workfront a etiquetas de Experience Manager Assets no estaba disponible.

Para obtener más información sobre esta funcionalidad en Experience Manager Assets as a Cloud Service, consulte [Configure las variables [!UICONTROL Experience Manager Assets as a Cloud Service] integración](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Para obtener más información sobre esta funcionalidad en Experience Manager Assets Essentials, consulte [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Asignar campos de Workfront a campos de metadatos de Experience Manager Assets personalizados

Con la integración nativa, ahora puede asignar campos nativos e integrados de Workfront a campos de esquema de metadatos personalizados en Experience Manager Assets as a Cloud Service.

Para obtener más información sobre esta funcionalidad en Experience Manager Assets as a Cloud Service, consulte [Configure las variables [!UICONTROL Experience Manager Assets as a Cloud Service] integración](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).
Para obtener más información sobre esta funcionalidad en Experience Manager Assets Essentials, consulte [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Ajuste la configuración de la plantilla de flujo de trabajo de revisión automatizada con Adobe Workfront for Creative Cloud

Ahora puede ajustar la configuración existente de la plantilla de flujo de trabajo automatizado directamente en el Creative Cloud. Una vez que haya elegido una plantilla de flujo de trabajo automatizada existente, podrá:

* Deshabilitar fases
* Adición de destinatarios adicionales
* Cambiar funciones de revisión
* Ajuste de la fecha límite
* Actualizar notificaciones por correo electrónico
* ¡Y más!

Para obtener más información, consulte [Carga de documentos y pruebas con [!DNL Adobe Workfront] complemento para [!DNL Creative Cloud] Aplicaciones](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-docs-proofs-toc.md).

Estas mejoras están disponibles para las siguientes aplicaciones de Creative Cloud:

* Photoshop
* XD
* InDesign
* Illustrator
