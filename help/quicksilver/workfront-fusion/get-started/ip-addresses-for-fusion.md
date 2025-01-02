---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Direcciones IP para acceder a Adobe Workfront Fusion
description: Adobe Workfront Fusion requiere una licencia Adobe Workfront Fusion y de Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 800cf889ff2729fca0c9d75d0ace0ecc1ee53a79
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 10%

---

# Direcciones IP para acceder a [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere una licencia de [!DNL Adobe Workfront Fusion] además de [!DNL Adobe Workfront license].

Si el firewall o el servidor de correo están configurados para permitir el acceso sólo a determinados proveedores, debe agregar determinadas direcciones IP a su lista de permitidos para permitir la comunicación abierta entre su entorno y [!DNL Adobe Workfront Fusion].

Puede añadir todas las direcciones IP y dominios de Fusion a la lista de permitidos o puede localizar el clúster de Fusion y añadir solo las direcciones IP y los dominios de ese clúster.

## Añadir todas las direcciones IP y dominios de Fusion

Añada las siguientes direcciones IP a su lista de permitidos:

* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

Además, si su organización utiliza el filtrado de red saliente, añada el siguiente dominio a su lista de permitidos para permitir que su sistema acceda a Workfront Fusion. Se utilizan para los webhooks.

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## Añadir direcciones IP y dominios de Fusion solo para su clúster

### Identificación del centro de datos

Las direcciones IP varían en función del lugar en el que se almacenan los datos.

Si accede a Fusion a través de una dirección URL, puede examinarla para localizar el centro de datos.

| URL | Datacenter |
| --- | --- |
| `https://app.workfrontfusion.com/` | centro de datos estadounidense |
| `https://app-eu.workfrontfusion.com/` | centro de datos UE |
| `https://app-az.workfrontfusion.com/` | Azure Datacenter |

Si accede a Fusion a través de experience.adobe.com, puede comprobar la pestaña de red en su explorador para identificar el centro de datos.

| URL | Datacenter |
| --- | --- |
| Llamadas a `https://fusion.adobe.com` | centro de datos estadounidense |
| Llamadas a `https://eu.fusion.adobe.com` | centro de datos UE |
| Llamadas a `https://az.fusion.adobe.com` | Azure Datacenter |

### Añadir direcciones IP y dominios al centro de datos

Agregue las siguientes direcciones IP a su lista de permitidos para permitir que [!DNL Workfront Fusion] acceda a su sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Centro de datos UE</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US Datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li>
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] en el clúster de Microsoft Azure</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Además, si su organización utiliza el filtrado de red saliente, añada el siguiente dominio a su lista de permitidos para permitir que su sistema acceda a Workfront Fusion.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Centro de datos UE</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] en el clúster de Microsoft Azure</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>El filtrado de red saliente es poco común. Consulte con el administrador de la red si necesita actualizar la lista de permitidos para adaptarla.

Para obtener más información sobre cómo configurar la lista de permitidos de su organización, consulte [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
