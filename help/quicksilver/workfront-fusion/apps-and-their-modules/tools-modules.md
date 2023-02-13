---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Herramientas
description: La variable [!DNL Adobe Workfront Fusion Tools] incluye varios módulos útiles que pueden mejorar el escenario.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2246'
ht-degree: 0%

---

# [!UICONTROL Herramientas]

La variable [!DNL Adobe Workfront Fusion Tools] incluye varios módulos útiles que pueden mejorar el escenario.

[!UICONTROL Herramientas] Los módulos están disponibles en la lista de aplicaciones o en el [!UICONTROL Herramientas] icono ![](assets/tools-icon-small.png) en la parte inferior de la pantalla.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr>
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Herramientas] y sus campos

* [Déclencheur](#triggers)
* [Acciones](#actions)
* [Acumuladores](#aggregators)
* [Transformadores](#transformers)

### Déclencheur

#### [!UICONTROL Déclencheur básico]

Este módulo le permite crear un déclencheur personalizado y definir sus paquetes de entrada.

Puede utilizar este módulo, por ejemplo, para contactos o cualquier otra lista programada para enviarse a una dirección de correo electrónico especificada (como [!UICONTROL Correo electrónico] >[!UICONTROL Enviar un correo electrónico]o [!DNL Gmail] >[!UICONTROL Enviar un correo electrónico] ), o como un simple recordatorio para que se active cuando lo desee.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>Cree paquetes personalizados añadiendo elementos de matriz. La matriz consta de los pares nombre-valor.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Obtener varias variables]](#get-multiple-variables)
* [[!UICONTROL Obtener variable]](#get-variable)
* [[!UICONTROL Función de incremento]](#increment-function)
* [[!UICONTROL Establecer varias variables]](#set-multiple-variables)
* [[!UICONTROL Establecer variable]](#set-variable)
* [[!UICONTROL Sueño]](#sleep)

#### [!UICONTROL Obtener varias variables]

Este módulo recupera los valores creados anteriormente por el [!UICONTROL Establecer variable] o [!UICONTROL Establecer varias variables] módulo.

Este módulo puede leer variables que se configuraron en cualquier lugar del escenario, incluso si la variable se configuró en una ruta diferente a la del escenario [!UICONTROL Obtener varias variables] está ubicado. El único requisito es que la variable [!UICONTROL Herramientas] > [!UICONTROL Establecer variable] o [!UICONTROL Herramientas] > [!UICONTROL Definir varias variables] se ejecuta antes de que [!UICONTROL Herramientas] > [!UICONTROL Obtener varias variables] módulo. Para obtener más información sobre el orden en que se ejecutan los módulos, consulte [Módulo Router en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>Añada las variables que desee que obtenga el módulo.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Variable name]</td>
        <td>Para cada variable que agregue, asigne el nombre de la variable que desee obtener.</td>
    </tr>
</table>

>[!INFO]
>
>**Ejemplos:**  Los siguientes son posibles usos del [!UICONTROL Establezca]/[!UICONTROL Obtener variables (múltiples)] módulos:
>
>* Para almacenar un valor calculado para su uso posterior, incluso en una ruta diferente. Esto resulta útil en casos en los que el valor se utiliza en varios módulos y la fórmula para calcular el valor es demasiado compleja.
>* Para depurar una fórmula. Si una fórmula utilizada en un módulo no parece proporcionar un resultado correcto, copie la fórmula y péguela en una [!UICONTROL Establecer variable] que inserte antes del módulo correspondiente. Desconecte los módulos después del [!UICONTROL Establecer variable] y ejecute el escenario. Compruebe el [!UICONTROL Establecer variable] salida del módulo, ajuste o simplifique la fórmula, ejecute de nuevo el escenario y continúe haciéndolo hasta que se haya resuelto el problema.



#### [!UICONTROL Obtener variable]

Este módulo recupera un valor que el [!UICONTROL Establecer variable] o [!UICONTROL Establecer varias variables] módulo.

Este módulo puede leer variables que se configuraron en cualquier lugar del escenario, incluso si la variable se configuró en una ruta diferente a la del escenario [!UICONTROL Obtener variable] está ubicado. El único requisito es que la variable [!UICONTROL Herramientas] > [!UICONTROL Establecer variable] o [!UICONTROL Herramientas] > [!UICONTROL Establecer varias variables] se ejecuta antes de que [!UICONTROL Herramientas] > [!UICONTROL Obtener variable] módulo. Para obtener más información sobre el orden en que se ejecutan los módulos, consulte [Módulo Router en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable name]</td> 
   <td> <p>Asigne el nombre de la variable que desea que obtenga el módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Función de incremento]

Este módulo devuelve un valor incrementado en 1 después de la operación de cada módulo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Restablecer un valor]</td> 
   <td> <p>Seleccione cuándo desea que el módulo incremente el valor. </p> 
    <ul> 
     <li>[!UICONTROL Después de un ciclo]</li> 
     <li>[!UICONTROL Después de ejecutar un escenario]</li> 
     <li>[!UICONTROL Nunca]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:**
>
>Uno de los usos del módulo es implementar una asignación &quot;de ida y vuelta&quot; de tareas, posibles clientes, correos electrónicos, etc., a los usuarios de un grupo. El algoritmo elige a los asignados de un grupo en un orden racional, que normalmente va de arriba a abajo en la lista. Cuando el algoritmo llega al final de la lista, entonces asignaría la siguiente asignación al usuario situado en la parte superior de la lista y seguiría asignando asignaciones en la lista.
>
>El siguiente escenario envía un correo electrónico al primer destinatario después de que se ejecute cada escenario impar y al segundo destinatario después de que se ejecute cada escenario par.
>
>![](assets/example-email-350x246.gif)
>
>1. Para crear este escenario:
>1. Configure el **[!UICONTROL Restablecer un valor]** a Nunca.
>1. Establezca la ruta para los valores impares. Establezca el filtro para esta ruta utilizando la función matemática del módulo igual a `1`:

>
>   ![](assets/odd-350x459.png)
>
>  **Nota**: No olvide cambiar el [!UICONTROL Igual a] del operador predeterminado [!UICONTROL Texto] al [!UICONTROL Numérico] operador.
>
>1. Establezca la ruta para valores pares utilizando la función matemática del módulo igual a `0`:
>
>La función increment agrega una cada vez que se ejecuta el escenario. Los filtros comprueban el incremento y actúan sobre su valor, asegurándose de que los correos electrónicos se distribuyen de manera uniforme.

#### [!UICONTROL Establecer varias variables]

Este módulo crea variables que pueden asignarse a otros módulos de la ruta. La variable también se puede asignar a la variable [!UICONTROL Obtener variable] o [!UICONTROL Obtener varias variables] módulos para cualquier ruta en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>Añada las variables que desee que establezca el módulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Para cada variable, introduzca el nombre de la variable. Este nombre se muestra al asignar la variable en otros módulos. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>Para cada variable, introduzca el valor de la variable . </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duración de la variable] </td> 
   <td> <p>Seleccione cuánto tiempo desea que las variables permanezcan válidas (mantenga el mismo valor).</p> 
    <ul> 
     <li><strong>[!UICONTROL Un ciclo]</strong>: La variable es válida para un ciclo. Útil cuando se reciben varios vínculos web en una ejecución de escenario (más vínculos web = más ciclos). </li> 
     <li><strong>[!UICONTROL Una ejecución]</strong>: La variable es válida para una ejecución de escenario. Una ejecución puede contener uno o más ciclos.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Establecer variable]

Este módulo crea una variable que puede asignarse a otros módulos de la ruta. La variable también se puede asignar a la variable [!UICONTROL Obtener variable] o [!UICONTROL Obtener varias variables] módulos para cualquier ruta en el escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Introduzca el nombre de la variable. Este nombre se muestra al asignar la variable en otros módulos. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Duración de la variable] </td> 
   <td> <p>Seleccione cuánto tiempo desea que las variables permanezcan válidas (mantenga el mismo valor).</p> 
    <ul> 
     <li><strong>[!UICONTROL Un ciclo]</strong>: La variable es válida para un ciclo. Útil cuando se reciben varios vínculos web en una ejecución de escenario (más vínculos web = más ciclos). </li> 
     <li><strong>[!UICONTROL Una ejecución]</strong>: La variable es válida para una ejecución de escenario. Una ejecución puede contener uno o más ciclos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>Introduzca o asigne el valor de la variable. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Sueño]

Este módulo le permite retrasar el flujo del escenario hasta 300 segundos (5 minutos).

Esta función puede resultar útil, por ejemplo, si desea reducir la variable [!DNL target] carga del servidor de servicio o para imitar el comportamiento humano al enviar SMS o correos electrónicos masivos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Retraso]</p> </td> 
   <td> <p>Introduzca el número de segundos que se pausará el escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Si desea pausar el flujo durante períodos de tiempo más largos, sugerimos dividir el escenario en dos escenarios:
>
>* El primer escenario contendría la parte antes de la pausa.
>* La segunda hipótesis contendría la parte que sigue.
>
>El primer escenario terminaría almacenando toda la información necesaria en un almacén de datos junto con la marca de tiempo actual. En el segundo escenario se comprobaría periódicamente si el almacén de datos tenía registros con una marca de tiempo anterior a la demora prevista, se recuperarían los registros, se finalizaría el procesamiento de los datos y se eliminarían los registros del almacén de datos.
>
>Para obtener más información sobre los almacenes de datos, consulte [Almacenes de datos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>Para obtener más información sobre módulos de almacenamiento de datos específicos, consulte [[!UICONTROL Almacén de datos] módulos](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Acumuladores

* [[!UICONTROL Acumulador numérico]](#numeric-aggregator)
* [[!UICONTROL Acumulador de tablas]](#table-aggregator)
* [[!UICONTROL Acumulador de texto]](#text-aggregator)

#### [!UICONTROL Acumulador numérico]

Este módulo le permite recuperar valores numéricos, luego aplicar una de las funciones seleccionadas (SUM, AVG, COUNT, MAX, MIN) y devolver el resultado en un paquete.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Seleccione el módulo desde el que desea acumular campos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Aggregate function]</p> </td> 
   <td> <p>Seleccione la función que desee utilizar para acumular los valores.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Defina una expresión por la que desee agrupar la salida agregada. Esta expresión puede contener uno o más elementos asignados. Los datos agregados se separan en grupos utilizando el valor de esta expresión. Cada grupo genera un paquete independiente con una clave (la expresión evaluada) y un valor (el valor agregado). Puede utilizar la clave como filtro en los módulos siguientes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detenga el procesamiento después de una agregación vacía]</td> 
   <td>Active esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Valor]</p> </td> 
   <td> <p>Introduzca o asigne el valor que desea acumular.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Acumulador de tablas]

Este módulo combina los valores de los campos seleccionados de los paquetes recibidos en un solo paquete utilizando un separador de columnas y filas especificado (que le permite crear una tabla).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Seleccione el módulo desde el que desea acumular campos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Campos agregados]</td> 
   <td> <p> Seleccione los campos del módulo seleccionado arriba que contienen valores que desea agregar en el paquete único.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separador de columnas]</p> </td> 
   <td> <p>Seleccione o introduzca el tipo de separador que separará las columnas del valor del campo en el paquete resultante. Si selecciona [!UICONTROL Otros], introduzca el carácter que desea utilizar para separar valores en el campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separador de filas]</p> </td> 
   <td> <p>Seleccione o introduzca el tipo de separador que separará las filas de valor de campo en el paquete resultante. Si selecciona [!UICONTROL Otros], introduzca el carácter que desea utilizar para separar valores en el campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Defina una expresión por la que desee agrupar la salida agregada. Esta expresión puede contener uno o más elementos asignados. Los datos agregados se separan en grupos utilizando el valor de esta expresión. Cada grupo genera un paquete independiente con una clave (la expresión evaluada) y un valor (el valor agregado). Puede utilizar la clave como filtro en los módulos siguientes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detenga el procesamiento después de una agregación vacía]</td> 
   <td>Seleccione esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Acumulador de texto]

Este módulo combina los valores de los campos seleccionados de los paquetes recibidos en un solo paquete.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Seleccione el módulo desde el que desea acumular campos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Separador de filas]</p> </td> 
   <td> <p>Seleccione o introduzca el tipo de separador que separará las filas de valor de campo en el paquete resultante. Si selecciona [!UICONTROL Otros], introduzca el carácter que desea utilizar para separar valores en el campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Defina una expresión que contenga uno o más elementos asignados. Los datos agregados se separan en Grupos con el mismo valor de expresión. Cada grupo genera como un paquete separado que contiene una clave con la expresión evaluada y el texto agregado. Al hacerlo, puede utilizar la clave como filtro en los módulos siguientes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Texto]</td> 
   <td> <p> Introduzca o asigne el texto que desea que agregue el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Detenga el procesamiento después de una agregación vacía]</td> 
   <td>Seleccione esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** Puede utilizar el agregador de texto para insertar más valores (por ejemplo, nombres de clientes o notas) en un solo paquete y enviar un correo electrónico que contenga todos los valores del cuerpo del correo electrónico o del asunto del correo electrónico.

### Transformadores

* [[!UICONTROL Componer una cadena]](#compose-a-string)
* [[!UICONTROL Convertir la codificación del texto]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Conmutador]](#switch)

#### [!UICONTROL Componer una cadena]

Convierte cualquier valor en un tipo de datos de cadena (texto). Facilita la asignación al asignar, por ejemplo, datos binarios.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Texto]</td> 
   <td> <p>Introduzca o asigne los datos que desea convertir en texto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertir la codificación del texto]

Convierte el texto de entrada introducido (o los datos binarios) en la codificación seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Datos de entrada]</p> </td> 
   <td> <p>Introduzca o asigne el contenido que desea convertir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Página de códigos de datos de entrada]</td> 
   <td> <p>Seleccione el tipo de codificación de los datos de entrada. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Página de códigos de datos de salida]</p> </td> 
   <td> <p>Seleccione el tipo de codificación de los datos de destino (salida).</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Conmutador]

Comprueba que el valor de entrada coincida con la lista de valores proporcionada. Devuelve el resultado en función del resultado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Entrada]</p> </td> 
   <td> <p>Introduzca la expresión que desea evaluar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Utilizar expresiones regulares para coincidir]</td> 
   <td> <p>Active esta opción para utilizar expresiones regulares. El módulo determina los casos en función de la expresión regular, en lugar de una coincidencia exacta.</p> 
    <div> 
     <p>Una expresión regular es una secuencia de caracteres en la que cada carácter es un metacaractero, tiene un significado especial, o un carácter normal que tiene un significado literal. Estos caracteres y metacaracteres identifican un patrón que se puede usar para buscar texto. Por ejemplo, si desea buscar nombres, puede configurar una expresión regular para buscar un patrón que consista en dos palabras consecutivas que empiecen por mayúsculas. Las expresiones regulares son una potente herramienta para buscar y manipular texto.</p> 
     <p>El debate sobre las expresiones regulares está fuera del alcance de este artículo. Recomendamos los siguientes recursos:</p> 
     <ul> 
      <li>La lista completa de metacaracteres puede consultarse en <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Expresiones regulares</a> en documentos web de MDN.</li> 
      <li>Para ver un tutorial sobre cómo crear expresiones regulares, se recomienda <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>Para experimentar con expresiones regulares, se recomienda usar la variable <a href="https://regex101.com/">Expresiones regulares 101</a> sitio web. Seleccione el FLAVOR de ECMAScript (JavaScript) en el panel izquierdo.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cases] </td> 
   <td> <p>Si la entrada contiene un valor introducido en el campo [!UICONTROL Pattern], se devuelve el valor introducido en el campo [!UICONTROL Output].</p> <p>Si la entrada no coincide con ninguno de los valores establecidos en un campo [!UICONTROL Pattern], se produce una de las siguientes:</p> 
    <ul> 
     <li>Se devuelve el valor del campo [!UICONTROL Else]</li> 
     <li>Si no hay ningún valor en el campo [!UICONTROL Else], no se devuelve ningún resultado.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Introduzca el valor que se devuelve cuando no se cumplen los criterios establecidos en el campo Cases . </p> </td> 
  </tr> 
 </tbody> 
</table>
