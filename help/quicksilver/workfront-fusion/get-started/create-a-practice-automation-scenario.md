---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Cree un escenario de automatización de prácticas en [!DNL Adobe Workfront Fusion]
description: En este artículo se describe cómo crear un escenario de automatización con Adobe Workfront Fusion. Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este ejemplo le guía durante el proceso de creación de un escenario que busca un proyecto y luego devuelve todas las tareas asociadas a ese proyecto.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1782'
ht-degree: 0%

---

# Cree un escenario de automatización de prácticas en [!DNL Adobe Workfront Fusion]

En este artículo se describe cómo crear un escenario de automatización con Adobe Workfront Fusion. Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este ejemplo le guía durante el proceso de creación de un escenario que busca un proyecto y luego devuelve todas las tareas asociadas a ese proyecto.

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
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de [!UICONTROL Adobe Workfront Fusion**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para integración y automatización de trabajo] </p><p>[!UICONTROL [!DNL Workfront Fusion] para la automatización del trabajo]</p>  </td> 
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
Este ejemplo lo lleva a través del proceso de creación de un escenario que busca un [!DNL Workfront] y devuelve las tareas del proyecto.

![](assets/create-practice-scenario-wf-only-350x157.png)

La creación de un escenario consta de varias tareas principales:

## Elija las aplicaciones y asigne un nombre al escenario

1. Inicie sesión en su [!DNL Workfront Fusion] cuenta.
1. Haga clic en **[!UICONTROL Situaciones]** ![](assets/scenarios-icon.png) en el panel izquierdo.

   En el panel izquierdo que aparece, puede organizar los escenarios en carpetas.

   En la parte superior derecha del área principal, se pueden ver **[!UICONTROL Todo]** escenarios que ha creado, su **[!UICONTROL Escenarios activos]**, **[!UICONTROL Escenarios inactivos]** y **[!UICONTROL Conceptos]**. Los conceptos son escenarios que necesitan más trabajo antes [!DNL Workfront Fusion] puede clasificarlos como activos o inactivos.

   ![](assets/scenarios-left-panel-350x215.png)

1. En el panel izquierdo, haga clic en el botón **[!UICONTROL Añadir carpeta]** icono ![](assets/add-folder-icon.png)y, a continuación, escriba un nombre como &quot;Situaciones prácticas&quot; para la primera carpeta.

1. Abra la carpeta y haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.

   La página de aterrizaje que se muestra le permite cargar previamente cualquier aplicación que desee utilizar en el escenario que vaya a crear.

1. Para este ejercicio, busque y seleccione la variable **[!DNL Workfront]** aplicación.
1. Haga clic en **[!UICONTROL Continuar]** en la esquina superior derecha.

   Se muestra el editor de escenarios, que contiene un módulo vacío en el centro, la variable [!DNL Workfront] aplicación que ha precargado, así como algunas opciones de la barra de herramientas en la parte inferior.

   ![](assets/scenario-editor-350x235.png)

   Cuando empiece a crear un nuevo escenario, es aconsejable comenzar por crear un nombre para él.

1. Seleccione el **[!UICONTROL Nuevo escenario]** nombre del marcador de posición en la esquina superior izquierda y, a continuación, escriba un nombre como &quot;Caso de práctica 1&quot;.
1. Continuar con [Añadir y configurar el primer módulo](#add-and-configure-the-first-module) más abajo.

## Añadir y configurar el primer módulo

El módulo vacío con un signo de interrogación representa el módulo de déclencheur que debe añadir. Este módulo inicia el escenario cada vez que se ejecuta. El icono de reloj del módulo vacío indica que es un módulo programado.

![](assets/empty-module.png)

Este módulo contendrá los datos que desea que el escenario tenga en cuenta.

Para este ejemplo, no se utiliza un módulo de déclencheur. En su lugar, este escenario comienza con una búsqueda.

1. Haga clic en el módulo vacío para elegir la aplicación desde la que desea seleccionar un módulo.

   La aplicación que ha cargado previamente se muestra junto al módulo vacío. Puede agregar cualquier otra aplicación que tenga módulos usando la variable [!UICONTROL Buscar] en la ventana

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Haga clic **[!DNL Workfront]**.

   La lista cambia para mostrar todas las [!DNL Workfront] módulos que se pueden usar como módulo de déclencheur.

1. Haga clic en el módulo Buscar **[!UICONTROL Buscar]**.

   Ahora debe establecer una conexión autenticada con su [!DNL Workfront] cuenta. Todos los módulos que agregue a un escenario deben tener una conexión con su aplicación.

1. En el **[!DNL Workfront]** en **[!UICONTROL Conexión]**, haga clic en **[!UICONTROL Agregar]** y, a continuación, escriba un nombre para la conexión, como &quot;Cuenta de Workfront de Olivia&quot;, y haga clic en **[!UICONTROL Continuar]**.
1. Autentique la conexión en la ventana que aparece.

   El proceso de autenticación de una conexión puede variar un poco entre aplicaciones. El siguiente proceso es específico de [!DNL Workfront], pero el proceso es similar a muchas aplicaciones.

   1. Escriba la [!DNL Workfront] y, a continuación, haga clic en **[!UICONTROL Continuar]**.
   1. Iniciar sesión [!DNL Workfront].
   1. Examine el acceso que [!DNL Workfront Fusion] está solicitando, luego haga clic en **[!UICONTROL Permitir acceso]**.

   Si necesita ayuda, consulte [Acerca de la conexión [!DNL Adobe Workfront Fusion] a una aplicación o servicio](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Configuración del primer módulo

Después de la conexión [!DNL Workfront Fusion] a su [!DNL Workfront] cuenta, puede especificar un [!DNL Workfront] la cola de solicitudes a la que tiene acceso y los datos allí a los que desea que procese el primer módulo.

1. En el [!UICONTROL Tipo de registro] , seleccione **[!UICONTROL Proyecto]**. Esto configura el módulo para que busque solo proyectos.

   >[!TIP]
   >
   >Puede encontrar **[!UICONTROL Proyecto]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL proyecto].&quot;

1. En el **[!UICONTROL Conjunto de resultados]** , seleccione **[!UICONTROL Primer registro coincidente]**. Esto configura el módulo para que devuelva solo el primer registro que encuentra que cumple los criterios. Para este ejemplo, solo necesitamos que se devuelva un registro.
1. En el **[!UICONTROL Criterios de búsqueda]** , configuraremos un filtro para devolver el proyecto específico.

   1. En el primer cuadro debajo de [!UICONTROL Criterios de búsqueda], seleccione el campo del que desea buscar los valores. Para este ejemplo, seleccione **[!UICONTROL Nombre]**.
   1. Para el operador , seleccione [!UICONTROL Contiene (sin distinción de mayúsculas y minúsculas)]. Esto permite que el módulo encuentre proyectos con las palabras elegidas en su nombre, incluso si no introduce el nombre completo o escribe el nombre con mayúsculas o minúsculas incorrectas (como todas las mayúsculas).
   1. En el último campo de [!UICONTROL Criterios de búsqueda], escriba una palabra o frase que sepa que está en el nombre del proyecto que está buscando.

1. En el **[!UICONTROL Salidas]** seleccione los campos que desea que muestre el problema. Para este ejemplo, seleccione la **[!UICONTROL ID]** y **[!UICONTROL Nombre]** campos.

   >[!TIP]
   >
   >Puede usar **Cmd + F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para encontrar un campo rápidamente.

1. Haga clic en **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(Solo información) Dado que no es un módulo de déclencheur, no elige dónde iniciarlo. Al utilizar un módulo de déclencheur, ahora debería seleccionar dónde iniciarlo.
   >
   >
   >Para obtener más información, consulte [Elija dónde comienza un módulo de déclencheur en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Haga clic con el botón derecho en el módulo y haga clic en **[!UICONTROL Cambiar nombre]** y, a continuación, escriba un nombre que describa lo que desea que haga el módulo (como &quot;Buscar proyecto&quot;) y haga clic en **[!UICONTROL OK]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-wf.png)

1. Continuar con [Añadir y configurar el segundo módulo](#add-and-configure-the-second-module).

## Añadir y configurar el segundo módulo

1. Haga clic en el círculo parcial a la derecha del del módulo para **[!UICONTROL Añadir otro módulo]**.
1. Select [!DNL Workfront] en la lista de aplicaciones, elija el módulo de búsqueda **[!UICONTROL Leer registros relacionados]**.
1. Ya ha creado una conexión con [!DNL Workfront] para el módulo anterior. No es necesario volver a crearlo aquí, pero debe asegurarse de que este módulo esté utilizando la misma conexión que el módulo anterior.\
   En el **[!UICONTROL Conexión]** , seleccione la conexión que ha creado para el módulo anterior.
1. Haga clic en **[!UICONTROL Tipo de registro]** y, a continuación, seleccione **[!UICONTROL Proyecto]**, porque queremos leer registros relacionados con un proyecto.

   >[!TIP]
   >
   >Puede encontrar **[!UICONTROL Proyecto]** en la lista si comienza a escribir la palabra &quot;proyecto&quot;.

1. Haga clic en el **[!UICONTROL ID de registro principal]** campo . Este campo requiere el Workfront ID del proyecto desde el que desea devolver las tareas.

   Al hacer clic en el campo, se abre la lista de variables que puede utilizar en la variable **[!UICONTROL ID de registro principal]** para identificar el proyecto en Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Haga clic en la variable . **[!UICONTROL ID]** para agregarlo al **[!UICONTROL ID de registro principal]** campo . Esto permite que el ID devuelto desde el primer módulo se utilice como identificador para el proyecto con el que desea trabajar en el segundo módulo, lo que garantiza que las tareas devueltas pertenezcan a ese proyecto.
1. En el **[!UICONTROL Colecciones]** campo, seleccione **[!UICONTROL Tareas]**. Esto indica que el módulo es para devolver tareas asociadas con el proyecto elegido.
1. Haga clic en **[!UICONTROL OK]**

   Ahora tiene un escenario en funcionamiento.

1. Asigne un nombre al segundo módulo como &quot;Devolver tareas asociadas con el proyecto&quot; y, a continuación, continúe con [Probar el escenario](#test-the-scenario).

## Probar el escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

Elegimos que se devolviera un proyecto, así como las tareas asociadas con ese proyecto. Si ejecuta el escenario, eso es lo que debería suceder.

1. Haga clic en **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja encima del primer módulo.

   ![](assets/click-bubble.png)

   En el cuadro que aparece, puede ver información sobre el paquete de datos que el módulo procesó, incluidos los datos reales extraídos del proyecto que el módulo devolvió.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Haga clic en la burbuja del inspector de ejecución situada encima del módulo Second para ver la entrada de información y la salida, que es una colección de tareas incluidas en el proyecto.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Puede obtener más información sobre cómo leer la información de ejecución de situaciones en los siguientes artículos:

   * Para obtener información general, consulte [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información sobre los paquetes procesados, consulte [Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** ![](assets/save-icon.png) cerca de la esquina inferior izquierda para guardar el progreso en el escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras establece y prueba un escenario.

>[!TIP]
>
>Recomendamos la práctica opcional pero útil de agregar notas sobre cada módulo.
>
>1. Haga clic con el botón derecho en un [!DNL Workfront] y, a continuación, haga clic en **[!UICONTROL Agregar una nota]**.
>1. En la nota que aparece, escriba una descripción general del módulo.

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

Este caso de ejemplo no tiene un módulo de déclencheur. Si este fuera un escenario que utilizaría para datos reales, comenzaría con un módulo de déclencheur y lo último que haría sería activarlo. Después de activar un escenario, se ejecuta de forma predeterminada cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre la activación de escenarios, consulte [Activar o desactivar un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
