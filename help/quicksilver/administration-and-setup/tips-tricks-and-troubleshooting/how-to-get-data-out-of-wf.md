---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '"Exportar datos históricos de Adobe Workfront: Ventajas y desventajas'
description: Este artículo explica las ventajas y desventajas de 4 opciones que puede utilizar para exportar datos históricos de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Exportar datos históricos de [!DNL Adobe Workfron]t: Ventajas y desventajas

Este artículo explica las ventajas y desventajas de 4 opciones que puede utilizar para exportar datos históricos de [!DNL Workfront].

## Use uno de nuestros socios

[!DNL AtAppStore], [!DNL Workfront] partner certificado, tiene una aplicación fácil de usar que le permite descargar sus datos. Esta aplicación también incluye un visor que le permite ver fácilmente sus datos.

* **Ventajas:** Todas [!DNL Workfront] se exportan, incluidos los campos personalizados. La interfaz del visor es fácil de usar y leer, y es fácilmente importable en un [!DNL MS Access] Base de datos.

* **Inconvenientes:** Los documentos no se exportan. Tendrás que descargarlos por separado. Para obtener más información, vaya a [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Solicitar un [!DNL Postgres] archivo de volcado de datos de nuestro equipo de bases de datos

Su ejecutivo de cuentas puede enviar una solicitud a nuestro equipo de base de datos para exportar un archivo de volcado de base de datos (.dmp [!DNL Postgres] ) con sus datos. Se solicitará más información a nuestro equipo de AOS para recuperar todos los documentos almacenados.

* **Pros**: Obtendrá toda la carga de datos, incluidos los campos personalizados, así como los documentos almacenados en el sistema.

* **Contras**: El archivo de base de datos es difícil de leer: no hay forma de leer este archivo a menos que lo cargue en un [!DNL Postgres] y restablecer las relaciones entre las tablas. Los documentos se almacenan en un servidor de archivos independiente y el equipo de AOS debe extraerlos por separado mediante un proceso independiente. Al hacerlo, no hay organización en los documentos, y todos ellos son referenciados por su GUID.
* **Costo**: Esta descarga conlleva un coste que depende del tiempo que tarde el equipo en crear el archivo. Consulte con su AE/ CAE para obtener más información o para iniciar este proceso.

## Exportación mediante [!UICONTROL Inicio]

Tanto si tiene horas de consultoría remotas como si no, puede utilizar uno de nuestros consultores para exportar sus datos en forma de informes o [!UICONTROL inicio]o puede ejecutar estos informes usted mismo:

* **Pros**: Los informes son fáciles de leer y pueden importarse en diversas aplicaciones; pueden personalizarse para incluir cualquier agrupación y vista que desee.

* **Contras**: Los documentos deberán descargarse por separado.

* **Costo**: Es gratuito si puede ejecutar los informes usted mismo (todo lo que necesita es un inicio de sesión del administrador del sistema) o si puede utilizar las horas de consultoría remotas restantes. Si está interesado en adquirir consultoría remota para esto, por favor hable con su AEM/CAE.

   Para obtener más información sobre el uso de Inicio rápido para exportar datos, consulte [Exportar datos de [!DNL Adobe Workfront] via [!UICONTROL Inicio]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Usar nuestra API abierta

si tiene los recursos adecuados en su organización, pueden crear una API personalizada para recuperar todos sus datos de Workfront:

* **Pros**: Usted está en control de lo que exporta del sistema.

* **Contras**: El tiempo se pasa de su lado y tendrá que encontrar recursos para codificar la API y realizar la exportación.

* **Costo**: Interno a su organización.
