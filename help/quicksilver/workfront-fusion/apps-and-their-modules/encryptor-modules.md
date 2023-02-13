---
title: Cifrado
description: Los módulos del cifrado de Adobe Workfront Fusion le permiten cifrar cualquier dato de texto. Actualmente son compatibles con el cifrado de mensajes a través de AES256 y PGP (OpenPGP).
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 9664c4f1-6467-45c9-8b9e-5a41d0e9ccb9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Cifrado

[!DNL Adobe Workfront Fusion] [!UICONTROL Cifrado] los módulos permiten cifrar cualquier dato de texto. Actualmente admiten el cifrado de mensajes a través de AES256 y PGP ([!UICONTROL OpenPGP]).

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>   <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Encriptado y descifrado de mensajes con PGP

Al cifrar y descifrar mediante PGP, es necesario utilizar un llavero y crear una clave privada o pública (o ambas).

Para obtener más información sobre claves públicas y privadas, consulte [Términos básicos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/basic-terms.md). Para obtener más información sobre las cadenas de claves, consulte [Claves en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/connections/keys.md).

## [!UICONTROL Cifrado] módulos y sus campos

Al configurar [!UICONTROL Cifrado] , se muestran los campos siguientes. Un título en negrita en un módulo indica un campo obligatorio.

### Codificar un mensaje PGP

Este módulo le permite cifrar un mensaje utilizando claves públicas y privadas.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Clave privada]</td>
        <td>Introduzca la clave privada del remitente. Esto puede autenticar la identidad del remitente.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Clave pública]</td>
        <td>Introduzca la clave pública del destinatario.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Mensaje]</td>
        <td>Introduzca el mensaje que desea cifrar.</td>
    </tr>

### Descifrar un mensaje PGP

Este módulo le permite descifrar un mensaje con claves públicas y privadas.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Clave privada]</td>
        <td>Introduzca la clave privada del destinatario.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Clave pública]</td>
        <td>Introduzca la clave pública del destinatario. Esto puede autenticar la identidad del remitente.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Mensaje]</td>
        <td>Asigne el mensaje que desee descifrar.</td>
    </tr>
</table>
