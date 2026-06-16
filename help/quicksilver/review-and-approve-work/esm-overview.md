---
product-area: documents
navigation-topic: approvals
title: información general sobre el almacenamiento en nube Adobe
description: información general sobre el almacenamiento en nube Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YOO4BspMzbMr8iPoXRBKK65IbU5yfpiJndNuYvYF5SM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 9d28f52ace4d443bdffc475baf79d482152d4157
workflow-type: tm+mt
source-wordcount: 1004
ht-degree: 1%

---

# información general sobre el almacenamiento en nube Adobe

El almacenamiento en la nube de Adobe es una solución de almacenamiento basada en la nube que sirve como repositorio central para los recursos de los productos empresariales de Adobe. La integración de Workfront y Frame.io se basa en el almacenamiento en la nube de Adobe, lo que permite una colaboración y administración de recursos fluidas entre estas plataformas.

Esta opción de almacenamiento también allana el camino para futuras integraciones de la administración de recursos con otros productos de Adobe, como Adobe Creative Cloud.

## Características principales

* **Nivel de almacenamiento unificado**: El almacenamiento en la nube de Adobe actúa como un servidor de almacenamiento compartido para Workfront, Frame.io, Document Cloud y Creative Cloud. Esto permite una colaboración y administración de recursos fluidas en todas estas plataformas.

* **Habilitación de supply chain de contenido**: el almacenamiento en la nube de Adobe es un componente básico para la visión de Supply chain de contenido de Adobe, que permite a los equipos administrar recursos de trabajo en curso sin necesidad de descargas manuales o volver a cargarlos en varias aplicaciones de Adobe.

* **Permisos y acceso centralizados**: el almacenamiento en la nube de Adobe admite controles de acceso de nivel empresarial, integrándose con Adobe IMS (Identity Management System) para obtener permisos de usuario seguros y escalables.

* **Visibilidad completa de los recursos**: Assets almacenado en el almacenamiento en la nube de Adobe se puede mostrar y administrar directamente en las aplicaciones de Workfront, Frame.io y Creative Cloud, lo que proporciona metadatos, versiones y pistas de auditoría coherentes.

* **Integración con flujos de trabajo de revisión y aprobación**: el almacenamiento en la nube de Adobe permite flujos de trabajo creativos de revisión y aprobación al servir como fuente fiable para todos los recursos, lo que garantiza que los comentarios y las aprobaciones se rastreen de forma centralizada.

* **Almacenamiento escalable y administración de cuotas**: el almacenamiento en la nube de Adobe ofrece opciones de almacenamiento escalable y seguimiento unificado de cuotas en todos los productos de Adobe.

## Integración con flujos de trabajo de revisión y aprobación

La integración de Workfront y Frame.io aprovecha el almacenamiento en la nube de Adobe para proporcionar una experiencia unificada de revisión y aprobación. Esta integración permite a los coordinadores de proyectos gestionar proyectos y planificar el trabajo en Workfront, mientras que los creativos, los especialistas en marketing y las partes interesadas pueden revisar y aprobar los recursos en Frame.io. Esto garantiza que todas las partes interesadas tengan acceso a las versiones más recientes de los recursos y que los comentarios estén centralizados en un solo lugar.

Para obtener más información sobre la integración de Workfront y Frame.io, consulte [Resumen unificado de revisión y aprobación](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento de Workfront heredado

Los entornos de Workfront existentes tienen una combinación de almacenamiento en la nube de Adobe y almacenamiento de Workfront heredado. Cualquier objeto creado antes del lanzamiento del almacenamiento en la nube de Adobe utiliza el almacenamiento heredado de Workfront.

Una vez habilitado el almacenamiento en la nube de Adobe en su entorno, puede crear proyectos de almacenamiento en la nube de Adobe y de almacenamiento de Workfront heredado.

>[!NOTE]
>
>Los nuevos entornos netos tienen habilitado de forma predeterminada el almacenamiento en la nube de Adobe y no tienen la opción de utilizar el almacenamiento heredado de Workfront.


### Documentos

#### Área Nuevos documentos

El nuevo área Documentos es un área de documentos unificada rediseñada para el almacenamiento en la nube de Adobe.

Esta interfaz actualizada simplifica la navegación, mejora la claridad y facilita a los equipos la administración de revisiones y aprobaciones en un entorno unificado. Para obtener más información, consulte la [Descripción general del área de documentos](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Nuevo modelo de permisos de documento

>[!IMPORTANT]
>
>En Adobe Cloud Storage, los permisos de documento funcionan de forma diferente que en el almacenamiento heredado de Workfront. Los documentos heredan los permisos del proyecto, la tarea o el problema al que están vinculados.

Los documentos no se pueden compartir individualmente. En su lugar, el sistema genera automáticamente una carpeta para cada tarea o problema y hereda los permisos de la tarea o problema. Cualquier documento cargado en la tarea o el problema se almacena en la carpeta generada.

Para obtener más información sobre el nuevo modelo de permisos de documento, consulte [Permisos de objeto e información general de nivel de acceso para el modelo de almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Objetos vinculados en carpetas

En el nivel de proyecto, las carpetas generadas por el sistema muestran un objeto vinculado. La carpeta recibe automáticamente el mismo nombre que la tarea o el problema al que pertenece. Las carpetas vinculadas son el modo en que el sistema sabe qué tarea o problema debe ver la carpeta.

Para obtener más información, consulte [Funcionamiento de los permisos de documentos](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Objetos de Workfront

La siguiente tabla compara las funciones del almacenamiento en la nube de Adobe y del almacenamiento heredado de Workfront para los objetos de Workfront.

Los objetos de Workfront incluyen portafolios, programas, proyectos, plantillas, tareas y problemas.

| Almacenamiento en la nube de Adobe | Almacenamiento de Workfront heredado |
|---|---|
| <ul><li>Utiliza el almacenamiento en la nube de Adobe</li><li>Integrado con Frame.io</li><li>Utiliza la nueva experiencia Documentos</li><li>Aplica convenciones de nomenclatura estrictas</li><li>El uso compartido directo de documentos no está disponible</li><li>Los documentos están disponibles en otros productos de Adobe como Frame.io y Creative Cloud</li></ul> | <ul><li>Utiliza el almacenamiento de Workfront</li><li>Utiliza el visor de revisión</li><li>Permite compartir documentos individuales</li></ul> |

### Mover, copiar y convertir objetos

En la mayoría de los casos, puede mover, copiar y convertir objetos de Workfront entre modelos de almacenamiento similares. Por ejemplo, puede mover una tarea de un proyecto de almacenamiento en la nube de Adobe a otro proyecto de almacenamiento en la nube Adobe.

En tres casos específicos, puede convertir un objeto de almacenamiento de Workfront heredado al almacenamiento en la nube de Adobe:

* Convierta una tarea de almacenamiento de Workfront heredada en un proyecto de almacenamiento en la nube de Adobe.
* Convierta una cartera de productos de almacenamiento de Workfront heredados en una cartera de productos de almacenamiento en la nube de Adobe.
* Cree un proyecto de almacenamiento en la nube de Adobe a partir de una plantilla de almacenamiento de Workfront heredada.

Los documentos y las carpetas de documentos no se mueven del almacenamiento heredado de Workfront al almacenamiento en la nube de Adobe durante ninguna de estas conversiones.

Para obtener más información, consulte [Portabilidad de objetos](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability) en [Mover a Workfront en el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Habilitar el almacenamiento en la nube de Adobe

Debe contar con una versión de Workfront que admita el almacenamiento en la nube de Adobe. Si su organización aún no tiene una versión compatible, póngase en contacto con el representante de cuentas de Adobe.

Para obtener información sobre cómo habilitar el almacenamiento en la nube de Adobe en su entorno, consulte [Habilitar el almacenamiento en la nube de Adobe para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Los nuevos clientes tienen habilitado de forma predeterminada el almacenamiento en la nube de Adobe y no tienen la opción de utilizar el almacenamiento heredado de Workfront.



## Almacenamiento en la nube de Adobe en entornos de espacio aislado

El almacenamiento en la nube de Adobe está disponible en [!DNL Workfront] entornos de espacio aislado, por lo que puede probarlo antes de habilitarlo en producción. Sin embargo, el visor Frame.io no está disponible en la zona protegida, por lo que la experiencia completa de revisión y aprobación unificadas debe validarse en la producción.

Si tiene una zona protegida de actualización personalizada, debe actualizarla después de actualizar a una versión de Workfront que admita el almacenamiento en la nube de Adobe para acceder a la funcionalidad de almacenamiento en la nube de Adobe en la zona protegida. Para obtener más información, consulte [El [!DNL Adobe Workfront] entorno de espacio aislado de actualización personalizado](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

## Consideraciones

* Es posible que Workfront no esté sincronizado con Frame.io o Creative Cloud, como un recurso que se está eliminando en Workfront pero que sigue apareciendo en Frame.io, póngase en contacto con el servicio de asistencia de Workfront para que se vuelva a sincronizar su entorno.


