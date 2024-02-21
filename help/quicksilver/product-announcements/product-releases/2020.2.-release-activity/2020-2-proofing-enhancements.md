---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: Mejoras de revisión 2020.2
description: Esta página describe todas las mejoras de revisión realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 021c6e0c-3593-40f7-8eeb-7e016001893e
source-git-commit: 99aac8d1621370f901704f58affd9e3e18497c4e
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# Mejoras de revisión 2020.2

Esta página describe todas las mejoras de revisión realizadas con la versión 2020.2 en el entorno de producción. Estas mejoras estaban disponibles en el entorno de producción en la semana del 11 de mayo de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.2, consulte [información general sobre la versión 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

## El dominio de revisión cambia de proofhq.com a workfront.com.

>[!NOTE]
>
>Esta función se comunicó originalmente como parte de la versión 2020.1, pero se eliminó de la versión antes de su lanzamiento en Producción.

Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a proveedores específicos, debe añadir la siguiente URL adicional a su lista de permitidos para garantizar que los usuarios de su organización puedan ver las pruebas en Workfront tanto en el visor de revisión del explorador como en el visor de revisión de escritorio:

&#42;.workfront.com

El &#42;La URL de proofhq.com también es obligatoria.

Para obtener más información sobre cómo actualizar la lista de permitidos, consulte [Configuración de la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Esta actualización solo se aplica a las pruebas en Workfront; no se aplica al utilizar la aplicación independiente Workfront Proof.

## Los comentarios de revisión realizados por los invitados aparecen en el área de Actualizaciones

Para optimizar la colaboración en las pruebas, los comentarios de los invitados aparecen en el área de Actualizaciones.

Anteriormente, los comentarios de prueba realizados por los invitados solo estaban disponibles en la prueba.
