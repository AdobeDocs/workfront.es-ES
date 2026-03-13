---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Exportar datos históricos de Adobe Workfront: ventajas y desventajas'
description: En este artículo se explican las ventajas y desventajas de 4 opciones que se pueden utilizar para exportar datos históricos de Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: bbd00374a6b291582cd03b9d0471d8547eb6ab7f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 42%

---

# Exportar datos históricos de [!DNL Adobe Workfront]: pros y contras

<!-- Audited: 5/2025 -->

En este artículo se explican las ventajas y desventajas de 4 opciones que puede utilizar para exportar datos históricos desde Adobe Workfront.

## Saque partido de uno de nuestros partners

[!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) tiene una aplicación fácil de usar (su solución [Workfront Snapshot](https://store.atappstore.com/product/workfront-snapshot/)) que te permite descargar tus datos tú mismo. Un visor opcional (su solución [Workfront Snapshot Viewer](https://store.atappstore.com/product/workfront-snapshot-viewer/)) te permite ver fácilmente tus datos sin conexión.

* **Ventajas:** Todos los [!DNL Workfront] objetos principales se exportan, incluidos los campos y notas personalizados, y se almacenan en una base de datos de [!DNL MS Access] de fácil acceso. La interfaz del Visor es fácil de usar y leer. La extracción de documentos también está disponible por separado como servicio, con el resultado organizado en una estructura de carpetas lógica que se asigna a cada documento y sus versiones anteriores.

* **Desventajas:** Existe una limitación técnica de 2 GB de datos, pero AtAppStore te permite comprar solo lo que necesitas.

* **Costos:** Para obtener más información, visite [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).



## Exportar mediante [!UICONTROL Kick-Starts]

Tanto si dispone de horas de consulta remota como si no, use uno de nuestros consultores para exportar los datos en forma de informes o [!UICONTROL kick-starts], o bien, ejecute los informes usted mismo:

* **Ventajas**: Los informes son fáciles de leer y se pueden importar en diversas aplicaciones. Se pueden personalizar para incluir las agrupaciones y vistas que desee.

* **Desventajas**: los documentos deberán descargarse por separado.

* **Costo**: Es gratis si puedes ejecutar los informes tú mismo (todo lo que necesitas es un inicio de sesión del administrador del sistema), o si puedes usar las horas de consulta remota restantes. En caso de interesarse en adquirir consultoría remota para esto, hable con su analista de datos o CAE.

  Para obtener más información sobre cómo usar Kick-Starts para la exportación de datos, consulte [Exportación de datos de [!DNL Adobe Workfront] mediante [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Utilice la API abierta

en caso de disponer de los recursos adecuados en la organización, es posible crear una API personalizada para recuperar todos los datos de Workfront:

* **Ventajas**: se tiene el control de lo que se exporta del sistema.

* **Desventajas**: el tiempo pasa y tendrá que encontrar recursos para codificar la API y realizar la exportación.

* **Costo**: es interno de la organización.
