---
content-type: reference
navigation-topic: announcements
title: Cambio necesario para agregar pruebas a la lista de permitidos
description: El dominio de prueba está cambiando de proofhq.com a workfront.com.
author: Luke
feature: Product Announcements
exl-id: 05a1fd37-224b-4a0b-abef-4d9a015de524
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Cambio necesario para agregar pruebas a la lista de permitidos

El dominio de prueba está cambiando de proofhq.com a workfront.com.

Si el servidor de seguridad o de correo está configurado para permitir acceso solo a proveedores específicos, debe agregar la siguiente URL adicional a la lista de permitidos para garantizar que los usuarios de su organización puedan ver pruebas en Adobe Workfront tanto en el visor de pruebas del explorador como en el visor de pruebas del escritorio:

&#42;.workfront.com

La variable &#42;la URL de proofhq.com también es obligatoria.

Para obtener más información sobre cómo actualizar la lista de permitidos, consulte [Configurar la lista de permitidos del cortafuegos](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Esta actualización solo se aplica a las pruebas en Workfront; no se aplica cuando se utiliza la aplicación independiente Workfront Proof.
