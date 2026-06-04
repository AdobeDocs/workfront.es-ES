---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configuración de la Lista de permitidos del cortafuegos
description: Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a determinados proveedores, debe añadir determinadas direcciones IP a su lista de permitidos. Esto abre la comunicación entre su entorno y los servidores de Adobe Workfront y permite a los usuarios enviar mensajes desde Workfront y utilizar SSO con Active Directory o LDAP.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
TQID: https://experienceleague.adobe.com/voAiMROhu9NJkN-WLjPWcpDu-x8YYgtlZNeNWk8dFjA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: ec8965fc-2f75-47f6-a9bb-730e8c2725f3
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1456
ht-degree: 11%

---

# Configuración de la lista de permitidos del cortafuegos

<!-- Audited: 12/2023 -->

<!--Follow up October 2026-->

>[!IMPORTANT]
>
>El procedimiento descrito en esta página se aplicaba únicamente a las organizaciones que aún no se habían incorporado a Admin Console. Dado que todas las organizaciones se han incorporado a Adobe Admin Console, debe realizar esta acción a través de Adobe Admin Console.
>
>Para configurar la lista de permitidos una vez que su organización se haya incorporado a Adobe Admin Console, consulte [Dominios permitidos para aplicaciones y servicios de Adobe](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Para obtener una lista de procedimientos que difieren según si su organización se ha incorporado a Adobe Admin Console, consulte [Diferencias de administración entre Adobe Workfront y Adobe Business Platform](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>La forma en que una organización configura su lista de permitidos es única para cada organización. Trabaje con su equipo de TI para identificar el procedimiento de su organización e implementar estas adiciones.

Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a determinados proveedores, debe añadir determinadas direcciones IP a su lista de permitidos. Esto abre la comunicación entre su entorno y los servidores de Adobe Workfront y permite los siguientes procesos:

* Uso de los webhooks de documentos al configurar integraciones de documentos personalizadas
* Uso de suscripciones a eventos de Workfront

  Para obtener más información, consulte [API de suscripción a eventos](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

También debe abrir ciertos puertos para que los mensajes de correo electrónico se cifren cuando se envíen.

## listas de permitidos de Workfront que puede utilizar

Si su organización tiene el plan Enterprise, también puede configurar dos listas de permitidos de Workfront:

* **lista de permitidos por correo electrónico**: permite controlar dónde pueden enviar los usuarios los datos almacenados en Workfront. Para obtener más información, consulte [Configuración de la lista de permitidos por correo electrónico](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **lista de permitidos IP**: limita el acceso a Workfront a 75 direcciones IP o rangos de direcciones IP que especifique, lo que proporciona un nivel de seguridad adicional para la aplicación Workfront. Para obtener más información, consulte [Restringir el acceso a Adobe Workfront por la dirección IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Busque el clúster de Workfront

Las direcciones IP que debe agregar a la lista de permitidos en el cortafuegos dependen del clúster en el que se ejecute el entorno de producción.

Para localizar el clúster de su organización:

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en **Sistema** y, a continuación, seleccione **Información del cliente**.
1. Busque el campo **Configuración de clúster** en la esquina superior derecha de la página. El clúster de su organización se muestra aquí.

   CL01 hace referencia al clúster 1, CL02 al clúster 2, etc.

Para obtener más información, consulte la sección [Ver el clúster de su organización y el plan de Workfront](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) en el artículo [Descripción general del firewall](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## Direcciones IP que agregar a la lista de permitidos

* [Direcciones IP que permiten los clústeres 1, 2, 3, 5, 7, 8 y 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Direcciones IP para permitir el clúster 4](#ip-addresses-to-allow-for-cluster-4)
* [Direcciones IP para permitir el clúster 6](#ip-addresses-to-allow-for-cluster-6)
* [Direcciones IP para permitir el clúster 10](#ip-addresses-to-allow-for-cluster-10)
* [Direcciones IP para permitir una unidad de prueba](#IP%20Addre2)
* [Direcciones IP que se permitirán al implementar suscripciones de evento](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Direcciones IP que agregar para acceder a Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Direcciones IP que agregar para usar Workfront para Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [Direcciones URL que se agregarán para todos los clústeres en Workfront](#urls-to-add-for-all-clusters-workfront)

### Para recibir correo electrónico desde la aplicación de Workfront

Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a determinados proveedores, debe añadir las siguientes direcciones IP a la lista de permitidos para recibir correo electrónico de la aplicación de Workfront.

#### Regiones de EE. UU.: clústeres 1, 2, 3, 5, 6, 7, 8, 9 y 10

* 206.55.149.211
* 206.55.149.212
* 206.55.149.213
* 206.55.149.214
* 206.55.149.215
* 23.251.237.106
* 23.251.237.107
* 23.251.237.108
* 23.251.237.109
* 54.240.119.54
* 54.240.119.55
* 54.240.60.174
* 54.240.60.175
* 54.240.61.222
* 54.240.61.223

#### Regiones de la UE: clústeres 4, 11, 12 y 13

* 23.251.239.98
* 23.251.239.99
* 24.110.76.223
* 24.110.76.224
* 69.169.230.231
* 69.169.230.232


### SSO, integraciones de ganchos web de documentos y otras funcionalidades

#### Regiones de EE. UU.: clústeres 1, 2, 3, 5, 6, 7, 8, 9 y 10

**Clústeres 1, 2, 3, 5, 6, 7, 8, 9**


* 35.160.0.242
* 34.213.36.118
* 3.209.27.146
* 18.205.251.4
* 34.211.224.9
* 54.218.48.56
* 52.36.154.34
* 54.244.142.219
* 52.39.217.230
* 44.241.82.96
* 54.203.255.135/32
* 35.155.2.51/32
* 52.34.192.77/32

**Clúster 10**

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

#### Regiones de la UE: agrupaciones 4 y 11


**Custer 4**

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
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
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32


### Direcciones IP para permitir una unidad de prueba

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para recibir correo electrónico desde la aplicación de Workfront al usar una unidad de prueba</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para integraciones de SSO y webhook de documentos al usar una unidad de prueba</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>Esta dirección también debe añadirse a la lista de permitidos para que los usuarios reciban correos electrónicos de Workfront.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Direcciones IP que se permitirán al implementar suscripciones de evento  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Para todos los entornos, añada las siguientes direcciones IP para recibir cargas útiles de suscripciones de evento de Workfront.

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
   <td role="rowheader">Para clientes de ubicaciones distintas de Europa</td> 
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

### Direcciones IP que añadir para acceder a Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Añada las siguientes direcciones IP a su lista de permitidos para permitir que Workfront Fusion acceda a su sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Centro de datos Adobe Workfront EU</td> 
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

Además, si su organización utiliza el filtrado de red saliente, añada el siguiente dominio a su lista de permitidos para permitir que su sistema acceda a Workfront Fusion. Estas direcciones URL se utilizan para los webhooks en Fusion.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Centro de datos Adobe Workfront EU</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
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

### Direcciones IP que se agregarán para usar Workfront para Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

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
   <td role="rowheader">Para clientes de ubicaciones distintas de Europa</td> 
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

## Dominios que se agregarán para acceder a Workfront

Si su organización utiliza el filtrado de red saliente, agregue los siguientes dominios a la lista de permitidos para permitir que el sistema acceda a Workfront.

>[!NOTE]
>
>El filtrado de red saliente es poco común. Consulte con el administrador de la red si necesita actualizar la lista de permitidos para adaptarla.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* fonts.gstatic.com
* dpm.demdex.net
* storage.googleapis.com
* snippet.maze.co
* *.aptrinsic.com
* *.static.workfront.com


  Este es un dominio estático que abarca todos los dominios siguientes. Puede agregar los dominios individuales si lo prefiere:

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com

Como su organización se encuentra en la experiencia unificada de Adobe, utiliza los siguientes dominios. Estos dominios están cubiertos en `*.adobe.com`, pero se pueden agregar si lo desea.

* &lt;su dominio>.my.workfront.adobe.com
* &lt;su dominio>.preview.workfront.adobe.com
* &lt;su dominio>.sb01.workfront.adobe.com
* &lt;su dominio>.sb02.workfront.adobe.com


Para Workfront Fusion, añada los siguientes dominios:

<!--Remove me October 2026-->

* Para las organizaciones que no están en la experiencia unificada de Adobe:
   * app.workfrontfusion.com (US AWS)
   * app-eu.workfrontfusion.com (EU AWS)
   * app-az.workfrontfusion.com (US Azure)

* Para la organización en la experiencia unificada de Adobe
(Estos dominios están cubiertos en `*.adobe.com`, pero se pueden agregar si lo desea).

   * fusion.adobe.com
   * app-eu.fusion.adobe.com
   * app-az.fusion.adobe.com



## Direcciones URL que se agregarán para todos los clústeres en Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para permitir que el contenido de ayuda se muestre en el entorno de Workfront</td> 
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
     <li>*.workfront.com: obligatorio para ver pruebas en Workfront</li> 
     <li>*.proofhq.com: obligatorio para ver pruebas en Workfront Proof</li> 
     <li>*.proofhq.eu: obligatorio para ver pruebas en Workfront Proof</li> 
    </ul> <p><b>NOTA</b>:  <p>No admitimos la adición de direcciones IP a su lista de permitidos para Workfront Proof. Han sido dinámicos después de que Workfront se trasladara a AWS. En su lugar, le recomendamos que solo permita dominios de Workfront Proof.</p> <p>Si hay algún problema con la adición de estos dominios a la lista de permitidos y necesita una dirección IP, póngase en contacto con el servicio de atención al cliente de Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Direcciones IP y URL que añadir para acceder a Workfront Proof

Debe añadir las siguientes direcciones IP a la lista de permitidos para utilizar varias funciones.

* [Para devoluciones de llamadas y pruebas de captura web](#for-callbacks-and-webcapture-proofs)
* [Para correo electrónico saliente](#for-outgoing-email)

### Para devoluciones de llamadas y pruebas de captura web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (clústeres 1, 2, 3, 5 y 7)</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
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
   <td role="rowheader">Prod-EU (grupo 4)</td> 
   <td> 
    <ul> 
    <li>34.255.252.190</li>
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
    </ul> <p><b>NOTA</b>: ya no se admiten las opciones del servidor DNS.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Para correo electrónico saliente {#for-outgoing-email}

Consulte [Para recibir correo electrónico desde la aplicación Workfront](#to-receive-email-from-the-workfront-application) sección anterior.


## Puertos para abrir y obtener el mejor rendimiento de Workfront Proof

Abra los siguientes puertos si tiene problemas con la carga de pruebas o no funciona en Workfront Proof:

* 5671
* 5672
* 15671

## Puertos que se abrirán para el correo electrónico cifrado

Los correos electrónicos de la aplicación de Workfront se envían cifrados mediante los puertos 465 y 587. Si el servidor de correo no admite el correo electrónico cifrado, los correos electrónicos se envían sin cifrar mediante el puerto 25.

## Notificaciones por correo electrónico del Soporte de Workfront

Si no recibe correos electrónicos del Soporte técnico de Workfront, asegúrese de añadir las direcciones IP y los dominios de Salesforce que necesita. Para obtener más información, consulte el artículo de ayuda de Salesforce acerca de las direcciones IP y los dominios de Salesforce que se van a permitir.
