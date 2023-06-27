---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Cree un escenario de automatización de prácticas en [!DNL Adobe Workfront Fusion]
description: En este artículo se describe cómo crear un escenario de automatización con Adobe Workfront Fusion. Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este ejemplo muestra el proceso de creación de un escenario que busca un proyecto y, a continuación, devuelve todas las tareas asociadas a dicho proyecto.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 0%

---

# Cree un escenario de automatización de prácticas en [!DNL Adobe Workfront Fusion]

En este artículo se describe cómo crear un escenario de automatización con Adobe Workfront Fusion. Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este ejemplo muestra el proceso de creación de un escenario que busca un proyecto y, a continuación, devuelve todas las tareas asociadas a dicho proyecto.

Para obtener instrucciones sobre la creación de un escenario de integración que conecte aplicaciones independientes, consulte [Creación de un escenario de integración de prácticas en Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

Para obtener más información sobre la funcionalidad disponible con cada licencia de Workfront Fusion, consulte [Licencias de Adobe Workfront Fusion](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion]**</td> 
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

## Crear un escenario de práctica

La función de [!DNL Adobe Workfront Fusion] es automatizar sus procesos para que pueda concentrarse en nuevas tareas en lugar de repetir las mismas tareas una y otra vez. Funciona vinculando acciones dentro de las aplicaciones y servicios y entre ellos para crear un escenario que transfiera y transforme los datos automáticamente. El escenario que cree inspecciona los datos de una aplicación o servicio y procesa esos datos para proporcionar el resultado deseado.

Un escenario se compone de una serie de módulos que indican cómo se deben transformar los datos dentro de una aplicación o transferirlos entre aplicaciones y servicios web.
Este ejemplo muestra el proceso de creación de un escenario que busca un [!DNL Workfront] proyecto y devuelve las tareas del proyecto.

![](assets/create-practice-scenario-wf-only-350x157.png)

La creación de un escenario consta de varias tareas principales:

## Elija las aplicaciones y asigne un nombre al escenario

1. Inicie sesión en su [!DNL Workfront Fusion] cuenta.
1. Clic **[!UICONTROL Escenarios]** ![](assets/scenarios-icon.png) en el panel izquierdo.

   >[!NOTE]
   >
   >Si no ve el panel de navegación izquierdo o sus iconos, haga clic en el menú ![Menú](assets/main-menu-icon-left-nav.png) icono.

   En el gris [!UICONTROL Carpetas] , puede organizar los escenarios en carpetas.

   En la parte superior del área principal a la derecha, puede ver **[!UICONTROL Todo]** escenarios que ha creado, sus **[!UICONTROL Escenarios activos]**, **[!UICONTROL Escenarios inactivos]**, y **[!UICONTROL Conceptos]**. Los conceptos son escenarios en los que es necesario trabajar más antes [!DNL Workfront Fusion] Puede clasificarlos como activos o inactivos.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. En el [!UICONTROL Carpetas] , haga clic en **[!UICONTROL Añadir carpeta]** icono ![](assets/add-folder-icon.png)A continuación, escriba un nombre como &quot;Escenarios de práctica&quot; para la primera carpeta.

1. Abra la carpeta y haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.

   La página de aterrizaje que se muestra le permite cargar previamente cualquier aplicación que desee utilizar en el escenario que va a crear.

1. Para este ejercicio, busque y seleccione **[!DNL Workfront]** aplicación.
1. Clic **[!UICONTROL Continuar]** en la esquina superior derecha.

   El editor de escenarios muestra, con un módulo vacío en el centro, el [!DNL Workfront] La aplicación que ha cargado previamente y algunas opciones en la barra de herramientas de la parte inferior.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

Cuando empiece a crear un nuevo escenario, es aconsejable empezar creando un nombre para él.

1. Seleccione el **[!UICONTROL Nuevo escenario]** Nombre del marcador de posición en la esquina superior izquierda y, a continuación, escriba un nombre como &quot;Escenario de práctica 1&quot;.
1. Continuar con [Adición y configuración del primer módulo](#add-and-configure-the-first-module) más abajo.

## Adición y configuración del primer módulo

El módulo vacío con un signo de interrogación representa el módulo de déclencheur que debe agregar. Este módulo iniciará el escenario cada vez que se ejecute. El icono de reloj del módulo vacío indica que es un módulo programado.

![](assets/empty-module.png)

Este módulo contendrá los datos que desea que el escenario observe.

Para este ejemplo, no se utiliza un módulo de déclencheur. En su lugar, este escenario comienza con una búsqueda.

1. Haga clic en el módulo vacío para elegir la aplicación desde la que seleccionará un módulo.

   La aplicación que ha cargado previamente anteriormente se muestra junto al módulo vacío. Puede agregar cualquier otra aplicación que tenga módulos usando [!UICONTROL Buscar] cuadro.

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Haga clic **[!DNL Workfront]**.

   La lista cambia para mostrar todo [!DNL Workfront] módulos que puede utilizar como módulo de déclencheur.

1. Haga clic en el módulo Buscar **[!UICONTROL Buscar]**.

   Ahora debe establecer una conexión autenticada con su [!DNL Workfront] cuenta. Cada módulo que agregue a un escenario debe tener una conexión con su aplicación.

1. En el **[!DNL Workfront]** cuadro, debajo de **[!UICONTROL Conexión]**, haga clic en **[!UICONTROL Añadir]** A continuación, escriba un nombre para la conexión, como &quot;Cuenta de Workfront de Olivia&quot;, y haga clic en **[!UICONTROL Continuar]**.
1. Autentique la conexión en la ventana que aparece.

   El proceso de autenticación de una conexión puede variar un poco entre aplicaciones. El siguiente proceso es específico de [!DNL Workfront], pero el proceso es similar al de muchas aplicaciones.

   1. Introduzca su [!DNL Workfront] dominio y haga clic en **[!UICONTROL Continuar]**.
   1. Iniciar sesión en [!DNL Workfront].
   1. Examine el acceso que [!DNL Workfront Fusion] está solicitando y haga clic en **[!UICONTROL Permitir el acceso]**.

   Si necesita ayuda, consulte [Acerca de conectar [!DNL Adobe Workfront Fusion] a una aplicación o servicio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configuración del primer módulo

Después de conectar [!DNL Workfront Fusion] a su [!DNL Workfront] cuenta, puede especificar una [!DNL Workfront] la cola de solicitudes a la que tiene acceso y los datos que desea que procese el primer módulo.

1. En el [!UICONTROL Tipo de registro] , seleccione **[!UICONTROL Proyecto]**. Esto configura el módulo para que solo busque proyectos.

   >[!TIP]
   >
   >Puede encontrar **[!UICONTROL Proyecto]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL proyecto].&quot;

1. En el **[!UICONTROL Conjunto de resultados]** , seleccione **[!UICONTROL Primer registro coincidente]**. Esto configura el módulo para que devuelva únicamente el primer registro que encuentre que cumpla los criterios. Para este ejemplo, solo necesitamos devolver un registro.
1. En el **[!UICONTROL Criterios de búsqueda]** área, configuraremos un filtro para devolver el proyecto específico.

   1. En el primer cuadro debajo de [!UICONTROL Criterios de búsqueda], seleccione el campo en el que desea buscar los valores. Para este ejemplo, seleccione **[!UICONTROL Nombre]**.
   1. Para el operador, seleccione [!UICONTROL Contiene (sin distinción de mayúsculas)]. Esto permite que el módulo encuentre proyectos con las palabras elegidas en el nombre, aunque no introduzca el nombre completo o el nombre con mayúsculas o minúsculas incorrectas (como todas las mayúsculas).
   1. En el último campo debajo de [!UICONTROL Criterios de búsqueda], escriba una palabra o frase que sepa que está en el nombre del proyecto que está buscando.

1. En el **[!UICONTROL Salidas]** , seleccione los campos de salida de los que desea que salga el problema. Para este ejemplo, seleccione **[!UICONTROL ID]** y **[!UICONTROL Nombre]** campos.

   >[!TIP]
   >
   >Puede utilizar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para buscar un campo rápidamente.

1. Clic **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(Solo información) Dado que no se trata de un módulo de déclencheur, no elige dónde iniciarlo. Al utilizar un módulo de déclencheur, ahora debe seleccionar dónde iniciarlo.
   >
   >
   >Para obtener más información, consulte [Elija dónde comienza un módulo de déclencheur en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Haga clic con el botón derecho en el módulo y seleccione **[!UICONTROL Cambiar nombre]**, escriba un nombre y describa lo que desea que haga el módulo (por ejemplo, &quot;Buscar proyecto&quot;) y haga clic en **[!UICONTROL OK]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-wf.png)

1. Continuar con [Adición y configuración del segundo módulo](#add-and-configure-the-second-module).

## Adición y configuración del segundo módulo

1. Haga clic en el círculo parcial a la derecha del del del módulo para **[!UICONTROL Añadir otro módulo]**.
1. Seleccionar [!DNL Workfront] en la lista de aplicaciones, seleccione el módulo de búsqueda **[!UICONTROL Leer registros relacionados]**.
1. Ya ha creado una conexión con [!DNL Workfront] para el módulo anterior. No es necesario que vuelva a crearlo aquí, pero debe asegurarse de que este módulo utiliza la misma conexión que el módulo anterior.\
   En el **[!UICONTROL Conexión]** , seleccione la conexión que creó para el módulo anterior.
1. Clic **[!UICONTROL Tipo de registro]**, luego seleccione **[!UICONTROL Proyecto]**, porque queremos leer registros relacionados con un proyecto.

   >[!TIP]
   >
   >Puede encontrar **[!UICONTROL Proyecto]** en la lista si empieza a escribir la palabra &quot;proyecto&quot;.

1. Haga clic en **[!UICONTROL Identificador de registro principal]** field. Este campo necesita el Workfront ID del proyecto desde el que desea devolver las tareas.

   Al hacer clic en el campo se abre la lista de variables que puede utilizar en la variable **[!UICONTROL Identificador de registro principal]** para identificar el proyecto en Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Haga clic en la variable **[!UICONTROL ID]** para agregarlo al **[!UICONTROL Identificador de registro principal]** field. Esto permite que el ID devuelto por el primer módulo se utilice como identificador del proyecto con el que desea trabajar en el segundo módulo, lo que garantiza que las tareas devueltas pertenezcan a ese proyecto.
1. En el **[!UICONTROL Colecciones]** , seleccione **[!UICONTROL Tareas]**. Esto indica que el módulo debe devolver las tareas asociadas con el proyecto elegido.
1. Clic **[!UICONTROL OK]**

   Ahora tiene un escenario de trabajo.

1. Asigne un nombre al segundo módulo, como &quot;Devolver tareas asociadas con el proyecto&quot; y, a continuación, continúe con [Prueba del escenario](#test-the-scenario).

## Prueba del escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

Elegimos que se devolviera 1 proyecto, así como las tareas asociadas con dicho proyecto. Si ejecuta el escenario, eso es lo que debería suceder.

1. Clic **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja situada encima del primer módulo.

   ![](assets/click-bubble.png)

   En el cuadro que aparece, puede ver información sobre el conjunto de datos que procesó el módulo, incluidos los datos reales extraídos del proyecto que devolvió el módulo.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Haga clic en la burbuja del inspector de ejecución situada encima del segundo módulo para ver la entrada de información y la salida, que es una recopilación de tareas incluidas en el proyecto.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Puede obtener más información sobre cómo leer la información de ejecución de escenarios en los siguientes artículos:

   * Para obtener información general, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información sobre los paquetes procesados, consulte [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Entrada [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** ![](assets/save-icon.png) cerca de la esquina inferior izquierda para guardar el progreso del escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras perfecciona y prueba un escenario.

>[!TIP]
>
>Recomendamos la práctica opcional pero útil de agregar notas sobre cada módulo.
>
>1. Haga clic con el botón derecho en [!DNL Workfront] módulo y haga clic en **[!UICONTROL Añadir una nota]**.
>1. En la nota que se muestra, escriba una descripción general del módulo.
>
>    Puede agregar varias notas para un módulo.
>
>1. Cierre el **[!UICONTROL Notas]** área.
>
>     Después de agregar una nota a un escenario, aparece un punto naranja en la etiqueta **[!UICONTROL Notas]** icono ![](assets/notes-icon-w-dot.png) en la parte inferior del editor de escenarios.
>
>1. Haga clic en **[!UICONTROL Notas]** icono ![](assets/notes-icon-w-dot.png) para ver las notas.
>



## Activación del escenario

Este escenario de ejemplo no tiene un módulo de déclencheur. Si este fuera un escenario que usaría para datos reales, empezaría con un módulo de déclencheur y lo último que haría es activarlo. Después de activar un escenario, de forma predeterminada, se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre la activación de escenarios, consulte [Activación o desactivación de un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
