---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exportar datos históricos de Adobe Workfront: ventajas e inconvenientes"
description: Este artículo explica las ventajas y desventajas de 4 opciones que puede utilizar para exportar datos históricos de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Exportar datos históricos de [!DNL Adobe Workfront]: pros y contras

Este artículo explica las ventajas y desventajas de cuatro opciones que puede utilizar para exportar datos históricos de [!DNL Workfront].

## Use a uno de nuestros socios

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) tiene una aplicación fácil de usar (su solución [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)) que le permite descargar los datos usted mismo. Un visor opcional (su solución [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)) le permite ver fácilmente sus datos sin conexión.

* **Profesionales:** Se exportan todos los objetos principales de [!DNL Workfront], incluidos los campos personalizados y las notas, todos los cuales se almacenan en una base de datos de [!DNL MS Access] de fácil acceso. La interfaz del Visor es fácil de usar y leer. La extracción de documentos también está disponible por separado como servicio, con la salida organizada en una estructura de carpetas lógica que se asigna a cada documento (y, opcionalmente, a sus versiones anteriores).

* **Inconvenientes:** Hay una limitación técnica de 2 GB de datos, pero AtAppStore le permite comprar solo lo que necesita.

* **Costos:** Para obtener más información, ve a [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).

## Solicitar un archivo de volcado de datos [!DNL Postgres] de nuestro equipo de base de datos

Debe enviar una solicitud a nuestro equipo de Atención al cliente, que enviará una solicitud a nuestro equipo de Base de datos para exportar un archivo de volcado de base de datos (archivo .dmp [!DNL Postgres]) con sus datos. Una solicitud adicional irá a nuestro equipo de NOC para recuperar todos sus documentos almacenados.

* **Profesionales**: obtendrá toda la carga de datos, incluidos los campos personalizados, así como los documentos almacenados en el sistema.

* **Inconvenientes**: el archivo de base de datos es difícil de leer: no hay forma de que pueda leer este archivo a menos que lo cargue en una base de datos de [!DNL Postgres] y restablezca las relaciones entre las tablas. Los documentos se almacenan en un servidor de archivos independiente y el equipo de NOC debe extraerlos por separado mediante un proceso independiente. Al hacerlo, no hay ninguna organización que se ocupe de los documentos y todos ellos están referenciados por su GUID.

* **Costo**: hay un costo asociado con esta descarga, dependiendo del tiempo que tarde el equipo en crear el archivo. Consulte con su AEM/ CAE para obtener más información o para comenzar este proceso.

## Exportar mediante [!UICONTROL Kick-Starts]

Tanto si tiene horas de consulta remota como si no, puede utilizar uno de nuestros consultores para exportar los datos en forma de informes o [!UICONTROL kick-starts], o puede ejecutar estos informes usted mismo:

* **Profesionales**: Los informes son fáciles de leer y se pueden importar en una variedad de aplicaciones; se pueden personalizar para incluir cualquier agrupación y vista que desee.

* **Inconvenientes**: los documentos deberán descargarse por separado.

* **Costo**: es gratis si puede ejecutar los informes usted mismo (todo lo que necesita es un inicio de sesión de administrador del sistema), o si puede usar las horas restantes de consultoría remota. Si está interesado en adquirir consultoría remota para esto, hable con su AEM/CAE.

  Para obtener más información sobre cómo usar Kick-Starts para exportar datos, consulte [Exportar datos de [!DNL Adobe Workfront] mediante [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilice nuestra API abierta

si tiene los recursos adecuados en su organización, pueden crear una API personalizada para recuperar todos los datos de Workfront:

* **Profesionales**: Usted tiene el control de lo que exporta del sistema.

* **Inconvenientes**: El tiempo se pasa de su lado y tendrá que encontrar recursos para codificar la API y realizar la exportación.

* **Costo**: interno de su organización.
