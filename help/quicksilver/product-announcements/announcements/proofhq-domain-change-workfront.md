---
content-type: reference
navigation-topic: announcements
title: Cambio necesario para agregar pruebas a la lista de permitidos
description: El dominio de revisión cambia de proofhq.com a workfront.com.
author: Luke
feature: Product Announcements
exl-id: 05a1fd37-224b-4a0b-abef-4d9a015de524
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Cambio necesario para agregar pruebas a la lista de permitidos

El dominio de revisión está cambiando de from proofhq.com a workfront.com.

Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a proveedores específicos, debe añadir la siguiente URL adicional a su lista de permitidos para garantizar que los usuarios de su organización puedan ver las pruebas en Adobe Workfront tanto en el visor de revisión del explorador como en el visor de revisión de escritorio:

&#42;.workfront.com

La dirección URL &#42;proofhq.com también es obligatoria.

Para obtener más información sobre cómo actualizar la lista de permitidos, consulte [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Esta actualización solo se aplica a las pruebas en Workfront; no se aplica al utilizar la aplicación independiente de Workfront Proof.
