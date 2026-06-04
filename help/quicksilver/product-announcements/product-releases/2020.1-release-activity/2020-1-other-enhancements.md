---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: Otras mejoras de la versión 2020.1
description: Esta página describe todas las mejoras realizadas en las áreas generales de Workfront con la versión 2020.1. Estas mejoras están disponibles actualmente en el entorno de vista previa y están disponibles en el entorno de producción desde finales de marzo o principios de abril de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
TQID: https://experienceleague.adobe.com/I5djuVv0ixHspF6afQaa5-jTkl0uXl26VlKf8BXqhO4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: b8ea32d4-f1fe-4c71-8871-afe5a702a009
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 100%

---

# Otras mejoras de la versión 2020.1

Esta página describe todas las mejoras realizadas en las áreas generales de Workfront con la versión 2020.1. Estas mejoras están disponibles actualmente en el entorno de vista previa y están disponibles en el entorno de producción desde finales de marzo o principios de abril de 2020.

Para obtener una lista de todos los cambios disponibles con la versión 2020.1, consulte [Información general de la versión 2020.1](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md).

## Cambio necesario para añadir pruebas a la lista de permitidos

>[!NOTE]
>
>Esta función se ha eliminado de la versión 2020.1. Se pondrá a disposición de los usuarios más adelante.

El dominio de revisión cambia de proofhq.com a workfront.com.

Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a proveedores específicos, debe añadir la siguiente URL adicional a su lista de permitidos para garantizar que los usuarios de su organización puedan ver las revisiones en Workfront tanto en el visor de corrección del explorador como en el de escritorio:

&#42;.workfront.com

La URL &#42;proofhq.com también es obligatoria.

Para obtener más información sobre cómo actualizar la lista de permitidos, consulte [Configuración de la lista de permitidos del cortafuegos](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Esta actualización solo se aplica a la revisión en Workfront; no se aplica al utilizar la aplicación independiente de Workfront Proof.

## Se ha actualizado el comportamiento de las cookies de Workfront para mantener la compatibilidad con Chrome

Para mantener la compatibilidad con una próxima actualización de Google Chrome (Chrome versión 80), hemos actualizado la plataforma de Workfront Platform para garantizar que las cookies se envíen correctamente con las solicitudes.

Esta actualización de Chrome cambia el valor predeterminado del atributo de cookie SameSite. Si desea probar cómo se comportará la instancia de Workfront después de la actualización de Google Chrome, ajuste los indicadores en Chrome y habilite las siguientes opciones:

* “SameSite con cookies predeterminadas”
* “Las cookies sin SameSite deben ser seguras”

## Sincronización de comentarios de Workfront con Jira

La integración de Workfront para Jira ahora sincroniza sus comentarios de Workfront con el flujo de comentarios nativo de Jira.

Anteriormente, se podían sincronizar comentarios de Jira a Workfront, pero no de Workfront a Jira.

Para obtener más información, consulte [Configurar Adobe Workfront para Jira](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Se ha quitado el Optimizador de portafolios de Flash

Hemos eliminado la capacidad de cambiar entre el nuevo Optimizador de portafolios y el heredado (basado en Flash) del entorno de Workfront Classic para todos los clientes. El Optimizador de portafolios heredado es una función obsoleta y las nuevas herramientas proporcionan actualmente las mismas funciones.

Para obtener información sobre el Optimizador de portafolios, consulte https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079

Para obtener información sobre la retirada de herramientas basadas en Flash en Workfront, consulte [Reemplazo de herramientas basadas en Flash en Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).
