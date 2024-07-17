---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Resolución de problemas de integración de Adobe Experience Manager
description: "Problema: Los Assets no se guardan en Adobe Experience Manager"
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Resolución de problemas de integración de Adobe Experience Manager

## Problema: Las Assets no se guardan en Adobe Experience Manager

Cuando un usuario selecciona un recurso o una carpeta para exportarlos a Experience Manager Assets y hace clic en Seleccionar, la ventana del selector se cierra pero los recursos no se guardan en Experience Manager Assets. Workfront no indica que los recursos no se hayan guardado en Experience Manager Assets.

### Causa

Esto puede ocurrir debido a la lista de permitidos de Adobe Cloud Manager. Si la lista de permitidos Cloud Manager de Adobe de una organización está vacía, las direcciones IP no están limitadas y Workfront puede acceder a las carpetas y recursos de la organización en Adobe Experience Manager. Sin embargo, si se agrega una sola dirección IP a la lista de permitidos de Cloud Manager, la lista de permitidos supone que no se permite ninguna dirección IP que no esté en la lista. Por lo tanto, si la lista de permitidos Workfront de Cloud Manager incluye direcciones IP, estas también deben agregarse a la lista de permitidos para permitir que Workfront envíe recursos a Experience Manager Assets.

### Solución:

Añada las direcciones IP de Workfront a la lista de permitidos de Cloud Manager de Adobe.

* Para obtener instrucciones sobre cómo agregar direcciones IP al Cloud Manager de Adobe, consulte [Introducción a las Listas de permitidos IP](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) en la documentación de Adobe Experience Manager.
* Para obtener una lista de direcciones IP de Workfront que agregar a la lista de permitidos, consulte [Configuración del firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
