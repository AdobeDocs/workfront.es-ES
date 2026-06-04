---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Resolución de problemas en la integración de Adobe Experience Manager
description: 'Problema: los recursos no se guardan en Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
TQID: https://experienceleague.adobe.com/VaiQnZXQe39sYlnJOblWoea9UwOaujEU3ME-jh7-0EI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 247
ht-degree: 93%

---

# Resolución de problemas en la integración de Adobe Experience Manager

## Problema: los recursos no se guardan en Adobe Experience Manager

Cuando un usuario selecciona un recurso o una carpeta para exportarlos a Experience Manager Assets y hace clic en Seleccionar, la ventana del selector se cierra, pero los recursos no se guardan en Experience Manager Assets. Workfront no indica que los recursos no se hayan guardado en Experience Manager Assets.

### Causa

Esto puede ocurrir debido a la lista de permitidos de Adobe Cloud Manager. Si la lista de permitidos de Adobe Cloud Manager de una organización está vacía, las direcciones IP no están limitadas y Workfront puede acceder a las carpetas y recursos de la organización en Adobe Experience Manager. Sin embargo, si se añade una única dirección IP a la lista de permitidos de Cloud Manager, la lista de permitidos supone que no se permite ninguna dirección IP que no esté en la lista. Por lo tanto, si la lista de permitidos de Cloud Manager incluye direcciones IP, estas también deben añadirse a la lista de permitidos para permitir que Workfront envíe recursos a Experience Manager Assets.

### Solución:

Añada las direcciones IP de Workfront a la lista de permitidos de Adobe Cloud Manager.

* Para obtener instrucciones sobre cómo añadir direcciones IP a Adobe Cloud Manager, consulte [Introducción a las listas de permitidos de IP](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) en la documentación de Adobe Experience Manager.
* Para obtener una lista de direcciones IP de Workfront que añadir a la lista de permitidos, consulte [Configurar el cortafuegos](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
