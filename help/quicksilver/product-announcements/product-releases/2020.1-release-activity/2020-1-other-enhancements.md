---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 Otras mejoras
description: Esta página describe todas las mejoras realizadas en las áreas generales de Workfront con la versión 2020.1. Estas mejoras están disponibles actualmente en el entorno de vista previa y estarán disponibles en el entorno de producción a finales de marzo o principios de abril de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# 2020.1 Otras mejoras

Esta página describe todas las mejoras realizadas en las áreas generales de Workfront con la versión 2020.1. Estas mejoras están disponibles actualmente en el entorno de vista previa y estarán disponibles en el entorno de producción a finales de marzo o principios de abril de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.1, consulte [Información general sobre la versión 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Cambio necesario para agregar pruebas a la lista de permitidos

>[!NOTE]
>
>Esta función se ha eliminado de la versión 2020.1. Se pondrá a disposición de los usuarios más adelante.

El dominio de revisión está cambiando de from proofhq.com a workfront.com.

Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a proveedores específicos, debe añadir la siguiente URL adicional a su lista de permitidos para garantizar que los usuarios de su organización puedan ver las pruebas en Workfront tanto en el visor de revisión del explorador como en el visor de revisión de escritorio:

&#42;.workfront.com

La dirección URL &#42;proofhq.com también es obligatoria.

Para obtener más información sobre cómo actualizar la lista de permitidos, consulte [Configuración de la lista de permitidos del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Esta actualización solo se aplica a las pruebas en Workfront; no se aplica al utilizar la aplicación independiente de Workfront Proof.

## Se ha actualizado el comportamiento de las cookies de Workfront para mantener la compatibilidad con Chrome

Para mantener la compatibilidad con una próxima actualización de Google Chrome (Chrome v80), hemos actualizado Workfront Platform para garantizar que las cookies se envíen correctamente con las solicitudes.

Esta actualización de Chrome cambia el valor predeterminado del atributo de cookie SameSite. Si desea probar cómo se comportará la instancia de Workfront después de la actualización de Google Chrome, ajuste los indicadores en Chrome y habilite las siguientes opciones:

* &quot;SameSite con cookies predeterminadas&quot;
* &quot;Las cookies sin SameSite debe ser seguras&quot;

## Sincronización de comentarios de Workfront con Jira

La integración de Workfront para Jira ahora sincroniza sus comentarios de Workfront con el flujo de comentarios nativo de Jira.

Anteriormente, se podían sincronizar comentarios de Jira a Workfront, pero no de Workfront a Jira.

Para obtener más información, consulte [Configuración de Adobe Workfront para Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Se ha eliminado Flash Portfolio Optimizer

Hemos eliminado la capacidad de cambiar entre el nuevo y el Portfolio Optimizer heredado (basado en el Flash) del entorno de Workfront Classic para todos los clientes. Portfolio Optimizer heredado es una función obsoleta y las nuevas herramientas proporcionan las mismas funciones hoy en día.

Para obtener información sobre el optimizador de portafolios, consulte https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Para obtener información sobre cómo dejar de utilizar las herramientas basadas en Flash en Workfront, consulte [Reemplazo de herramientas basadas en Flash en Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
