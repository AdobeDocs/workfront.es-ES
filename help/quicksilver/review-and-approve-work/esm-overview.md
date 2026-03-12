---
product-area: documents
navigation-topic: approvals
title: Información general sobre el almacenamiento empresarial de Adobe
description: Información general sobre el almacenamiento empresarial de Adobe
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: 97c351ca38a8b6075634b2f755f2330562bc8b52
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 2%

---

# Información general sobre el almacenamiento empresarial de Adobe

El almacenamiento empresarial de Adobe es una solución de almacenamiento basada en la nube que sirve como repositorio central para los recursos de los productos empresariales de Adobe. La integración de Workfront y Frame.io se basa en el almacenamiento empresarial de Adobe, lo que permite una colaboración y administración de recursos sin problemas entre estas plataformas.

Esta opción de almacenamiento también allana el camino para futuras integraciones de la administración de recursos con otros productos de Adobe, como Adobe Creative Cloud.

## Características principales

* **Nivel de almacenamiento unificado**: El almacenamiento empresarial de Adobe actúa como servidor de almacenamiento compartido para Workfront, Frame.io, Document Cloud y Creative Cloud. Esto permite una colaboración y administración de recursos fluidas en todas estas plataformas.

* **Habilitación de supply chain de contenido**: el almacenamiento empresarial de Adobe es un componente básico para la visión de Supply chain de contenido de Adobe, que permite a los equipos administrar recursos de trabajo en curso sin necesidad de descargas manuales o volver a cargar en varias aplicaciones de Adobe.

* **Permisos y acceso centralizados**: el almacenamiento empresarial de Adobe admite controles de acceso de nivel empresarial, integrándose con Adobe IMS (Identity Management System) para obtener permisos de usuario seguros y escalables.

* **Visibilidad completa de los recursos**: los Assets almacenados en el almacenamiento empresarial de Adobe se pueden ver y administrar directamente en las aplicaciones de Workfront, Frame.io y Creative Cloud, lo que proporciona metadatos, versiones y pistas de auditoría coherentes.

* **Integración con flujos de trabajo de revisión y aprobación**: el almacenamiento empresarial de Adobe habilita los flujos de trabajo de revisión y aprobación creativos al servir como fuente fiable para todos los recursos, lo que garantiza que los comentarios y las aprobaciones se rastreen de forma centralizada.

* **Almacenamiento escalable y administración de cuotas**: el almacenamiento empresarial de Adobe ofrece opciones de almacenamiento escalable y seguimiento unificado de cuotas en todos los productos de Adobe.

## Integración con flujos de trabajo de revisión y aprobación

La integración de Workfront y Frame.io aprovecha el almacenamiento empresarial de Adobe para proporcionar una experiencia unificada de revisión y aprobación. Esta integración permite a los coordinadores de proyectos gestionar proyectos y planificar el trabajo en Workfront, mientras que los creativos, los especialistas en marketing y las partes interesadas pueden revisar y aprobar los recursos en Frame.io. Esto garantiza que todas las partes interesadas tengan acceso a las versiones más recientes de los recursos y que los comentarios estén centralizados en un solo lugar.

Para obtener más información sobre la integración de Workfront y Frame.io, consulte [Descripción general de la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).

## Diferencias entre el almacenamiento empresarial de Adobe y el almacenamiento heredado de Workfront

Los entornos de Workfront existentes tienen una combinación de almacenamiento empresarial de Adobe y almacenamiento de Workfront heredado. Cualquier objeto creado antes del lanzamiento del almacenamiento empresarial de Adobe utiliza el almacenamiento heredado de Workfront.

Una vez que haya habilitado el almacenamiento empresarial de Adobe en su entorno, puede crear proyectos de almacenamiento empresarial de Adobe y de almacenamiento de Workfront heredado.

>[!NOTE]
>
>Los nuevos entornos netos tienen habilitado de forma predeterminada el almacenamiento empresarial de Adobe y no tienen la opción de utilizar el almacenamiento heredado de Workfront.


### Documentos

#### Área de nuevos documentos

El área de nuevos documentos es un área de documentos unificada rediseñada para el almacenamiento empresarial de Adobe.

Esta interfaz actualizada simplifica la navegación, mejora la claridad y facilita a los equipos la administración de revisiones y aprobaciones en un entorno unificado. Para obtener más información, consulte la [Descripción general del área de documentos](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Nuevo modelo de permisos de documento

>[!IMPORTANT]
>
>En el almacenamiento empresarial de Adobe, los permisos de documento funcionan de forma diferente que en el almacenamiento heredado de Workfront. Los documentos heredan los permisos del proyecto, la tarea o el problema al que están vinculados.

Los documentos no se pueden compartir individualmente. En su lugar, el sistema genera automáticamente una carpeta para cada tarea o problema y hereda los permisos de la tarea o problema. Cualquier documento cargado en la tarea o el problema se almacena en la carpeta generada.

Para obtener más información acerca del nuevo modelo de permisos de documento, vea [Permisos de objeto e información general de nivel de acceso para el modelo de almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Objetos vinculados en carpetas

En el nivel de proyecto, las carpetas generadas por el sistema muestran un objeto vinculado. La carpeta recibe automáticamente el mismo nombre que la tarea o el problema al que pertenece. Las carpetas vinculadas son el modo en que el sistema sabe qué tarea o problema debe ver la carpeta.

Para obtener más información, consulte [Funcionamiento de los permisos de documentos](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Objetos de Workfront

La siguiente tabla compara las funciones del almacenamiento empresarial de Adobe y del almacenamiento heredado de Workfront para los objetos de Workfront.

Los objetos de Workfront incluyen portafolios, programas, proyectos, plantillas, tareas y problemas.

| almacenamiento empresarial de Adobe | Almacenamiento de Workfront heredado |
|---|---|
| <ul><li>Utiliza el almacenamiento empresarial de Adobe</li><li>Integrado con Frame.io</li><li>Utiliza la nueva experiencia Documentos</li><li>Aplica convenciones de nomenclatura estrictas</li><li>El uso compartido directo de documentos no está disponible</li><li>Los documentos están disponibles en otros productos de Adobe como Frame.io y Creative Cloud</li></ul> | <ul><li>Utiliza el almacenamiento de Workfront</li><li>Utiliza el visor de revisión</li><li>Permite compartir documentos individuales</li></ul> |

### Mover, copiar y convertir objetos

Puede mover, copiar y convertir objetos de Workfront entre modelos de almacenamiento similares. Por ejemplo, puede mover una tarea de un proyecto de almacenamiento empresarial de Adobe a otro proyecto de almacenamiento empresarial de Adobe. No puede mover una tarea de un proyecto de almacenamiento empresarial de Adobe a un proyecto de almacenamiento de Workfront heredado.

Estas acciones están disponibles en el menú Más sobre una tarea o un problema. Cada acción respeta la integridad del documento, la herencia de permisos y las reglas de almacenamiento empresarial de Adobe.

## Habilitar el almacenamiento empresarial de Adobe

Los clientes existentes pueden habilitar el almacenamiento empresarial de Adobe en su entorno tras la renovación del contrato. Para obtener más información sobre cómo habilitar el almacenamiento empresarial de Adobe, consulte [Habilitar el almacenamiento empresarial de Adobe para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Los nuevos clientes tienen habilitado de forma predeterminada el almacenamiento empresarial de Adobe y no tienen la opción de utilizar el almacenamiento heredado de Workfront.






