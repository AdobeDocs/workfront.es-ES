---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Exportar datos históricos de Adobe Workfront: ventajas e inconvenientes'
description: En este artículo se explican las ventajas y desventajas de 4 opciones que se pueden utilizar para exportar datos históricos de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 7f0aac7c8519b1e570e29fedf1492918e8120ad2
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 39%

---

# Exportar datos históricos de [!DNL Adobe Workfront]: pros y contras

<!-- Audited: 5/2025 -->

Este artículo explica las ventajas y desventajas de 4 opciones que puede utilizar para exportar datos históricos de Adobe Workfront.

## Saque partido de uno de nuestros partners

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) tiene una aplicación fácil de usar (su solución [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)) que le permite descargar los datos usted mismo. Un visor opcional (su solución [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)) le permite ver fácilmente sus datos sin conexión.

* **Profesionales:** Todos los objetos principales de [!DNL Workfront] se exportan, incluidos los campos personalizados y las notas, y se almacenan en una base de datos de [!DNL MS Access] de fácil acceso. La interfaz del Visor es fácil de usar y leer. La extracción de documentos también está disponible por separado como servicio, con la salida organizada en una estructura de carpetas lógica que se asigna a cada documento y a sus versiones anteriores.

* **Inconvenientes:** Hay una limitación técnica de 2 GB de datos, pero AtAppStore le permite comprar solo lo que necesita.

* **Costos:** Para obtener más información, ve a [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).

## Solicitar un archivo de volcado de datos de [!DNL Postgres] del equipo de bases de datos

Debe enviar una solicitud a nuestro equipo de Atención al cliente, que enviará una solicitud a nuestro equipo de Base de datos para exportar un archivo de volcado de base de datos (archivo .dmp [!DNL Postgres]) con sus datos. Una solicitud adicional irá a nuestro equipo de NOC para recuperar todos sus documentos almacenados.

* **Ventajas**: se obtiene toda la carga de datos, incluyendo los campos personalizados, así como los documentos almacenados en el sistema.

* **Desventajas**: No existe una forma de leer este archivo a menos que lo cargue en una base de datos de [!DNL Postgres] y restablezca las relaciones entre las tablas. Los documentos se almacenan en un servidor de archivos independiente y el equipo de NOC debe extraerlos por separado mediante un proceso independiente. Al hacerlo, no habrá ninguna organización que se ocupe de los documentos y todos ellos se referenciarán por su GUID.

* **Costo**: hay un costo asociado con esta descarga según el tiempo que tarde el equipo en crear el archivo. Consulte con su analista de datos o CAE para obtener más información o para comenzar este proceso.

## Exportar mediante [!UICONTROL Kick-Starts]

Tanto si dispone de horas de consulta remota como si no, use uno de nuestros consultores para exportar los datos en forma de informes o [!UICONTROL kick-starts], o bien, ejecute los informes usted mismo:

* **Profesionales**: Los informes son fáciles de leer y se pueden importar en diversas aplicaciones. Se pueden personalizar para incluir cualquier agrupación y vista que desee.

* **Desventajas**: los documentos deberán descargarse por separado.

* **Costo**: es gratuito si puede ejecutar los informes usted mismo (todo lo que necesita es un inicio de sesión de administrador del sistema), o si puede utilizar las horas restantes de consultoría remota. En caso de interesarse en adquirir consultoría remota para esto, hable con su analista de datos o CAE.

  Para obtener más información sobre cómo usar Kick-Starts para la exportación de datos, consulte [Exportación de datos de [!DNL Adobe Workfront] mediante [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilice la API abierta

en caso de disponer de los recursos adecuados en la organización, es posible crear una API personalizada para recuperar todos los datos de Workfront:

* **Ventajas**: se tiene el control de lo que se exporta del sistema.

* **Desventajas**: el tiempo pasa y tendrá que encontrar recursos para codificar la API y realizar la exportación.

* **Costo**: Es interno de su organización.
