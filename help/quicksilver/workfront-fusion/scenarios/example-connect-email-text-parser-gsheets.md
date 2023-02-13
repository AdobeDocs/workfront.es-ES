---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 'Ejemplo de escenario de Adobe Workfront Fusion: Conecte el correo electrónico, el analizador de texto y las hojas de Google'
description: Esta situación le ayuda a crear un registro de todos los mensajes de correo electrónico y etiquetarlos para realizar acciones adicionales en una hoja de cálculo. Captura un cuerpo de correo electrónico en dos tablas independientes de una hoja de cálculo utilizando expresiones regulares (Regex) como patrones de búsqueda. El primer patrón busca una frase y la segunda busca la misma frase y una dirección de correo electrónico.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] ejemplo de escenario: Conectar correo electrónico, [!UICONTROL Analizador de texto]y [!DNL Google Sheets]

Esta situación le ayuda a crear un registro de todos los mensajes de correo electrónico y etiquetarlos para realizar acciones adicionales en una hoja de cálculo. Captura un cuerpo de correo electrónico en dos tablas independientes de una hoja de cálculo utilizando expresiones regulares (Regex) como patrones de búsqueda. El primer patrón busca una frase y la segunda busca la misma frase y una dirección de correo electrónico.

## Requisitos de acceso

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] o superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Este tutorial requiere conocimientos básicos de las expresiones regulares. Para obtener más información sobre Regex, visite [https://regexone.com](https://regexone.com/).

Añada el primer módulo y configúrelo

1. Busque Correo electrónico y elija **[!UICONTROL Ver correos electrónicos]** como Déclencheur.

   >[!NOTE]
   >
   >Mientras que puede conectar un [!DNL Google] cuenta que utiliza la Emódulo de correo, también puede utilizar un [!DNL Gmail] módulo.

1. Conecte una [!DNL Google] cuenta o cualquier otro cliente de correo electrónico basado en IMAP (como [!DNL Outlook]).
1. Una vez conectado, seleccione una carpeta cuyos correos electrónicos entrantes desee ver, como [!UICONTROL Bandeja de entrada].
1. En [!UICONTROL Criterios], elija **[!UICONTROL Todo el correo electrónico]** (o reducirlo a correos electrónicos leídos o no leídos).

   También puede elegir marcar los correos electrónicos recuperados como leídos o no leídos.

1. Configure las variables [!UICONTROL Número máximo de resultados] a 1.

   ![](assets/save-max-as-1-350x304.png)

   Puede cambiar esto en función del volumen de mensajes que reciba. Sin embargo, se recomienda establecer un valor bajo y ejecutar el escenario con más frecuencia.

1. Haga clic en **[!UICONTROL Mostrar configuración avanzada]** en la parte inferior.

   ![](assets/show-adv-settings-350x332.png)

1. Filtre los correos electrónicos por [!UICONTROL Dirección del remitente], [!UICONTROL Asunto] y [!UICONTROL Frase].

   Esto le permite ver solo los correos electrónicos relevantes. En este ejemplo, hemos añadido solo un filtro Subject y hemos dejado los otros 2 en blanco.

   >[!NOTE]
   >
   >Añadiremos un router para buscar frases en un correo electrónico usando la variable [!UICONTROL Patrón de coincidencia] iterador y expresión regular (Regex) como patrón de búsqueda. Esto también nos permite crear un escenario de utilidad múltiple.

1. Una vez que haya terminado la configuración y se le pedirá que especifique dónde desea comenzar a ver los correos electrónicos, haga clic en **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Continúe con [Buscar [!UICONTROL Control de flujo] y agregue un [!UICONTROL Enrutador]](#search-for-flow-control-and-add-a-router)

## Buscar [!UICONTROL Control de flujo] y agregue un [!UICONTROL Enrutador]

1. Agregue un router después de cualquier módulo para dividir o duplicar los datos antes de enviarlos al siguiente módulo.

   Aquí, hemos utilizado un [!UICONTROL Enrutador] para enviar el texto del cuerpo del correo electrónico a 2 tablas independientes en una [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## Utilice la variable [!UICONTROL Analizador de texto] Módulo

1. Agregue un [!UICONTROL Patrón de coincidencia] transformador para buscar una frase en un correo electrónico.

   Buscaremos la frase &quot;[!UICONTROL módulo analizador de texto]&quot; en todos los correos electrónicos entrantes para capturar el texto del cuerpo y el nombre del remitente de los que coinciden con esa frase.

   1. Escribir el patrón como una expresión regular:

      text\sparser\smoap

   1. (Opcional) Utilice cualquiera de las otras opciones de Patrón.

      ![](assets/pattern-350x318.png)

      Multilínea es útil si el texto contiene varias líneas y necesita buscar el patrón en cada línea. Para este tutorial necesitamos buscar el patrón en todo el texto del cuerpo del correo electrónico, por lo que lo dejaremos sin marcar.

   1. En el [!UICONTROL Texto] , haga clic en el atributo **Contenido del texto** en la lista.

      ![](assets/text-content-350x264.png)

      Este es el atributo que almacena el texto del cuerpo del correo electrónico en el que buscaremos el patrón.

1. Agregue otro [!UICONTROL Patrón de coincidencia] que busca la misma frase y una dirección de correo electrónico.

   Esto resulta especialmente útil si tiene cuentas de cliente con varios usuarios. Para ahorrar tiempo, puede clonar la variable [!UICONTROL Analizador de texto] módulo que acaba de crear y vincularlo al Router.

   ![](assets/clone.png)

1. Edite el patrón como se indica a continuación:

   text\sparser\smoap.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Este patrón busca la frase &quot;[!UICONTROL módulo analizador de texto]&quot; y una dirección de correo electrónico como john.doe@gmail.com y devuelve solo la dirección de correo electrónico.

   >[!NOTE]
   >
   >Es importante escribir su regex de acuerdo con la especificación de las direcciones de correo electrónico que acepta, pero la anterior se encarga de las direcciones de correo electrónico más estándar.

   * Si desea buscar únicamente direcciones de correo electrónico, puede utilizar la regex siguiente:

      ([\w.-]+@[\w.-]+)

   * También puede buscar solamente números de teléfono usando la regex de abajo:

      ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4} El patrón anterior cubre los formatos más comunes en los que se escribe un número de teléfono.
   Para probar los patrones, recomendamos usar [[!DNL https://regex101.com]](https://regex101.com/) con [!DNL javascript] como el Sabor.

   El resto de la configuración sigue siendo la misma que antes.

## Agregue la variable [!DNL Google Sheets] módulos

Para [!DNL Sheets], primero debemos crear una hoja de cálculo con los encabezados necesarios.

1. Cree una hoja de cálculo con las columnas en las que desea capturar los datos del usuario. (También puede utilizar un archivo existente).

   Por ejemplo, cree uno llamado &quot;Datos de correo electrónico: Compatibilidad con ticket&quot; con nombre de remitente, correo electrónico del remitente y contenido de correo electrónico como columnas. Asigne un nombre a la hoja de cálculo &quot;contiene: módulo analizador de texto&quot;.

1. Agregue la variable [!UICONTROL Hojas de Google] módulo con **[!UICONTROL Añadir una fila]** como la acción.

   ![](assets/add-a-row-350x174.png)

1. Conecte su [!DNL Google] (si aún no lo ha hecho). Elija el archivo que ha creado anteriormente, seguido de elegir la hoja de cálculo en la que está capturando los datos.

   La configuración debería tener este aspecto:

   ![](assets/connect-google-acct-350x279.png)

1. Asigne los atributos en los campos relevantes (columnas) para finalizar la configuración del módulo.

   ![](assets/map-attributes-350x282.png)

1. Clona el módulo que acaba de crear y lo vincula al segundo [!UICONTROL Analizador de texto] módulo.

   1. Vaya a la hoja de cálculo, duplique la hoja de cálculo que creó anteriormente y asígnele un nombre.

      Por ejemplo, asígnele el nombre &quot;contiene: módulo del analizador de texto y correo electrónico&quot;.

   1. Agregue otra columna para almacenar la dirección de correo electrónico que contiene el cuerpo del correo electrónico.

      Por ejemplo, asígnele el nombre &quot;Dirección de correo electrónico compartida&quot;.

   1. Haga clic en el [!DNL Google Sheets] para configurar la configuración.
   1. Cambie la hoja de cálculo por la nueva que acaba de crear.
   1. Asigne el resultado desde la variable [!UICONTROL Patrón de coincidencia] ($1) a la columna donde desea almacenar la dirección de correo electrónico (dirección de correo electrónico compartida).

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Haga clic en **[!UICONTROL OK]**, guarde el escenario y tómelo para una ejecución de prueba.

      Deberá enviar dos correos electrónicos independientes a la dirección de correo electrónico conectada de la siguiente manera:

      * Que contenga la frase &quot;[!UICONTROL módulo analizador de texto]&quot; (y sin dirección de correo electrónico)

         ![](assets/text-parser-module-350x103.png)

      * Que contiene la frase anterior y una dirección de correo electrónico

         ![](assets/above-phrase-and-email-350x106.png)

         Si no hay errores en la configuración, verá que la primera hoja de cálculo captura todos los correos electrónicos que contengan la frase &quot;[!UICONTROL módulo analizador de texto]&quot; mientras que la segunda hoja de cálculo captura solo aquellos que contienen la frase &quot;[!UICONTROL módulo analizador de texto]&quot; y una dirección de correo electrónico. Puede consultar las capturas de pantalla a continuación.

         Hoja de cálculo 1:

         ![](assets/worksheet-1-350x57.png)

         Hoja de cálculo 2:

         ![](assets/worksheet-2-350x41.png)

## Recursos

* [Ejercicios libres](https://regexone.com/) para obtener más información sobre las expresiones regulares
* [Obtenga información sobre la coincidencia de números de teléfono](https://regexone.com/problem/matching_phone_numbers) uso de Regex
* [Más información sobre la coincidencia de correo electrónico](https://regexone.com/problem/matching_emails) uso de Regex
* [Probar las expresiones regulares](https://regex101.com/)
