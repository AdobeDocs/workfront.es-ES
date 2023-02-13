---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creación de un escenario de integración de prácticas en Adobe Workfront Fusion
description: Este artículo describe cómo crear un escenario de integración con Adobe Workfront Fusion. Los escenarios de integración conectan aplicaciones independientes, lo que permite que los datos fluyan a través de distintas aplicaciones.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '2076'
ht-degree: 0%

---

# Creación de un escenario de integración de prácticas en Adobe Workfront Fusion

Este artículo describe cómo crear un escenario de integración con Adobe Workfront Fusion. Los escenarios de integración conectan aplicaciones independientes, lo que permite que los datos fluyan a través de distintas aplicaciones.

Para crear un escenario de integración, su organización debe tener un [!DNL Workfront Fusion for Work Automation and Integration] licencia.

Para obtener instrucciones sobre cómo crear un escenario de automatización solo para Workfront, consulte [Crear un escenario de automatización de prácticas en Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Para obtener más información sobre las licencias de Workfront Fusion, consulte [Licencias de Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Es posible que su organización no permita el acceso a las hojas de Google. Si ese es el caso, no podrá configurar esta integración, pero la información presentada aquí puede utilizarse como ejemplo general de cómo funcionan los escenarios de integración.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Su organización debe comprar [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar las funciones descritas en este artículo.</td> 
  </tr> 
 </tbody> 
</table>

Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su [!DNL Workfront] administrador.

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Crear un escenario de práctica

El papel de [!DNL Adobe Workfront Fusion] es automatizar los procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de y entre aplicaciones y servicios para crear un escenario que transfiera y transforme sus datos automáticamente. El escenario que cree observa los datos en una aplicación o servicio y procesa esos datos para proporcionar el resultado deseado.

Un escenario consta de una serie de módulos que indican cómo se deben transformar los datos dentro de una aplicación o transferirlos entre aplicaciones y servicios web.

Para explicar cómo crear un escenario y reforzar las prácticas recomendadas a medida que aprende a utilizar [!DNL Workfront Fusion], este artículo le guía paso a paso por el proceso. Crearemos un escenario que cree un nuevo registro en [!DNL Workfront] para cada fila de una [!DNL Google Sheets] hoja de cálculo.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Un escenario como este sería útil si tuviera una hoja de cálculo que enumera los proyectos en los que se debe trabajar usando proyectos en [!DNL Workfront]. El escenario podría &quot;ver&quot; la hoja de cálculo para filas nuevas y agregar un nuevo proyecto en [!DNL Workfront] para cada uno.

La creación de un escenario consta de varias tareas principales:

## Elija las aplicaciones y asigne un nombre al escenario

1. Descargue esto [hoja de cálculo](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)y, a continuación, cárguelo en su [!DNL Google Drive] para su uso durante todo este ejercicio.

   O

   Cree o encuentre su propia sencilla [!DNL Google Sheets] hoja de cálculo similar a esta:

   ![](assets/spreadsheet-headers-350x55.png)

1. Inicie sesión en su [!DNL Workfront Fusion] cuenta.
1. Haga clic en **[!UICONTROL Situaciones]** ![](assets/scenarios-icon.png) en el panel izquierdo.

   En el panel izquierdo que aparece, puede organizar los escenarios en carpetas.

   En la parte superior derecha del área principal, se pueden ver **[!UICONTROL Todo]** escenarios que ha creado, su **[!UICONTROL Escenarios activos]** y **[!UICONTROL Escenarios inactivos]** y **[!UICONTROL Conceptos]**, que son escenarios que necesitan más trabajo antes [!DNL Workfront Fusion] puede clasificarlos como activos o inactivos.

   ![](assets/scenarios-left-panel-350x215.png)

1. En el panel izquierdo, haga clic en el botón **[!UICONTROL Añadir carpeta]** icono ![](assets/add-folder-icon.png)y, a continuación, escriba un nombre como &quot;Situaciones prácticas&quot; para la primera carpeta.

1. Abra la carpeta y haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.

   La página de aterrizaje que se muestra le permite cargar previamente cualquier aplicación que desee utilizar en el escenario que vaya a crear.

1. Para este ejercicio, busque y seleccione la variable **[!UICONTROL Hojas de Google]** aplicación.
1. Haga clic en **[!UICONTROL Continuar]** en la esquina superior derecha.

   Se muestra el editor de escenarios, que contiene un módulo vacío en el centro, la variable [!DNL Google Sheets] aplicación que ha precargado, así como algunas opciones de la barra de herramientas en la parte inferior.

   ![](assets/scenario-editor-350x235.png)

   Cuando empiece a crear un nuevo escenario, es aconsejable comenzar por crear un nombre para él.

1. Seleccione el **[!UICONTROL Nuevo escenario]** nombre del marcador de posición en la esquina superior izquierda y, a continuación, escriba un nombre como &quot;Caso de práctica 1&quot;.
1. Continuar con [Añadir y configurar el primer módulo](#add-and-configure-the-first-module) más abajo.

## Añadir y configurar el primer módulo

El módulo vacío con un signo de interrogación representa el módulo de déclencheur que debe añadir. Este módulo inicia el escenario cada vez que se ejecuta. El icono de reloj del módulo vacío indica que es un módulo programado.

![](assets/empty-module.png)

Este módulo contendrá los datos que desea que el escenario tenga en cuenta.

1. Haga clic en el módulo vacío para elegir la aplicación desde la que desea seleccionar un módulo.

   La aplicación que ha cargado previamente se muestra junto al módulo vacío. Puede agregar cualquier otra aplicación que tenga módulos usando la variable [!UICONTROL Buscar] en la ventana

   ![](assets/pre-loaded-apps-350x139.png)

1. Haga clic **[!DNL Google Sheets]**.

   La lista cambia para mostrar todas las [!DNL Google Sheets] módulos que se pueden usar como módulo de déclencheur.

1. Haga clic en el módulo déclencheur **[!UICONTROL Ver registros]**.

   Ahora debe establecer una conexión autenticada con su cuenta de Google. Todos los módulos que agregue a un escenario deben tener una conexión con su aplicación.

1. En el **[!DNL Google Sheets]** en **[!UICONTROL Conexión]**, haga clic en **[!UICONTROL Agregar]** y, a continuación, escriba un nombre para la conexión, como &quot;Cuenta de Google de Olivia&quot;, y haga clic en **[!UICONTROL Continuar]**.
1. Autentique la conexión en la ventana que aparece.

   El proceso de autenticación de una conexión puede variar un poco entre aplicaciones. Es posible que deba iniciar sesión en la aplicación. Normalmente tendrá que hacer clic en un **[!UICONTROL Permitir]** botón. Si necesita ayuda, consulte [Acerca de la conexión [!DNL Adobe Workfront Fusion] a una aplicación o servicio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configuración del primer módulo

Después de la conexión [!DNL Workfront Fusion] a su [!DNL Google Sheets] cuenta, puede especificar un [!DNL Google Sheets] hoja de cálculo a la que tiene acceso y los datos allí a los que desea que procese el primer módulo.

1. Haga clic en el **[!UICONTROL Hoja de cálculo]** y, a continuación, seleccione **[!UICONTROL Caso práctico de Workfront Fusion] #1** hoja de cálculo de la lista que aparece.

   Esta hoja de cálculo contiene 2 hojas (fichas), por lo que es necesario especificar qué hoja contiene los datos que queremos:

1. En el **[!UICONTROL Hoja]** lista desplegable, seleccione **[!UICONTROL Proyectos]**.

   Nuestra hoja de cálculo contiene encabezados y queremos que el módulo los utilice para identificar los datos que queremos procesar:

   ![](assets/spreadsheet-headers-350x55.png)

1. Leave **[!UICONTROL Sí]** seleccionados para **[!UICONTROL La tabla contiene encabezados]**.

1. En el **[!UICONTROL Fila con encabezados]** , puede especificar un rango de filas que desee incluir, pero dejemos la A1:Z1 predeterminada para este ejercicio.
1. En el **[!UICONTROL Límite]** , escriba 1.

   De este modo, cada vez que ejecute el escenario, el módulo procesará solo 1 fila en la hoja de cálculo. Esto resulta útil para simplificar las ejecuciones de pruebas mientras crea el escenario.

1. Haga clic en **[!UICONTROL OK]**.

   La variable **[!UICONTROL Elija dónde empezar]** le solicita que especifique en qué parte de la hoja de cálculo desea que el módulo inicie el procesamiento.

1. Haga clic en **[!UICONTROL Elegir manualmente]**, seleccione la opción superior de la lista que aparece y haga clic en **[!UICONTROL OK]**.
1. Haga clic con el botón derecho en el módulo y haga clic en **[!UICONTROL Cambiar nombre]** y, a continuación, escriba un nombre que describa lo que desea que haga el módulo (como &quot;Ver la lista de proyectos&quot;) y haga clic en **[!UICONTROL OK]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-350x388.png)

1. Continuar con [Añadir y configurar el segundo módulo](#add-and-configure-the-second-module).

## Añadir y configurar el segundo módulo

1. Haga clic en el círculo parcial a la derecha del del módulo para **[!UICONTROL Añadir otro módulo]**.

   Este segundo módulo debe ser un [!DNL Workfront] , pero no cargamos previamente el [!DNL Workfront] aplicación.

1. Para encontrar la variable [!DNL Workfront] aplicación, empiece a escribir &quot;[!DNL Workfront]&quot; y haga clic en la aplicación cuando aparezca.
1. En la lista de [!DNL Workfront] módulos que aparecen, haga clic en **[!UICONTROL Crear registro]**.

1. Como ya ha hecho anteriormente con la aplicación Google Sheets, haga clic en **[!UICONTROL Agregar]** en el [!DNL Workfront] para añadir una conexión entre Workfront Fusion y Workfront.

   Ahora empezaremos a especificar lo que queremos hacer con los datos de la hoja de cálculo.

1. Haga clic en **[!UICONTROL Tipo de registro]** y, a continuación, seleccione **[!UICONTROL Proyecto]** porque queremos crear un proyecto en [!DNL Workfront] uso de una fila de la hoja de cálculo.

   >[!TIP]
   >
   >Puede encontrar **[!UICONTROL Proyecto]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL proyecto].&quot;

   El cuadro se expande para mostrar todas las opciones disponibles [!DNL Workfront] campos del proyecto en los que puede colocar la información encontrada por el primer módulo.

   Vamos a usar el **[!UICONTROL Nombre]** campo: queremos que este módulo asigne un nombre a cada proyecto en [!DNL Workfront] utilizando el texto de la [!UICONTROL Hojas de Google] fila.

1. Busque y haga clic en el botón **[!UICONTROL Nombre]** campo .

   >[!TIP]
   >
   >Puede usar **Cmd + F** ([!DNL Mac] OS) o **Ctrl-F**([!DNL Windows] OS) para encontrar un campo rápidamente.

   Se abre la lista de variables que puede utilizar en la **[!UICONTROL Nombre]** para definir el nombre de cada proyecto creado en Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Observe que las variables cercanas a la parte superior de la lista corresponden a los encabezados de columna de la hoja de cálculo.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Haga clic en la variable . **[!UICONTROL Mi nombre de proyecto (A)]** para agregarlo al **[!UICONTROL Nombre]** campo .

   Acaba de asignar su primer fragmento de datos para este escenario.

   Asignemos un fragmento más de datos de la hoja de cálculo a [!DNL Workfront]: la fecha de inicio de cada proyecto.

1. Busque y haga clic en el botón **[!UICONTROL Fecha de inicio planeada]** y, a continuación, haga clic en la **[!UICONTROL Fecha de inicio prevista (E)]** para extraer datos de esa columna en la hoja de cálculo.

1. Haga clic en **[!UICONTROL OK]**.

   Ahora tiene un escenario en funcionamiento.

1. Asigne un nombre al segundo módulo como &quot;Crear proyecto de Workfront&quot; y, a continuación, continúe con [Probar el escenario](#test-the-scenario).

## Probar el escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

Para crear un proyecto en Workfront, se ha elegido procesar una fila de la hoja de cálculo. Si ejecuta el escenario, eso es lo que debería suceder.

1. Haga clic en **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja encima de la [!DNL Google Sheets] módulo.

   ![](assets/click-bubble.png)

   En el cuadro que aparece, puede ver información sobre el paquete de datos que el módulo procesó, incluidos los datos reales extraídos de la hoja de cálculo para la fila con la que comenzó.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Haga clic en la burbuja del inspector de ejecución situada encima de la [!DNL Workfront] para ver la entrada de información y el resultado, que es el ID del proyecto creado ahora en [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Puede obtener más información sobre cómo leer la información de ejecución de situaciones en los siguientes artículos:

   * Para obtener información general, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información sobre los paquetes procesados, consulte [Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Vaya a [!DNL Workfront] y busque &quot;loft del centro de soho&quot; para ver el proyecto que creó el escenario. Esta fue la última fila de la hoja de cálculo.
1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** ![](assets/save-icon.png) cerca de la esquina inferior izquierda para guardar el progreso en el escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras establece y prueba un escenario.

## Finalice el escenario y pruébelo de nuevo

Aún necesitamos configurar el escenario para crear proyectos para todas las demás filas de la hoja de cálculo.

1. Haga clic en el **[!UICONTROL Filas de observación]** que ha creado para hojas de Google.
1. Cambie el **[!UICONTROL Límite]** a 100.

   Si especifica un número mayor que el número de filas que conoce que están en la hoja de cálculo, se asegura de que el escenario las capturará a todas.

1. Haga clic con el botón derecho en el **[!UICONTROL Filas de observación]** módulo, haga clic en **[!UICONTROL Elija dónde empezar]**, haga clic en **[!UICONTROL Todo]** y haga clic en **[!UICONTROL OK]**.

1. Haga clic en **[!UICONTROL Ejecutar una vez]** y observe qué sucede en las burbujas del inspector de ejecución.

   La variable [!DNL Google] Hojas **[!UICONTROL Filas de observación]** se ejecuta una vez para leer todas las filas. A continuación, Workfront **[!UICONTROL Crear registro]** se ejecuta 20 veces para crear un proyecto para cada una de las 20 filas restantes de la hoja de cálculo.

1. Haga clic en la burbuja del inspector de ejecución para [!DNL Workfront] para ver las 20 operaciones y, a continuación, haga clic en una de las operaciones para ver la información sobre el proyecto creado.
1. Haga clic en **[!UICONTROL Guardar]** ![](assets/save-icon.png) cerca de la esquina inferior izquierda.
1. Vaya a [!DNL Workfront] para ver los proyectos que creó el escenario.

>[!TIP]
>
>Recomendamos la práctica opcional pero útil de agregar notas sobre cada módulo.
>
>1. Haga clic con el botón derecho en el [!DNL Workfront] y, a continuación, haga clic en **[!UICONTROL Agregar una nota]**.
>1. En la nota que aparece, escriba una descripción general del módulo.

>
>   Esto es útil porque no tendrá que abrir continuamente el módulo para ver qué hace. Puede escribir algo como &quot;Crea un proyecto con Nombre, Fecha de inicio planeada y Prioridad asignada desde la hoja de cálculo&quot;.
>
>   Para la variable [!UICONTROL Hojas de Google] , puede escribir algo como &quot;Ver lista de proyectos para nuevas filas o proyectos agregados&quot;.
>
>   Puede agregar varias notas para un módulo.
>
>1. Cierre las **[!UICONTROL Notas]** .
>
>   Después de agregar una nota a un escenario, aparece un punto naranja en la variable **[!UICONTROL Notas]** icono ![](assets/notes-icon-w-dot.png) en la parte inferior del editor de escenarios.
>
>1. Haga clic en el **[!UICONTROL Notas]** icono ![](assets/notes-icon-w-dot.png) para ver sus notas.

>




## Activar el escenario

Si este fuera un escenario que utilizaría para los datos reales, lo último que haría sería activarlo. Después de activar un escenario, se ejecuta de forma predeterminada cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre la activación de escenarios, consulte [Activar o desactivar un escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
