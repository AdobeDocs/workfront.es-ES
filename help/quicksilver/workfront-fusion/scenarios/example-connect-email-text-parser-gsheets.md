---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 'Ejemplo de escenario de Adobe Workfront Fusion: Conectar correo electrónico, analizador de texto y hojas de Google'
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 96%

---

# Ejemplo de escenario [!DNL Adobe Workfront Fusion]: conectar correo electrónico, [!UICONTROL analizador de texto] y [!DNL Google Sheets]

>[!IMPORTANT]
>
>Este artículo se eliminará en un futuro próximo.

Este escenario le ayuda a crear un registro de todos los mensajes de correo electrónico y a etiquetarlos para realizar más acciones en una hoja de cálculo. Registra un cuerpo del correo electrónico en dos tablas independientes en una hoja de cálculo utilizando expresiones regulares (Regex) como patrones de búsqueda. El primer patrón busca una frase y el segundo busca la misma frase y una dirección de correo electrónico.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td role="rowheader">Licencia** de [!UICONTROL Adobe Workfront Fusion]</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere la licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront] su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Requisitos previos

Este tutorial requiere conocimientos básicos de expresiones regulares. Para obtener más información sobre Regex, visite [https://regexone.com](https://regexone.com/).

Añadir el primer módulo y configurarlo

1. Busque Correo electrónico y elija **[!UICONTROL Ver correos electrónicos]** como activador.

   >[!NOTE]
   >
   >Aunque puede conectar una cuenta de [!DNL Google] mediante el módulo Correo electrónico, también puede usar el módulo [!DNL Gmail].

1. Conecte una cuenta de [!DNL Google] o cualquier otro cliente de correo electrónico basado en IMAP (como [!DNL Outlook]).
1. Una vez conectado, seleccione una carpeta cuyos correos electrónicos entrantes desee ver, como [!UICONTROL bandeja de entrada].
1. En [!UICONTROL Criterio], elija **[!UICONTROL Todos los correos electrónicos]** (o reduzca para leer o no leer correos electrónicos).

   También puede elegir marcar los correos electrónicos recuperados como leídos o no leídos.

1. Establezca el [!UICONTROL número máximo de resultados] en 1.

   ![](assets/save-max-as-1-350x304.png)

   Puede cambiar esto en función del volumen de mensajes que reciba. Sin embargo, se recomienda establecer un valor bajo y ejecutar el escenario con más frecuencia.

1. Haga clic en **[!UICONTROL Mostrar ajustes avanzados]** en la parte inferior.

   ![](assets/show-adv-settings-350x332.png)

1. Filtre los correos electrónicos por [!UICONTROL Dirección del remitente], [!UICONTROL Sujeto] y [!UICONTROL Frase].

   Esto le permite ver solo los correos electrónicos relevantes. En este ejemplo, solo hemos añadido un filtro Asunto y dejado los otros 2 en blanco.

   >[!NOTE]
   >
   >Añadiremos un enrutador para buscar frases en un correo electrónico usando el iterador [!UICONTROL Coincidir con el patrón] y una expresión regular (Regex) como patrón de búsqueda. Esto también nos permite crear un escenario de varias utilidades.

1. Cuando se complete la configuración y se le indique que especifique dónde comenzar a ver sus mensajes de correo electrónico, haga clic en **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Continúe con [Buscar [!UICONTROL Control de flujo] y añada un [!UICONTROL enrutador]](#search-for-flow-control-and-add-a-router)

## Busque [!UICONTROL Control de flujo] y añada un [!UICONTROL enrutador]

1. Añada un enrutador después de cualquier módulo para dividir o duplicar los datos antes de enviarlos al siguiente módulo.

   En este caso, hemos usado un [!UICONTROL enrutador] para enviar el texto del cuerpo del mensaje de correo electrónico a 2 tablas independientes en una [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## Usar el módulo [!UICONTROL Analizador de texto]

1. Añada el transformador [!UICONTROL Coincidir con el patrón] para buscar una frase en un mensaje de correo electrónico.

   Buscaremos la frase “[!UICONTROL módulo de analizador de texto]” en todos los correos electrónicos entrantes para capturar el texto del cuerpo y el nombre del remitente de los que coinciden con esa frase.

   1. Escriba el patrón como una expresión regular:

      text\sparser\smodule

   1. (Opcional) Utilice cualquiera de las otras opciones del patrón.

      ![](assets/pattern-350x318.png)

      Multilínea es útil si el texto contiene varias líneas y necesita buscar el patrón en cada línea. Para este tutorial necesitamos buscar el patrón en todo el texto del cuerpo del correo electrónico, por lo tanto, lo dejaremos sin marcar.

   1. En el campo [!UICONTROL Texto], haga clic en el atributo **Contenido de texto** de la lista.

      ![](assets/text-content-350x264.png)

      Este es el atributo que almacena el texto del cuerpo del correo electrónico en el que buscaremos el patrón.

1. Añada otro [!UICONTROL Patrón de coincidencia] que busque la misma frase y una dirección de correo electrónico.

   Esto resulta especialmente útil si tiene cuentas de cliente con varios usuarios. Para ahorrar tiempo, puede clonar el módulo del [!UICONTROL Analizador de texto] que acaba de crear y vincularlo al enrutador.

   ![](assets/clone.png)

1. Edite el patrón de la siguiente manera:

   text\sparser\smodule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Este patrón busca la frase “[!UICONTROL módulo de analizador de texto]” y una dirección de correo electrónico como john.doe@gmail.com y solo devuelve la dirección de correo electrónico.

   >[!NOTE]
   >
   >Es importante escribir su Regex de acuerdo con la especificación de las direcciones de correo electrónico que acepta, pero la anterior se encarga de la mayoría de las direcciones de correo electrónico estándar.

   * Si desea buscar solo direcciones de correo electrónico, puede utilizar Regex que se indica a continuación:

     ([\w.-]+@[\w.-]+)

   * También puede buscar solo números de teléfono usando Regex que se indica a continuación:

     ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}
El patrón anterior cubre los formatos más comunes en los que se escribe un número de teléfono.

   Para probar sus patrones, recomendamos usar [[!DNL https://regex101.com]](https://regex101.com/) con [!DNL javascript] como opción.

   El resto de la configuración permanece igual que la anterior.

## Añadir los módulos [!DNL Google Sheets]

Para [!DNL Sheets], primero debemos crear una hoja de cálculo con los encabezados necesarios.

1. Cree una hoja de cálculo con las columnas en las que desee capturar los datos del usuario. (No dude en utilizar también un archivo existente).

   Por ejemplo, cree uno llamado “Datos de correo electrónico: ticket de asistencia” con el nombre del remitente, el correo electrónico del remitente y el contenido del correo electrónico como columnas. Asigne el nombre “contiene: módulo de analizador de texto” a la hoja de cálculo.

1. Añada el módulo [!UICONTROL Hojas de cálculo de Google] con **[!UICONTROL Añadir una fila]** como acción.

   ![](assets/add-a-row-350x174.png)

1. Conecte su cuenta de [!DNL Google] (si aún no lo ha hecho). Elija el archivo ya creado anteriormente, seguido de la hoja de cálculo de la que está capturando los datos.

   Su configuración debería tener este aspecto:

   ![](assets/connect-google-acct-350x279.png)

1. Asigne los atributos en los campos relevantes (columnas) para finalizar la configuración del módulo.

   ![](assets/map-attributes-350x282.png)

1. Clone el módulo que acaba de crear y vincúlelo al segundo módulo del [!UICONTROL Analizador de texto].

   1. Vaya a la hoja de cálculo, duplique la hoja de cálculo que creó anteriormente y asígnele un nombre.

      Por ejemplo, asígnele el nombre “contiene: módulo de analizador de texto y correo electrónico”.

   1. Añada otra columna para almacenar la dirección de correo electrónico que contiene el cuerpo del correo electrónico.

      Por ejemplo, asígnele el nombre “Dirección de correo electrónico compartida”.

   1. Haga clic en el módulo de [!DNL Google Sheets] clonado para configurar los ajustes.
   1. Cambie la hoja de cálculo por la nueva que acaba de crear.
   1. Asigne el resultado del módulo [!UICONTROL Patrón de coincidencia] ($1) a la columna donde desea almacenar la dirección de correo electrónico (Dirección de correo electrónico compartida).

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Haga clic en **[!UICONTROL Aceptar]**, guarde el escenario y realice una ejecución de prueba.

      Deberá enviar dos correos electrónicos independientes a la dirección de correo electrónico conectada de la siguiente manera:

      * Que contenga la frase “[!UICONTROL módulo analizador de texto]” (y ninguna dirección de correo electrónico)

        ![](assets/text-parser-module-350x103.png)

      * Que contenga la frase anterior y una dirección de correo electrónico

        ![](assets/above-phrase-and-email-350x106.png)

        Si no hay errores en la configuración, verá que la primera hoja de cálculo captura todos los mensajes de correo electrónico que contengan la frase “[!UICONTROL módulo de analizador de texto]”, mientras que la segunda hoja de cálculo captura únicamente los que contienen la frase “[!UICONTROL módulo de analizador de texto]” y una dirección de correo electrónico. Puede consultar las capturas de pantalla siguientes.

        Hoja de trabajo 1:

        ![](assets/worksheet-1-350x57.png)

        Hoja de trabajo 2:

        ![](assets/worksheet-2-350x41.png)

## Recursos

* [Ejercicios gratuitos](https://regexone.com/) para obtener información sobre las expresiones regulares
* [Obtener información sobre la coincidencia de número de teléfono](https://regexone.com/problem/matching_phone_numbers) con Regex
* [Información sobre la coincidencia de correo electrónico](https://regexone.com/problem/matching_emails) con Regex
* [Probar las expresiones regulares](https://regex101.com/)
