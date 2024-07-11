---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: módulo de Adobe Authenticator
description: Con el módulo Adobe Authenticator, puede conectarse a cualquier producto de Adobe con una API mediante una sola conexión.
author: Becky
feature: Workfront Fusion
exl-id: 74c943fb-37ad-4d91-8af7-9808ba69992e
source-git-commit: 443bdb5caee4b8a7ba9df95b0befff27b7aaabc2
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 1%

---

# Módulos de Adobe Authenticator

El módulo Adobe Authenticator le permite conectarse a cualquier API de Adobe mediante una sola conexión. Esto le permite conectarse más fácilmente a los productos de Adobe que aún no tienen un conector Fusion específico.

La ventaja sobre los módulos HTTP es que puede crear una conexión, como en una aplicación dedicada.

Para ver una lista de las API de Adobe disponibles, consulte [API de Adobe](https://developer.adobe.com/apis). Es posible que solo pueda utilizar las API que le han sido asignadas.

## Requisitos de acceso

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan</td>
      <td>
        <p>Nuevo: Cualquiera</p><p>O</p><p>Actual: [!UICONTROL Pro] o superior</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] licencia</td>
      <td>
        <p>Nuevo: estándar</p><p>O</p><p>Actual: [!UICONTROL Plan], [!UICONTROL Trabajo]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia</td>
      <td>
   <p>Requisito de licencia de Fusion actual: No [!DNL Workfront Fusion] requisito de licencia.</p>
   <p>O</p>
   <p>Requisito de licencia de Fusion heredada: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>
   <p>Nuevo plan de Workfront: si tiene [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>O</p>
   <p>Plan Workfront actual: su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td>
    </tr>
  </tbody>
</table>

## Requisitos previos

* Debe tener acceso al producto de Adobe al que desea conectarse el módulo.
* Debe tener acceso a Adobe Developer Console.
* Debe tener un proyecto en Adobe Developer Console que incluya la API a la que desea conectarse el módulo. Puede:

   * Cree un nuevo proyecto con la API.

     O
   * Añada la API a un proyecto existente.

  Para obtener información sobre cómo crear o añadir una API a un proyecto en Adobe Developer Console, consulte [Creación de un proyecto](https://developer.adobe.com/dep/guides/dev-console/create-project/) en la documentación del Adobe.

## Crear una conexión

Una conexión de Adobe Authenticator se conecta a un solo proyecto en Adobe Developer Console. Para utilizar la misma conexión para más de una API de Adobe, agregue las API al mismo proyecto y cree una conexión con ese proyecto.

Puede crear conexiones independientes a proyectos independientes, pero no puede utilizar una conexión para acceder a una API que no esté en el proyecto especificado en esa conexión.

>[!IMPORTANT]
>
>Con el conector de Adobe Authenticator, puede elegir entre realizar una conexión de servidor a servidor OAuth o una conexión de cuenta de servicio (JWT). La Adobe tiene credenciales de JWT obsoletas, que dejarán de funcionar el 1 de enero de 2025. **Por lo tanto, recomendamos encarecidamente la creación de conexiones de OAuth.**
>
>Para obtener más información sobre estos tipos de conexiones, consulte [Autenticación de servidor a servidor](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) en la documentación del Adobe

Para crear una conexión:

1. En cualquier módulo de Adobe Authenticator, haga clic en **Añadir** junto al campo Conexión.
1. Rellene los campos siguientes:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo de conexión]</td>
        <td>
          <p>Seleccione si desea crear una conexión de servidor a servidor OAuth o una conexión de cuenta de servicio (JWT).</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Nombre de conexión]</td>
        <td>
          <p>Escriba un nombre para esta conexión.</p>
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
        <td role="rowheader">[!UICONTROL Ámbitos]</td>
        <td>Si ha seleccionado una conexión OAuth, introduzca los ámbitos necesarios para esta conexión.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID de cuenta técnica]</td>
        <td>Introduzca su [!DNL Adobe] ID de cuenta técnica. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ID de organización]</td>
        <td>Si ha seleccionado una conexión JWT, introduzca su [!DNL Adobe] ID de organización. Esto se puede encontrar en la sección [!UICONTROL Credentials details] del [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL MetaÁmbitos]</td>
        <td>Si ha seleccionado una conexión JWT, introduzca los metaámbitos necesarios para esta conexión. </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Clave privada]</td>
        <td>
          <p>Si ha seleccionado una conexión JWT, introduzca la clave privada que se generó cuando se crearon las credenciales en [!DNL Adobe Developer Console]. </p>
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
      <tr>
        <td role="rowheader">[!UICONTROL URL base]</td>
        <td>Debe agregar las direcciones URL base que desea que permita este autenticador. Cuando utilice el módulo Crear una llamada de API personalizada más adelante en el escenario, agregará una ruta relativa a la dirección URL elegida. Al introducir las direcciones URL aquí, puede controlar a qué se puede conectar el módulo Crear una llamada de API personalizada, lo que aumenta la seguridad.<p>Para cada URL base que desee añadir al autenticador, haga clic en <b>Añadir elemento</b> e introduzca la dirección URL base.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL URL de autenticación]</td>
        <td>Deje esto en blanco para utilizar la URL de autenticación IMS estándar de Adobe. <code>https://ims-na1.adobelogin.com</code>. Si no utiliza Adobe IMS para la autenticación, introduzca la URL que desea utilizar para la autenticación.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Entorno]</td>
        <td>Seleccione si desea conectarse a un entorno de producción o de no producción.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Tipo]</td>
        <td>Seleccione si desea conectarse a una cuenta de servicio o a una cuenta personal.</td>
      </tr>
    </tbody>
    </table>

1. Clic **[!UICONTROL Continuar]** para guardar la conexión y volver al módulo.

## Módulo

### Realizar una llamada de API personalizada

Este módulo de acción le permite realizar una llamada a cualquier API de Adobe.

>[!TIP]
>
>Debe introducir la dirección URL completa de la API a la que desea conectarse. Este módulo no acepta direcciones URL relativas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Conexión]</td>
     <td>Para obtener instrucciones sobre cómo crear una conexión con el módulo de Adobe Authenticator, consulte <a href="#create-a-connection" class="MCXref xref" >Crear una conexión</a> en este artículo.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Introduzca la dirección URL completa del punto de API al que desea conectarse.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Método]</p>
   <td> <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, consulte <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Encabezados]</td>
      <td>
        <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p>
        <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion añade los encabezados de autorización automáticamente.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cadena de consulta]  </td>
      <td>
        <p>Introduzca la cadena de consulta de solicitud.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Cuerpo]</td>
   <td> <p>Añada el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar.</p> <p>Nota:  <p>Cuando se utilizan afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera del enunciado condicional.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Límite]  </td>
      <td>
        <p>Introduzca el número máximo de resultados que desea que devuelva el módulo en un ciclo de ejecución.</p>
      </td>
    </tr>
  </tbody>
</table>
