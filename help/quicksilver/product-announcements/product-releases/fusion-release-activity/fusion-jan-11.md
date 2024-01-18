---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Actividad de la versión de Workfront Fusion: Semana del 11 de enero de 2021"
description: Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 11 de enero de 2021.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 2439e2a7-9404-433a-bd71-a7776042d8a0
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 0%

---

# Actividad de la versión de Workfront Fusion: Semana del 11 de enero de 2021

Esta página describe todas las mejoras realizadas en Adobe Workfront Fusion durante la semana del 11 de enero de 2021.

Para ver una lista de todos los cambios recientes, consulte [Actividad de la versión de Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obtener una lista de las correcciones de errores recientes en Workfront Fusion, consulte la [Actualizaciones de mantenimiento de Workfront](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) y compruebe si hay alguna actualización denominada Actualización de mantenimiento de Workfront Fusion.

## Ya están disponibles el conector y los módulos ampliados

Ahora puede utilizar Workfront Fusion para conectarse a su cuenta de Widen. Con los módulos Ampliar, puede:

* Agregar o quitar recursos de una colección
* Descargar o cargar archivos
* Leer o actualizar metadatos de recursos
* Buscar recursos en función de los criterios especificados
* Recuperación de una lista de recursos de una colección
* Realizar una llamada de API personalizada.

Para obtener más información, consulte [Ampliar módulos](../../../workfront-fusion/apps-and-their-modules/widen-modules.md).

## Ya están disponibles el conector Datadog y los módulos

Ahora puede utilizar Workfront Fusion para conectarse a su cuenta de Datadog.

Con los módulos Datadog puede:

* Publicar puntos de series temporales
* Realizar una llamada de API personalizada

Para obtener información sobre los módulos Datadog, consulte [Módulos Datadog](../../../workfront-fusion/apps-and-their-modules/datadog-modules.md).

## Ya están disponibles el conector y los módulos Cvent

Ahora puede utilizar Workfront Fusion 2.0 para conectarse a su cuenta de Cvent.

Con los módulos de Cvent puede:

* Crear una convocatoria de reunión
* Leer registros como contactos, eventos o invitados
* Enumerar registros en función de los criterios especificados
* Registrar o agregar invitados a eventos específicos
* Actualizar o eliminar contactos
* Realizar una llamada de API personalizada

Para obtener información sobre los módulos Cvent disponibles, consulte [Módulos Cvent](../../../workfront-fusion/apps-and-their-modules/cvent-modules.md).

## Módulos y conector de Microsoft Dynamics 365 ya disponibles

Ahora puede utilizar Workfront Fusion 2.0 para conectarse a su cuenta de Microsoft Dynamics 365. Con los módulos de Microsoft Dynamics 365, puede:

* Déclencheur de un escenario cuando se agregan o actualizan registros en Microsoft Dynamics 365
* Crear, leer, actualizar o eliminar un registro de Microsoft Dynamics 365
* Realizar una llamada de API personalizada

Para obtener información sobre los módulos disponibles de Microsoft Dynamics 365, consulte [Módulos de Microsoft Dynamics 365](../../../workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

## Ya están disponibles el conector y los módulos de DocuSign

Ahora puede utilizar Workfront Fusion 2.0 para conectarse a su cuenta de Docusign. Con los módulos de Docusign puede:

* Déclencheur de un escenario cuando un sobre cambia su estado
* Creación de un sobre
* Leer, enviar o agregar un destinatario a un sobre existente
* Agregar o modificar campos personalizados en documentos
* Descargar un documento como campo
* Cargar un archivo en un sobre
* Realizar una llamada de API personalizada

Para obtener más información, consulte [Módulos de DocuSign](../../../workfront-fusion/apps-and-their-modules/docusign-modules.md).

## Buscar en el historial de ejecución de escenarios

Le hemos facilitado la localización de información específica de ejecuciones de escenarios anteriores. La nueva búsqueda de texto completo de Fusion permite buscar en el historial de ejecución cualquier dato contenido en un paquete. Por ejemplo, para identificar qué ejecución creó una tarea específica, puede utilizar la búsqueda de texto completo para buscar ese ID de tarea.

Anteriormente, para encontrar información de ejecución específica era necesario ver cada ejecución individualmente.

Para obtener más información, consulte [Visualización del historial de ejecución de un escenario en Adobe Workfront Fusion](../../../workfront-fusion/scenarios/view-scenario-execution-history.md).

## Actualizaciones en el almacén de datos de Fusion 2.0

Para facilitarle la personalización de sus almacenes de datos, hemos añadido algunas funciones nuevas. Ahora, cuando esté viendo un almacén de datos, puede:

* Arrastrar y soltar para reordenar las columnas
* Editar una sola celda
* Añadir varias filas

Para obtener más información sobre los almacenes de datos, consulte [Módulos de almacén de datos](../../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Realizar una solicitud de autorización de clave API a través del conector HTTP

Para aumentar la flexibilidad en las formas de acceder a las API, hemos añadido un nuevo módulo al conector HTTP. Ahora puede utilizar el conector HTTP para realizar una solicitud cuando el servicio web al que accede requiera el uso de una clave de API.

Para obtener más información, consulte [Módulos HTTP](../../../workfront-fusion/apps-and-their-modules/http-modules/http-modules-1.md).

## Nuevas funciones disponibles en el panel de asignación

Para ayudarle a personalizar y simplificar fórmulas en sus módulos, hemos agregado algunas funciones nuevas.

* El

  ```
  omit
  ```

  es una función general que omite las claves dadas del objeto y devuelve el resto.
* El

  ```
  pick
  ```

  es una función general que selecciona solo las claves dadas del objeto.
* El

  ```
  escapeMarkdown
  ```

  es una función de cadena que omite todas las etiquetas Markdown de un texto.

Para obtener más información sobre las funciones de omisión y selección, consulte [Funciones generales en Adobe Workfront Fusion](../../../workfront-fusion/functions/general-functions.md).

Para obtener más información sobre la función escapeMarkdown, consulte [Funciones de cadena en Adobe Workfront Fusion](../../../workfront-fusion/functions/string-functions.md).
