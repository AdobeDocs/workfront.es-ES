---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exportar datos históricos de Adobe Workfront: pros y contras"
description: Este artículo explica las ventajas y desventajas de 4 opciones que puede utilizar para exportar datos históricos de Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Exportación de datos históricos de [!DNL Adobe Workfron]t: Ventajas y desventajas

Este artículo explica las ventajas y desventajas de las 4 opciones que puede utilizar para exportar datos históricos de [!DNL Workfront].

## Use a uno de nuestros socios

[!DNL AtAppStore], a [!DNL Workfront] partner certificado, tiene una aplicación fácil de usar que le permite descargar sus datos. Esta aplicación también incluye un visor que le permite ver fácilmente sus datos.

* **Ventajas:** Todos sus [!DNL Workfront] Los objetos se exportan, incluidos los campos personalizados. La interfaz del Visor es fácil de usar y leer, y es fácilmente importable en un [!DNL MS Access] Base de datos.

* **Desventajas:** Los documentos no se exportan. Tendrá que descargarlos por separado. Para obtener más información, vaya a [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Solicite un [!DNL Postgres] Archivo de volcado de datos de nuestro equipo de base de datos

El ejecutivo de cuentas puede enviar una solicitud a nuestro equipo de bases de datos para exportar un archivo de volcado de la base de datos (.dmp) [!DNL Postgres] ) con sus datos. Una solicitud adicional irá a nuestro equipo de AOS para recuperar todos sus documentos almacenados.

* **Pros**: obtiene toda la carga de datos, incluidos los campos personalizados, así como los documentos almacenados en el sistema.

* **Contras**: El archivo de base de datos es difícil de leer: no hay forma de leer este archivo a menos que lo cargue en un [!DNL Postgres] base de datos y restablezca las relaciones entre las tablas. Los documentos se almacenan en un servidor de archivos independiente y el equipo de AOS debe extraerlos por separado mediante un proceso independiente. Al hacerlo, no hay ninguna organización que se ocupe de los documentos y todos ellos están referenciados por su GUID.
* **Coste**: Hay un coste asociado con esta descarga, según el tiempo que tarde el equipo en crear el archivo. Consulte con su AEM/ CAE para obtener más información o para comenzar este proceso.

## Exportar mediante [!UICONTROL Kick-Start]

Tanto si dispone de horas de consultoría remota como si no, puede utilizar uno de nuestros consultores para exportar sus datos en forma de informes o [!UICONTROL kick-starts], o puede ejecutar estos informes usted mismo:

* **Pros**: los informes son fáciles de leer y se pueden importar en una variedad de aplicaciones; se pueden personalizar para incluir cualquier agrupación y vista que desee.

* **Contras**: los documentos deberán descargarse por separado.

* **Coste**: Es gratuito si puede ejecutar los informes usted mismo (todo lo que necesita es un inicio de sesión de administrador del sistema) o si puede utilizar las horas de consultoría remota restantes. Si está interesado en adquirir consultoría remota para esto, hable con su AEM/CAE.

  Para obtener más información sobre el uso de KickStarts para exportar datos, consulte [Exportación de datos desde [!DNL Adobe Workfront] mediante [!UICONTROL Kick-Start]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilice nuestra API abierta

si tiene los recursos adecuados en su organización, pueden crear una API personalizada para recuperar todos los datos de Workfront:

* **Pros**: usted tiene el control de lo que exporta del sistema.

* **Contras**: el tiempo se pasa de su lado y tendrá que encontrar recursos para codificar la API y realizar la exportación.

* **Coste**: interno de su organización.
