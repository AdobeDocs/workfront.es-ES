---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Creación de un escenario de integración de prácticas en Adobe Workfront Fusion
description: La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación. Este artículo ha quedado obsoleto, pero contiene un vínculo al nuevo artículo que cubre esta funcionalidad.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '2188'
ht-degree: 96%

---

# Creación de un escenario de integración de prácticas en Adobe Workfront Fusion

>[!IMPORTANT]
>
>La documentación de Adobe Workfront Fusion se ha trasladado a una nueva ubicación.
>
>La información de este artículo ahora se encuentra en el artículo:
>
>* [Flujo de trabajo para crear un escenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Actualice sus marcadores.
>
>Este artículo ya no se actualiza y se eliminará en un futuro próximo.

En este artículo se describe cómo crear un escenario de integración con Adobe Workfront Fusion. Los escenarios de integración conectan aplicaciones independientes entre sí, lo que permite que los datos fluyan por distintas aplicaciones.

Para crear un escenario de integración, su organización debe tener una licencia de [!DNL Workfront Fusion for Work Automation and Integration].

Para obtener instrucciones sobre cómo crear un escenario de automatización solo de Workfront, consulte [Crear un escenario de automatización de prácticas en Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Para obtener más información sobre las licencias de Workfront Fusion, consulte [licencias de Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Es posible que su organización no permita el acceso a Google Sheets. En ese caso, no podrá configurar esta integración, pero la información presentada aquí puede utilizarse como ejemplo general del funcionamiento de los escenarios de integración.

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

Para obtener información sobre las licencias de [!DNL Adobe Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Crear un escenario de práctica

La función de [!DNL Adobe Workfront Fusion] es automatizar sus procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de las aplicaciones y servicios y entre ellos para crear un escenario que transfiera y transforme los datos automáticamente. El escenario que crea ve los datos de una aplicación o servicio y los procesa para proporcionar el resultado deseado.

Un escenario se compone de una serie de módulos que indican cómo se deben transformar los datos dentro de una aplicación o transferirse entre aplicaciones y servicios web.

Para explicar cómo crear un escenario y reforzar las prácticas recomendadas a medida que aprende a utilizar [!DNL Workfront Fusion], este artículo le explica el proceso paso a paso. Crearemos un escenario en el que se cree un nuevo registro en [!DNL Workfront] por cada fila de una hoja de cálculo de [!DNL Google Sheets].

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Un escenario como este podría ser útil si tuviera una hoja de cálculo con una lista de proyectos en los que hay que trabajar utilizando proyectos en [!DNL Workfront]. El escenario podría “inspeccionar” la hoja de cálculo en busca de nuevas filas y añadir un nuevo proyecto en [!DNL Workfront] para cada una de ellas.

La creación de un escenario consta de varias tareas principales:

## Elegir las aplicaciones y dar un nombre al escenario

1. Descargue esta [hoja de cálculo](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx) y, a continuación, cárguela a su [!DNL Google Drive] para usarla durante este ejercicio.

   O

   Cree o encuentre su propia hoja de cálculo sencilla de [!DNL Google Sheets] similar a esta:

   ![](assets/spreadsheet-headers-350x55.png)

1. Inicie sesión en la cuenta de [!DNL Workfront Fusion].
1. Haga clic en **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) en el panel izquierdo.

   >[!NOTE]
   >
   >Si no ve el panel de navegación izquierdo o sus iconos, haga clic en el icono ![Menú](assets/main-menu-icon-left-nav.png).

   En el panel gris [!UICONTROL Carpetas] que se muestra, puede organizar los escenarios en carpetas.

   En la parte superior del área principal, a la derecha, puede ver **[!UICONTROL Todos]** los escenarios que ha creado, los **[!UICONTROL Escenarios activos]** y los **[!UICONTROL Escenarios inactivos]**, y los **[!UICONTROL Conceptos]**, que son escenarios que necesitan algo más de trabajo antes de que [!DNL Workfront Fusion] pueda clasificarlos como activos o inactivos.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. En el panel [!UICONTROL Carpetas], haga clic en el icono **[!UICONTROL Añadir carpeta]** ![](assets/add-folder-icon.png) y escriba un nombre como “Escenarios de práctica” para su primera carpeta.

1. Abra la carpeta y haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.

   La página de aterrizaje que se muestra le permite subir previamente cualquier aplicación que desee utilizar en el escenario que va a crear.

1. Para este ejercicio, busque y seleccione la aplicación **[!UICONTROL Google Sheets]**.
1. Haga clic en **[!UICONTROL Continuar]** en la esquina superior derecha.

   Aparece el editor de escenarios, que contiene un módulo vacío en el centro, la aplicación [!DNL Google Sheets] que cargado previamente y algunas opciones en la barra de herramientas de la parte inferior.

<!--
   ![](assets/scenario-editor.png)
-->

Cuando empiece a crear un nuevo escenario, es aconsejable empezar por darle un nombre.

1. Seleccione el nombre del marcador de posición **[!UICONTROL Nuevo escenario]** en la esquina superior izquierda y, a continuación, escriba un nombre como “Práctica de escenario 1”.
1. Continúe con [Añadir y configurar el primer módulo](#add-and-configure-the-first-module) a continuación.

## Añadir y configurar el primer módulo

El módulo vacío con un signo de interrogación representa el módulo de activador que debe añadir. Este módulo iniciará el escenario cada vez que se ejecute. El icono de reloj del módulo vacío indica que es un módulo programado.

![](assets/empty-module.png)

Este módulo contendrá los datos que desea que el escenario vea.

1. Haga clic en el módulo vacío para elegir la aplicación desde la que seleccionará un módulo.

   La aplicación que ha cargado anteriormente se muestra junto al módulo vacío. Puede añadir cualquier otra aplicación que tenga módulos mediante el cuadro [!UICONTROL Buscar].

   ![](assets/pre-loaded-apps-350x139.png)

1. Haga clic en **[!DNL Google Sheets]**.

   La lista cambia para mostrar todos los módulos de [!DNL Google Sheets] que puede utilizar como módulo de activador.

1. Haga clic en el módulo de activador **[!UICONTROL Observar registros]**.

   Ahora debe establecer una conexión autenticada con su cuenta de Google. Cada módulo que añada a un escenario debe tener una conexión con su aplicación.

1. En el cuadro **[!DNL Google Sheets]**, en **[!UICONTROL Conexión]**, haga clic en **[!UICONTROL Agregar]**, escriba un nombre para la conexión, como “Cuenta de Google de Olivia”, y haga clic en **[!UICONTROL Continuar]**.
1. Autentique la conexión en la ventana que aparece.

   El proceso de autenticación de una conexión puede variar un poco entre aplicaciones. Es posible que tenga que iniciar sesión en la aplicación. Normalmente, tendrá que hacer clic en un botón **[!UICONTROL Permitir]**. Si necesita ayuda, consulte [Información general sobre las conexiones](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configurar el primer módulo

Después de conectar [!DNL Workfront Fusion] a su cuenta de [!DNL Google Sheets], puede especificar una hoja de cálculo de [!DNL Google Sheets] a la que tenga acceso y los datos que desea que procese el primer módulo.

1. Haga clic en el cuadro **[!UICONTROL Hoja de cálculo]** y, a continuación, seleccione la hoja de cálculo **[!UICONTROL Workfront Fusion practice scenario] #1** en la lista que aparece.

   Esta hoja de cálculo contiene 2 hojas (pestañas), por lo que es necesario especificar qué hoja contiene los datos deseados:

1. En la lista desplegable **[!UICONTROL Hoja]**, seleccione **[!UICONTROL Proyectos]**.

   Nuestra hoja de cálculo contiene encabezados y queremos que el módulo los utilice para identificar los datos que queremos procesar:

   ![](assets/spreadsheet-headers-350x55.png)

1. Deje seleccionado **[!UICONTROL Sí]** para **[!UICONTROL La tabla contiene encabezados]**.

1. En el cuadro **[!UICONTROL Fila con encabezados]**, puede especificar el rango de filas que desea incluir, pero dejemos el valor predeterminado A1:Z1 para este ejercicio.
1. En el cuadro **[!UICONTROL Límite]**, escriba 1.

   De este modo, cada vez que ejecute el escenario, el módulo procesará solo 1 fila en la hoja de cálculo. Esto resulta útil para simplificar las ejecuciones de prueba mientras crea el escenario.

1. Haga clic en **[!UICONTROL Aceptar]**.

   El cuadro **[!UICONTROL Elegir por dónde empezar]** le pide que especifique en qué parte de la hoja de cálculo desea que comience a procesarse el módulo.

1. Haga clic en **[!UICONTROL Elegir manualmente]**, seleccione la opción superior en la lista que aparece y, a continuación, haga clic en **[!UICONTROL Aceptar]**.
1. Haga clic con el botón secundario en el módulo, haga clic en **[!UICONTROL Cambiar nombre]**, escriba un nombre que describa lo que desea que haga el módulo (como “Ver la lista de proyectos”) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-350x388.png)

1. Continúe con [Añadir y configurar el segundo módulo](#add-and-configure-the-second-module).

## Añadir y configurar el segundo módulo

1. Haga clic en el círculo parcial a la derecha del módulo para **[!UICONTROL añadir otro módulo]**.

   Este segundo módulo debe ser un módulo [!DNL Workfront], pero no se precargó la aplicación [!DNL Workfront].

1. Para encontrar la aplicación [!DNL Workfront], empiece a escribir “[!DNL Workfront]” y haga clic en la aplicación cuando aparezca.
1. En la lista de módulos de [!DNL Workfront] que aparece, haga clic en **[!UICONTROL Crear registro]**.

1. Tal como hizo anteriormente con la aplicación Google Sheets, haga clic en **[!UICONTROL Añadir]** en el cuadro [!DNL Workfront] para añadir una conexión entre Workfront Fusion y Workfront.

   Ahora empezaremos a especificar qué queremos hacer con los datos de la hoja de cálculo.

1. Haga clic en **[!UICONTROL Record type]** y, a continuación, seleccione **[!UICONTROL Project]** porque queremos crear un proyecto en [!DNL Workfront] utilizando una fila de la hoja de cálculo.

   >[!TIP]
   >
   >Puede encontrar **[!UICONTROL Project]** en la lista si empieza a escribir la palabra “[!UICONTROL project]”.

   El cuadro se expande para mostrar todos los campos de proyecto de [!DNL Workfront] disponibles donde puede colocar la información que encontró el primer módulo.

   Vamos a usar el campo **[!UICONTROL Name]**: queremos que este módulo asigne un nombre a cada proyecto de [!DNL Workfront] usando el texto en la fila [!UICONTROL Google Sheets] correspondiente.

1. Busque y haga clic en el campo **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Puede usar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F**([!DNL Windows] OS) para encontrar un campo rápidamente.

   Se abrirá la lista de variables que puede usar en el campo **[!UICONTROL Name]** para definir el nombre de cada proyecto creado en Workfront.

   ![](assets/list-of-available-variables-350x261.png)

   Observe que las variables cerca de la parte superior de la lista corresponden a los encabezados de columna de la hoja de cálculo.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Haga clic en la variable **[!UICONTROL My Project Name (A)]** para añadirla al campo **[!UICONTROL Name]**.

   Acaba de asignar el primer fragmento de datos para este escenario.

   Asignemos un fragmento más de datos de la hoja de cálculo a [!DNL Workfront]: la fecha de inicio de cada proyecto.

1. Busque y haga clic en el campo **[!UICONTROL Planned Start Date]** y, a continuación, haga clic en la variable **[!UICONTROL Planned Begin Date (E)]** para extraer datos de esa columna en la hoja de cálculo.

1. Haga clic en **[!UICONTROL OK]**.

   Ahora tiene un escenario de trabajo.

1. Asigne un nombre al segundo módulo, como “Crear proyecto de Workfront” y continúe con [Probar el escenario](#test-the-scenario).

## Probar el escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

Elegimos procesar 1 fila de la hoja de cálculo para crear un proyecto en Workfront. Si ejecuta el escenario, eso es lo que debería suceder.

1. Haga clic en **[!UICONTROL Run once]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja situada encima del módulo [!DNL Google Sheets].

   ![](assets/click-bubble.png)

   En el cuadro que aparece, puede ver información sobre el conjunto de datos que procesó el módulo, incluidos los datos reales extraídos de la hoja de cálculo para la fila con la que comenzó.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Haga clic en la burbuja del inspector de ejecución situada encima del módulo [!DNL Workfront] para ver la entrada de información y la salida, que es el identificador del proyecto que se está creando en [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Puede obtener más información sobre cómo leer la información de ejecución de escenarios en los siguientes artículos:

   * Para obtener información general, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información acerca de los paquetes procesados, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Vaya a [!DNL Workfront] y busque &quot;soho center loft&quot; para ver el proyecto que creó el escenario. Esta era la última fila de la hoja de cálculo.
1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Save]** ![](assets/save-icon.png) cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

   >[!IMPORTANT]
   >
   >Se recomienda guardar con frecuencia mientras se perfeccionan y prueban escenarios.

## Finalice el escenario y vuelva a probarlo

Aún tenemos que configurar el escenario para crear proyectos para todas las demás filas de la hoja de cálculo.

1. Haga clic en el módulo **[!UICONTROL Watch Rows]** que creó para las hojas de Google.
1. Cambie el **[!UICONTROL Límite]** a 100.

   La especificación de un número mayor que el número de filas que sabe que están en la hoja de cálculo garantiza que el escenario las capturará todas.

1. Haga clic con el botón secundario en el módulo **[!UICONTROL Watch Rows]**, haga clic en **[!UICONTROL Choose where to start]**, haga clic en **[!UICONTROL All]** y, a continuación, haga clic en **[!UICONTROL OK]**.

1. Haga clic en **[!UICONTROL Run once]** y observe qué sucede en las burbujas del inspector de ejecución.

   El módulo [!DNL Google] Sheets **[!UICONTROL Watch Rows]** se ejecuta una vez para leer todas las filas. A continuación, el módulo **[!UICONTROL Create Record]** de Workfront se ejecuta 20 veces para crear un proyecto para cada una de las 20 filas restantes de la hoja de cálculo.

1. Haga clic en la burbuja del inspector de ejecución del módulo [!DNL Workfront] para ver las 20 operaciones y, a continuación, haga clic en una de ellas para ver la información sobre el proyecto creado.
1. Haga clic en **[!UICONTROL Save]** ![](assets/save-icon.png) cerca de la esquina inferior izquierda.
1. Vaya a [!DNL Workfront] para ver los proyectos que creó el escenario.

>[!TIP]
>
>Recomendamos la práctica opcional pero útil de añadir notas sobre cada módulo.
>
>1. Haga clic con el botón secundario en el módulo [!DNL Workfront] y, a continuación, haga clic en **[!UICONTROL Add a note]**.
>1. En la nota que se muestra, escriba una descripción general del módulo.
>
>    Esto resulta útil porque no tiene que abrir continuamente el módulo para ver qué hace. Puede escribir algo como “Crea un proyecto con el nombre, la fecha de inicio planificada y la prioridad asignada desde la hoja de cálculo”.
>
>    Para el módulo [!UICONTROL Google Sheets], podría escribir algo como “Observar lista de proyectos para nuevas filas/proyectos añadidos”.
>
>    Puede añadir varias notas para un módulo.
>
>1. Cierre el área **[!UICONTROL Notas]**.
>
>    Después de añadir una nota a un escenario, aparece un punto naranja en el icono **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) en la parte inferior del editor de escenarios.
>
>1. Haga clic en el icono **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) para ver sus notas.
>



## Activar el escenario

Si se tratara de un escenario que utilizase para datos reales, lo último que haría es activarlo. Después de activar un escenario, de forma predeterminada, se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre cómo activar escenarios, consulte [Activar o desactivar escenarios en Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programación de escenarios en Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
