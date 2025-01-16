---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Herramientas
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 97a68fbc-1272-43fc-b4f2-4c1c9e590741
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2344'
ht-degree: 95%

---

# [!UICONTROL Herramientas]

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Herramientas](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/tools-modules.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

La sección [!DNL Adobe Workfront Fusion Tools] incluye varios módulos útiles que pueden mejorar su escenario.

Los módulos de [!UICONTROL Herramientas] están disponibles en la lista de aplicaciones o en el icono de [!UICONTROL Herramientas] ![](assets/tools-icon-small.png) en la parte inferior de la pantalla.

## Requisitos de acceso

Para utilizar la funcionalidad de este artículo debe tener el siguiente acceso:

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
   <td>
   <p>Requisito de licencia actual: no se requiere ninguna licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Producto</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront].

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte Licencias de [[!DNL Adobe Workfront Fusion] ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Herramientas] y sus campos

* [Activadores](#triggers)
* [Acciones](#actions)
* [Agregadores](#aggregators)
* [Transformadores](#transformers)

### Activadores

#### [!UICONTROL Activador básico]

Este módulo le permite crear un activador personalizado y definir sus paquetes de entrada.

Puede usar este módulo, por ejemplo, para contactos o cualquier otra lista programada para enviarse a una dirección de correo electrónico especificada (como los módulos [!UICONTROL Correo electrónico] >[!UICONTROL Enviar un correo electrónico] o [!DNL Gmail] >[!UICONTROL Enviar un correo electrónico]), o como un simple recordatorio que se activará cuando quiera.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bundle]</td> 
   <td> <p>Cree paquetes personalizados añadiendo elementos de matriz. La matriz consta de pares nombre-valor.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Acciones

* [[!UICONTROL Obtener múltiples variables]](#get-multiple-variables)
* [[!UICONTROL Obtener variable]](#get-variable)
* [[!UICONTROL Función de incremento]](#increment-function)
* [[!UICONTROL Establecer varias variables]](#set-multiple-variables)
* [[!UICONTROL Establecer variable]](#set-variable)
* [[!UICONTROL Suspensión]](#sleep)

#### [!UICONTROL Obtener múltiples variables]

Este módulo recupera valores creados anteriormente por el módulo [!UICONTROL Establecer variable] o [!UICONTROL Establecer múltiples variables].

Este módulo puede leer variables que se establecieron en cualquier parte del escenario, incluso si la variable se estableció en una ruta diferente a la ubicación del módulo [!UICONTROL Obtener múltiples variables]. El único requisito es que el módulo [!UICONTROL Herramientas] > [!UICONTROL Establecer variable] o [!UICONTROL Herramientas] > [!UICONTROL Establecer múltiples variables] se ejecute antes que el módulo [!UICONTROL Herramientas] > [!UICONTROL Obtener múltiples variables].  Para obtener más información sobre el orden en que se ejecutan los módulos, consulte [Módulo de enrutador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Variables]</td>
        <td>Añada las variables que desea que obtenga el módulo.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Variable name]</td>
        <td>Para cada variable que añada, asigne el nombre de la variable que desee obtener.</td>
    </tr>
</table>

>[!INFO]
>
>**Ejemplos:** los siguientes son posibles usos de los módulos [!UICONTROL Establecer]/[!UICONTROL Obtener (múltiples) variables]:
>
>* Para almacenar un valor calculado para su uso posterior, incluso en una ruta diferente. Esto resulta útil en casos en los que el valor se utiliza en varios módulos y la fórmula para calcularlo es demasiado compleja.
>* Para depurar una fórmula. Si una fórmula utilizada en un módulo no proporciona aparentemente un resultado correcto, copie la fórmula y péguela en un módulo [!UICONTROL Establecer variable] que inserte antes del módulo correspondiente. Desconecte los módulos después del módulo [!UICONTROL Establecer variable] y ejecute el escenario. Compruebe el resultado del módulo [!UICONTROL Establecer variable], ajuste o simplifique la fórmula, ejecute de nuevo el escenario y continúe haciéndolo hasta que se haya resuelto el problema.


#### [!UICONTROL Obtener variable]

Este módulo recupera un valor creado anteriormente por el módulo [!UICONTROL Establecer variable] o [!UICONTROL Establecer múltiples variables].

Este módulo puede leer variables que se establecieron en cualquier parte del escenario, incluso si la variable se estableció en una ruta diferente a donde se encuentra el módulo [!UICONTROL Obtener variable]. El único requisito es que el módulo [!UICONTROL Herramientas] > [!UICONTROL Establecer variable] o [!UICONTROL Herramientas] > [!UICONTROL Establecer múltiples variables] se ejecute antes que el módulo [!UICONTROL Herramientas] > [!UICONTROL Obtener variable].  Para obtener más información sobre el orden en que se ejecutan los módulos, consulte [Módulo de enrutador en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/router-module.md).

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
   <td role="rowheader">[!UICONTROL Reset a value]</td> 
   <td> <p>Seleccione cuando desee que el módulo incremente el valor. </p> 
    <ul> 
     <li>[!UICONTROL After one cycle]</li> 
     <li>[!UICONTROL After one scenario run]</li> 
     <li>[!UICONTROL Never]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:**
>
>Uno de los usos del módulo es implementar una asignación “rotativa” de tareas, posibles clientes, correos electrónicos, etc., a los usuarios de un grupo. El algoritmo elige a los usuarios asignados de un grupo en un orden racional, que generalmente va de la parte superior a la parte inferior de una lista. Cuando el algoritmo llega al final de la lista, le asigna la siguiente asignación al usuario en la parte superior de la lista y continúa realizando asignaciones en la lista.
>
>El siguiente escenario envía un correo electrónico al primer destinatario después de ejecutar cada escenario impar y al segundo destinatario después de ejecutar cada escenario par.
>
>![](assets/example-email-350x246.gif)
>
>1. Para crear este escenario, haga lo siguiente:
>1. Establezca el campo **[!UICONTROL Restablecer un valor]** del módulo en Nunca.
>1. Defina la ruta para los valores impares. Establezca el filtro para esta ruta mediante la función de coincidencia de módulo igual a `1`:
>
>   ![](assets/odd-350x459.png)
>
>  **Nota**: no olvide cambiar el operador [!UICONTROL Igual a] del operador [!UICONTROL Texto] predeterminado al operador [!UICONTROL Numérico].
>
>1. Establezca la ruta para los valores pares utilizando la función de coincidencia de módulo igual a `0`:
>
>La función de incremento añade uno cada vez que se ejecuta el escenario. Los filtros comprueban el incremento y actúan en su valor, lo que garantiza que los correos electrónicos se distribuyan de manera uniforme.

#### [!UICONTROL Establecer múltiples variables]

Este módulo crea variables que otros módulos pueden asignar en la ruta. La variable también se puede asignar a los módulos [!UICONTROL Obtener variable] u [!UICONTROL Obtener varias variables] para cualquier ruta del escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variables]</td> 
   <td>Añada las variables que desea que establezca el módulo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Para cada variable, introduzca su nombre. Este nombre se muestra al asignar la variable en otros módulos. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>Para cada variable, introduzca el valor de la variable. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable lifetime] </td> 
   <td> <p>Seleccione el tiempo que desea que las variables sigan siendo válidas (mantengan el mismo valor).</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>: la variable es válida durante un ciclo. Resulta útil cuando se reciben varios webhooks en una ejecución de escenario (más webhooks = más ciclos). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: la variable es válida para una ejecución de escenario. Una ejecución puede contener uno o más ciclos.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Establecer variable]

Este módulo crea una variable que otros módulos pueden asignar en la ruta. La variable también se puede asignar a los módulos [!UICONTROL Obtener variable] u [!UICONTROL Obtener varias variables] para cualquier ruta del escenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Variable name] </td> 
   <td>Introduzca el nombre de la variable. Este nombre se muestra al asignar la variable en otros módulos. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable lifetime] </td> 
   <td> <p>Seleccione el tiempo que desea que las variables sigan siendo válidas (mantengan el mismo valor).</p> 
    <ul> 
     <li><strong>[!UICONTROL One cycle]</strong>: la variable es válida durante un ciclo. Resulta útil cuando se reciben varios webhooks en una ejecución de escenario (más webhooks = más ciclos). </li> 
     <li><strong>[!UICONTROL One execution]</strong>: la variable es válida para una ejecución de escenario. Una ejecución puede contener uno o más ciclos.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Variable value] </td> 
   <td>Introduzca o asigne el valor de la variable. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suspensión]

Este módulo le permite retrasar el flujo del escenario hasta 300 segundos (5 minutos).

Esta función puede resultar útil, por ejemplo, si desea reducir la carga del servidor de servicio de [!DNL target] o para imitar el comportamiento humano al enviar SMS o correos electrónicos masivos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Delay]</p> </td> 
   <td> <p>Introduzca el número de segundos durante los que se detendrá el escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Si desea pausar el flujo durante períodos de tiempo más largos, es recomendable dividir el escenario en dos escenarios:
>
>* El primer escenario contendría la parte antes de la pausa.
>* El segundo escenario contendría la parte posterior.
>
>El primer escenario acabaría almacenando toda la información necesaria en un almacén de datos junto con la marca de tiempo actual. El segundo escenario comprobaría periódicamente si hay registros con una marca de tiempo anterior al retraso previsto en el almacén de datos, recuperaría los registros, finalizaría el procesamiento de los datos y eliminaría los registros del almacén de datos.
>
>Para obtener más información sobre los almacenes de datos, consulte [Almacenes de datos en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md).
>
>Para obtener más información sobre módulos de almacenes de datos específicos, consulte [[!UICONTROL Módulos de almacenes de datos]](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

### Agregadores

* [[!UICONTROL Agregador numérico]](#numeric-aggregator)
* [[!UICONTROL Agregador de tablas]](#table-aggregator)
* [[!UICONTROL Agregador de texto]](#text-aggregator)

#### [!UICONTROL Agregador numérico]

Este módulo le permite recuperar valores numéricos y, a continuación, aplicar una de las funciones seleccionadas (SUM, AVG, COUNT, MAX, MIN) y devolver el resultado en un paquete.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Seleccione el módulo desde el que desea agregar los campos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Aggregate function]</p> </td> 
   <td> <p>Seleccione la función que desee utilizar para agregar los valores.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Defina una expresión por la cual desea agrupar la salida agregada. Esta expresión puede contener uno o varios elementos asignados. Los datos añadidos se separan en grupos utilizando el valor de esta expresión. Cada grupo genera como un paquete independiente con una clave (la expresión evaluada) y un valor (el valor agregado). Puede utilizar la clave como filtro en módulos posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Active esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Value]</p> </td> 
   <td> <p>Introduzca o asigne el valor que desea agregar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregador de tablas]

Este módulo combina los valores de los campos seleccionados de los paquetes recibidos en un solo paquete utilizando un separador de columnas y filas especificado (que le permite crear una tabla).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Seleccione el módulo desde el que desea agregar los campos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aggregated fields]</td> 
   <td> <p> Seleccione los campos del módulo seleccionado anteriormente que contienen los valores que desea agregar al paquete.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Column separator]</p> </td> 
   <td> <p>Seleccione o introduzca el tipo de separador que separará las columnas de valor de campo en el paquete resultante. Si selecciona [!UICONTROL Other], introduzca el carácter que desea utilizar para separar valores en el campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Row separator]</p> </td> 
   <td> <p>Seleccione o introduzca el tipo de separador que separará las filas de valor de campo en el paquete resultante. Si selecciona [!UICONTROL Other], introduzca el carácter que desea utilizar para separar valores en el campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Defina una expresión por la cual desea agrupar la salida agregada. Esta expresión puede contener uno o varios elementos asignados. Los datos agregados se separarán entonces en grupos utilizando el valor de esta expresión. Cada grupo genera como un paquete independiente con una clave (la expresión evaluada) y un valor (el valor agregado). Puede utilizar la clave como filtro en módulos posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Seleccione esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Agregador de texto]

Este módulo combina los valores de los campos seleccionados de los paquetes recibidos en un solo paquete.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Source module]</p> </td> 
   <td> <p>Seleccione el módulo desde el que desea agregar los campos.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Row separator]</p> </td> 
   <td> <p>Seleccione o introduzca el tipo de separador que separará las filas de valor de campo en el paquete resultante. Si selecciona [!UICONTROL Other], introduzca el carácter que desea utilizar para separar valores en el campo separador.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Group by]</p> </td> 
   <td> <p>Defina una expresión que contenga uno o varios elementos asignados. Los datos agregados se separan en Grupos con el mismo valor de expresión. Cada grupo genera como un paquete independiente que contiene una clave con la expresión evaluada y el texto agregado. Al hacerlo, puede utilizar la clave como filtro en módulos posteriores.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Text]</td> 
   <td> <p> Introduzca o asigne el texto que desea que agregue el módulo.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Seleccione esta opción para detener el escenario cuando no haya resultados.</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Ejemplo:** puede usar el agregador de texto para insertar más valores (por ejemplo, nombres de clientes o notas) en un solo paquete y enviar un correo electrónico que contenga todos los valores del cuerpo del correo electrónico o del asunto del correo electrónico.

### Transformadores

* [[!UICONTROL Escribir una cadena]](#compose-a-string)
* [[!UICONTROL Convertir la codificación del texto]](#convert-the-encoding-of-the-text)
* [[!UICONTROL Conmutador]](#switch)

#### [!UICONTROL Escribir una cadena]

Convierte cualquier valor en un tipo de datos de cadena (texto). Facilita la asignación al asignar, por ejemplo, datos binarios.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p>Introduzca o asigne los datos que desea convertir en texto.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertir la codificación del texto]

Convierte el texto de entrada (o los datos binarios) a la codificación seleccionada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input data]</p> </td> 
   <td> <p>Introduzca o asigne el contenido que desea convertir.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Input data codepage]</td> 
   <td> <p>Seleccione el tipo de codificación de los datos de entrada. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Output data codepage]</p> </td> 
   <td> <p>Seleccione el tipo de codificación de los datos de destino (salida).</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Conmutador]

Comprueba si el valor de entrada coincide con la lista de valores proporcionada. Devuelve la salida en función del resultado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!UICONTROL Input]</p> </td> 
   <td> <p>Introduzca la expresión que desea evaluar.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Use regular expressions to match]</td> 
   <td> <p>Active esta opción para utilizar expresiones regulares. El módulo determina los casos en función de la expresión regular, en lugar de una coincidencia exacta.</p> 
    <div> 
     <p>Una expresión regular es una secuencia de caracteres en la que cada carácter es un metacarácter, que tiene un significado especial, o un carácter regular que tiene un significado literal. Estos caracteres y metacaracteres identifican un patrón que se puede utilizar para buscar texto. Por ejemplo, si desea buscar nombres, puede configurar una expresión regular para buscar un patrón que consista en dos palabras consecutivas que comiencen con mayúsculas. Las expresiones regulares son una potente herramienta para buscar y manipular texto.</p> 
     <p>El análisis de las expresiones regulares excede el ámbito de este artículo. Recomendamos los siguientes recursos:</p> 
     <ul> 
      <li>Para obtener la lista completa de metacaracteres, consulte <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions">Expresiones regulares</a> en los documentos web de MDN.</li> 
      <li>Para ver un tutorial sobre cómo crear expresiones regulares, recomendamos <a href="https://regexone.com/">RegexOne</a>.</li> 
      <li>Para experimentar con expresiones regulares, recomendamos el sitio web <a href="https://regex101.com/">Expresiones regulares 101</a>. Seleccione ECMAScript (JavaScript) FLAVOR en el panel izquierdo.</li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Cases] </td> 
   <td> <p>Si la entrada contiene un valor introducido en el campo [!UICONTROL Pattern], se devuelve el valor introducido en el campo [!UICONTROL Output].</p> <p>Si la entrada no coincide con ninguno de los valores establecidos en un campo de [!UICONTROL Pattern], se produce una de las siguientes situaciones:</p> 
    <ul> 
     <li>Se devuelve el valor del campo [!UICONTROL Else]</li> 
     <li>Si no hay ningún valor en el campo [!UICONTROL Else], no se devuelve ningún resultado.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Else]</p> </td> 
   <td> <p>Introduzca el valor que se devuelve cuando no se cumplen los criterios establecidos en el campo Casos. </p> </td> 
  </tr> 
 </tbody> 
</table>
