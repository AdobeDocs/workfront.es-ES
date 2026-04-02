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
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 42%

---

# Exportar datos históricos de [!DNL Adobe Workfront]: pros y contras

<!-- Audited: 5/2025 -->

Este artículo explica las ventajas y desventajas de 4 opciones que puede utilizar para exportar datos históricos de Adobe Workfront.

## Saque partido de uno de nuestros partners

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) tiene una aplicación fácil de usar (su solución [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)) que le permite descargar los datos usted mismo. Un visor opcional (su solución [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)) le permite ver fácilmente sus datos sin conexión.

* **Profesionales:** Todos los objetos principales de [!DNL Workfront] se exportan, incluidos los campos personalizados y las notas, y se almacenan en una base de datos de [!DNL MS Access] de fácil acceso. La interfaz del Visor es fácil de usar y leer. La extracción de documentos también está disponible por separado como servicio, con la salida organizada en una estructura de carpetas lógica que se asigna a cada documento y a sus versiones anteriores.

* **Inconvenientes:** Hay una limitación técnica de 2 GB de datos, pero AtAppStore le permite comprar solo lo que necesita.

* **Costos:** Para obtener más información, ve a [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).



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
