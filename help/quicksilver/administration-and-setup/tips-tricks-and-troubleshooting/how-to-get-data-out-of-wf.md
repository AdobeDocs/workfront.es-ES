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
source-wordcount: '504'
ht-degree: 0%

---

# Exportar datos históricos de [!DNL Adobe Workfron]t: pros y contras

Este artículo explica los pros y los contras de 4 opciones que puede usar para exportar datos históricos de [!DNL Workfront].

## Use a uno de nuestros socios

[!DNL AtAppStore], un socio certificado de [!DNL Workfront], tiene una aplicación fácil de usar que te permite descargar tus datos. Esta aplicación también incluye un visor que le permite ver fácilmente sus datos.

* **Profesionales:** Se han exportado todos los objetos de [!DNL Workfront], incluidos los campos personalizados. La interfaz del visor es fácil de usar y leer, y se puede importar fácilmente en una base de datos de [!DNL MS Access].

* **Inconvenientes:** Los documentos no se exportan. Tendrá que descargarlos por separado. Para obtener más información, vaya a [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Solicitar un archivo de volcado de datos [!DNL Postgres] de nuestro equipo de base de datos

El ejecutivo de cuentas puede enviar una solicitud a nuestro equipo de bases de datos para exportar un archivo de volcado de base de datos (archivo .dmp [!DNL Postgres]) con sus datos. Una solicitud adicional irá a nuestro equipo de AOS para recuperar todos sus documentos almacenados.

* **Profesionales**: obtendrá toda la carga de datos, incluidos los campos personalizados, así como los documentos almacenados en el sistema.

* **Inconvenientes**: el archivo de base de datos es difícil de leer: no hay forma de que pueda leer este archivo a menos que lo cargue en una base de datos de [!DNL Postgres] y restablezca las relaciones entre las tablas. Los documentos se almacenan en un servidor de archivos independiente y el equipo de AOS debe extraerlos por separado mediante un proceso independiente. Al hacerlo, no hay ninguna organización que se ocupe de los documentos y todos ellos están referenciados por su GUID.
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
