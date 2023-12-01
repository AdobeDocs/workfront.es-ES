---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de Adobe Experience Manager Forms
description: Con el [!DNL Adobe Experience Manager Forms] conector para [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Forms] crear, cargar y actualizar recursos, y copiar o mover carpetas y recursos.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: c4e068729d8de4bef4b2018868e3fa020ca61a06
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# [!DNL Adobe Experience Manager Forms] módulos

Con el [!DNL Adobe Experience Manager Forms] conector para [!DNL Adobe Workfront Fusion], puede iniciar un escenario basado en eventos en su [!DNL Adobe Experience Manager Forms] creando un webhook.

Puede configurar un formulario en [!DNL Adobe Experience Manager Forms] para enviar envíos de formularios a este webhook.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito actual del producto: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

* Debe tener un [!DNL Adobe Experience Manager Forms] cuenta para utilizar este módulo.

## Creación de una conexión con Adobe Experience Manager Forms

Para crear una conexión para su [!DNL Adobe Experience Manager Forms] módulos:

1. Clic **[!UICONTROL Añadir]** situado junto al cuadro Conexión.

1. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
        <td>
          <p>Escriba un nombre para esta conexión.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Entorno]</td>
        <td>
          <p>Seleccione si esta conexión se conecta a un entorno de producción o de no producción.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo]</td>
        <td>
          <p>Seleccione si esta cuenta es una cuenta de servicio o personal.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">URL de instancia de [!UICONTROL sin barra diagonal]</td>
        <td>
          <p>Introduzca la URL que utiliza para acceder a la cuenta, sin la barra final.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Extremo [!UICONTROL IMS]</td>
        <td>
          <p><code>https://ims-na1.adobelogin.com</code></p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID de cliente]</td>
        <td>Introduzca su [!DNL Adobe] ID de cliente. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Secreto de cliente]</td>
        <td>Introduzca su [!DNL Adobe] Secreto del cliente. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Org ID]</td>
        <td>Introduzca su [!DNL Adobe] ID de organización. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
        <td>Introduzca su [!DNL Adobe] ID de cuenta técnica. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL MetaÁmbitos]</td>
        <td>Introduzca los metaámbitos adecuados       </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Clave privada]</td>
        <td>
          <p>Introduzca la clave privada que se generó cuando se crearon las credenciales en la [!DNL Adobe Developer Console]. </p>
          <p>Para extraer la clave privada o el certificado:</p>
          <ol>
            <li value="1">
              <p>Clic <b>[!UICONTROL Extraer]</b>.</p>
            </li>
            <li value="2">
              <p>Seleccione el tipo de archivo que está extrayendo.</p>
            </li>
            <li value="3">
              <p>Seleccione el archivo que contiene la clave privada o el certificado.</p>
            </li>
            <li value="4">
              <p>Introduzca la contraseña del archivo.</p>
            </li>
            <li value="5">
              <p>Clic <b>[!UICONTROL Guardar]</b> para extraer el archivo y volver a la configuración de conexión.</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. Clic **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## Módulo Adobe Experience Manager Forms y sus campos

Actualmente, solo hay un módulo en el conector de Adobe Experience Manager Forms.

### Buscar eventos de formulario

Este déclencheur instantáneo (webhook) le permite iniciar un escenario cuando se produce una acción de envío en un formulario Adobe Experience Manager Forms.

>[!IMPORTANT]
>
>Este módulo también requiere configuración en Adobe Experience Manager. Después de configurar este webhook, debe abrir Adobe Experience Manager y configurar su formulario para enviar envíos al webhook.
>
><!--For instructions on the required form configuration, see insert url here-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Nombre de webhook de [!UICONTROL]</td> 
   <td> <p>Escriba un nombre para el webhook</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su [!DNL Adobe Experience Manager] cuenta a [!DNL Workfront Fusion], consulte <a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">Cree una conexión con [!DNL Adobe Experience Manager Forms]</a></p> </td> 
  </tr>

El módulo crea un webhook y le proporciona la dirección del webhook, que puede introducir en el cuadro de diálogo de envío del formulario en [!DNL Adobe Experience Manager Forms].











