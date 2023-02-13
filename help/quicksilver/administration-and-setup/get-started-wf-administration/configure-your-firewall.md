---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar la lista de permitidos del cortafuegos
description: Si el servidor de firewall o de correo está configurado para permitir el acceso solo a determinados proveedores, debe añadir ciertas direcciones IP a su lista de permitidos. Esto abre la comunicación entre su entorno y los servidores de Adobe Workfront y permite a los usuarios enviar mensajes desde Workfront y utilizar SSO con Active Directory o LDAP.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 13%

---

# Configurar la lista de permitidos del cortafuegos

>[!IMPORTANT]
>
>El procedimiento descrito en esta página solo se aplica a organizaciones que aún no se han incorporado al Admin Console. Si su organización se ha incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para configurar la lista de permitidos si su organización se ha incorporado a Adobe Admin Console, consulte [Dominios permitidos para aplicaciones y servicios de Adobe](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Para obtener una lista de procedimientos que difieren en función de si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración basadas en plataformas (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Si el servidor de firewall o de correo está configurado para permitir el acceso solo a determinados proveedores, debe añadir ciertas direcciones IP a su lista de permitidos. Esto abre la comunicación entre su entorno y los servidores de Adobe Workfront y permite los siguientes procesos:

* Envío de mensajes desde la aplicación Workfront

   >[!NOTE]
   >
   >Esto no está disponible si la instancia de Workfront de su organización está habilitada con Adobe IMS. Si necesita más información, consulte con su administrador de red o TI.

* Uso de webhooks de documentos al configurar integraciones de documentos personalizadas
* Uso de suscripciones a eventos de Workfront

   Para obtener más información, consulte [API de suscripción de evento](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

También debe abrir ciertos puertos para que los mensajes de correo electrónico se cifren cuando se envíen.

## Listas de permitidos de Workfront que puede usar

Si su organización tiene el plan de Enterprise, también puede configurar dos listas de permitidos de Workfront:

* **Lista de permitidos de correo electrónico**: Le permite controlar dónde pueden enviar por correo electrónico los datos almacenados en Workfront. Para obtener más información, consulte [Configurar la lista de permitidos de correo electrónico](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **LISTA DE PERMITIDOS IP**: Limita el acceso a Workfront a 45 direcciones IP o rangos de direcciones IP que especifique, lo que proporciona una capa adicional de seguridad para la aplicación Workfront. Para obtener más información, consulte [Restringir el acceso a Adobe Workfront por dirección IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Direcciones IP que se agregarán a la lista de permitidos

Las direcciones IP que debe agregar a la lista de permitidos en el cortafuegos dependen del clúster en el que se ejecuta el entorno de producción. Para saber cuál es este clúster, consulte Configuración > Sistema > Información personalizada. Para obtener más información, consulte la sección [Configurar información básica](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md#configuring-basic-info) en el artículo [Configurar información básica para el sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

>[!IMPORTANT]
>
>Algunas integraciones de Workfront no funcionan cuando la lista de permitidos está habilitada porque no se pueden configurar con una dirección IP estática. Para utilizar las integraciones siguientes, debe desactivar la lista de permitidos .
>
>* Workfront para G Suite
>* Workfront para Outlook
>* Workfront para Salesforce


* [Direcciones IP para permitir los clústeres 1, 2, 3, 5, 7, 8 y 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Direcciones IP que permiten el clúster 4](#ip-addresses-to-allow-for-cluster-4)
* [Direcciones IP para permitir el clúster 6](#ip-addresses-to-allow-for-cluster-6)
* [Direcciones IP para permitir una unidad de prueba](#IP%20Addre2)
* [Direcciones IP permitidas al implementar suscripciones de eventos](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Direcciones IP para permitir una autenticación mejorada](#ip-addresses-to-allow-for-enhanced-authentication)
* [Direcciones IP que agregar para acceder a Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Direcciones IP que se agregan para usar Workfront para Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [Direcciones IP que se agregan para usar Workfront Ascent](#ip-addresses-to-add-for-using-workfront-ascent)
* [URL que se agregarán para todos los clústeres Workfront](#urls-to-add-for-all-clusters-workfront)

### Direcciones IP para permitir los clústeres 1, 2, 3, 5, 7, 8 y 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Si el entorno de producción se encuentra en los clústeres 1, 2, 3, 5 o 7, debe permitir las siguientes direcciones IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para SSO, enlaces web de documentos u otras funciones</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para recibir correo electrónico de la aplicación Workfront</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>Para obtener información sobre las siguientes direcciones IP, consulte <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md" class="MCXref xref">Nuevas direcciones IP para el correo electrónico de Adobe Workfront con la versión 21.1</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Direcciones IP que permiten el clúster 4 {#ip-addresses-to-allow-for-cluster-4}

Si el entorno de producción está en el clúster 4, añada las siguientes direcciones IP para SSO, documentar integraciones de weblock y recibir correo electrónico de la aplicación Workfront:

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230.232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122

Para obtener información sobre las siguientes direcciones IP, consulte [Nuevas direcciones IP para el correo electrónico de Adobe Workfront con la versión 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md)

* 23.251.239.98
* 23.251.239.99

### Direcciones IP para permitir el clúster 6 {#ip-addresses-to-allow-for-cluster-6}

Si el entorno de producción está en el clúster 6, agregue las siguientes direcciones IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para recibir correo electrónico de la aplicación Workfront</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para utilizar el servicio de correo electrónico de AWS</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Direcciones IP para permitir una unidad de prueba

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Recibir correo electrónico de la aplicación Workfront al utilizar una unidad de prueba</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para integraciones de SSO y weblock de documentos al utilizar una unidad de prueba</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>Esta dirección también debe agregarse a la lista de permitidos para que los usuarios puedan recibir correos electrónicos de Workfront.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Direcciones IP permitidas al implementar suscripciones de eventos  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Para todos los entornos, agregue las siguientes direcciones IP para recibir cargas útiles desde suscripciones de eventos de Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Para clientes de Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para clientes en ubicaciones distintas de Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Direcciones IP para permitir una autenticación mejorada {#ip-addresses-to-allow-for-enhanced-authentication}

Añada las siguientes direcciones IP para utilizar la autenticación mejorada para la vista previa o la producción.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Si su entorno está en el clúster 1, 2, 3, 5, 7, 8 o 9</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Si su entorno está en el clúster 4</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Direcciones IP que agregar para acceder a Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Añada las siguientes direcciones IP a su lista de permitidos para permitir que Workfront Fusion acceda a su sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Centro de datos de la UE de Adobe Workfront</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Además, si su organización utiliza el filtrado de red saliente, agregue el siguiente dominio a su lista de permitidos para permitir que su sistema acceda a Workfront Fusion.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Centro de datos de la UE de Adobe Workfront</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>El filtrado de red saliente no es común. Consulte con el administrador de red para ver si debe actualizar la lista de permitidos para adaptarla.

### Direcciones IP que se agregan para usar Workfront para Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Añada las siguientes direcciones IP a su lista de permitidos para utilizar la integración de Workfront para Jira.

El dominio jira.workfront.com también debe ser accesible desde los servidores corporativos. Este dominio es obligatorio porque sirve como middleware entre Workfront y Jira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Para clientes de Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para clientes en ubicaciones distintas de Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Direcciones IP que se agregan para usar Workfront Ascent {#ip-addresses-to-add-for-using-workfront-ascent}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para acceder a los recursos de formación de Workfront mediante Workfront Ascent</td> 
   <td> 
    <ul> 
     <li>18.223.140.34</li> 
     <li>3.13.223.30</li> 
     <li>3.13.19.112</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para recibir notificaciones por correo electrónico de Workfront Ascent</td> 
   <td> 
    <ul> 
     <li>23.251.227.75</li> 
     <li>23.251.227.76</li> 
     <li>23.251.227.77</li> 
     <li>23.251.227.78</li> 
     <li>23.251.227.79</li> 
     <li>23.251.227.80</li> 
     <li>23.251.227.81</li> 
     <li>23.251.227.82</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Dominios que se agregan para acceder a Workfront

Si su organización utiliza el filtrado de red saliente, agregue los siguientes dominios a su lista de permitidos para permitir que su sistema acceda a Workfront.

>[!NOTE]
>
>El filtrado de red saliente no es común. Consulte con el administrador de red para ver si debe actualizar la lista de permitidos para adaptarla.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/

## URL que se agregarán para todos los clústeres Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para permitir que el contenido de ayuda se muestre en su entorno de Workfront</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para permitir que Workfront Proof acceda a Workfront en cualquier clúster, agréguelos a todos los entornos</td> 
   <td> 
    <ul> 
     <li>*.workfront.com : necesario para ver pruebas en Workfront</li> 
     <li>*.proofhq.com: necesario para ver pruebas en Workfront Proof</li> 
     <li>*.proofhq.eu - Necesario para ver pruebas en Workfront Proof</li> 
    </ul> <p><b>NOTA</b>:  <p>No se pueden agregar direcciones IP a la lista de permitidos para Workfront Proof. Han sido dinámicos después de que Workfront se trasladara a AWS. En su lugar, se recomienda permitir solo dominios de prueba de Workfront.</p> <p>Si hay algún problema con la adición de estos dominios a la lista de permitidos y necesita una dirección IP, póngase en contacto con el servicio de atención al cliente de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Direcciones IP y direcciones URL que se agregarán para acceder a la prueba de Workfront

Debe añadir las siguientes direcciones IP a la lista de permitidos para poder utilizar varias funciones.

* [Para llamadas de retorno y pruebas de captura web](#for-callbacks-and-webcapture-proofs)
* [Para el correo electrónico saliente](#for-outgoing-email)

### Para llamadas de retorno y pruebas de captura web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (Clústeres 1, 2, 3, 5 y 7)</td> 
   <td> 
    <ul> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>NOTA</b>: Ya no se admiten las opciones del servidor DNS.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Para el correo electrónico saliente {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (Clústeres 1, 2, 3, 5 y 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Puertos que se abren para el mejor rendimiento de la prueba de Workfront

Abra los puertos siguientes si tiene problemas con la carga de pruebas o no funciona en Workfront Proof:

* 5671
* 5672
* 15671

## Puertos que se abrirán para correo electrónico cifrado

Los correos electrónicos de la aplicación Workfront se envían cifrados utilizando los puertos 465 y 587. Si su servidor de correo no admite correos electrónicos cifrados, los correos electrónicos se envían sin encriptar utilizando el puerto 25.

## Notificaciones por correo electrónico de la asistencia de Workfront

Si no recibe correos electrónicos de la asistencia de Workfront, asegúrese de agregar los dominios y las direcciones IP de Salesforce que necesite. Para obtener más información, consulte el artículo de ayuda de Salesforce sobre las direcciones IP y los dominios permitidos de Salesforce.
