---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Crear un escenario de automatización de prácticas en  [!DNL Adobe Workfront Fusion]
description: En este artículo se describe cómo crear un escenario de automatización con Adobe Workfront Fusion. Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este ejemplo muestra el proceso de creación de un escenario que busca un proyecto y, a continuación, devuelve todas las tareas asociadas a dicho proyecto.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 8769ed5844e340e007f844370791e93393696819
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# Crear un escenario de automatización de prácticas en [!DNL Adobe Workfront Fusion]

Los escenarios de automatización automatizan los procesos de Workfront, incluida la manipulación y transformación de datos. Este artículo explica el proceso de creación de un escenario que busca un proyecto y, a continuación, devuelve todas las tareas asociadas a dicho proyecto.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para utilizar la funcionalidad de este artículo:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>plan de Adobe Workfront</td>  
      <td>Cualquiera</td>  
    </tr>  
    <tr>  
      <td>Licencia de Adobe Workfront</td>  
      <td>
        Nuevo: Estándar<br>
        O<br>
        Actual: Trabajo o superior
      </td>  
    </tr>  
    <tr>  
      <td>Licencia de Adobe Workfront Fusion</td>  
      <td> 
        Actual: No se requiere licencia de Workfront Fusion.<br>
        O<br>
        Heredado: cualquiera
      </td>  
    </tr>  
    <tr>  
      <td>Product</td>  
      <td> 
        Nuevo: Plan Select or Prime Workfront: su organización debe adquirir Adobe Workfront Fusion.<br>
        Plan Workfront definitivo: Workfront Fusion está incluido.<br>
        O<br>
        Actual: Su organización debe adquirir Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obtener información sobre [!DNL Adobe Workfront Fusion] licencias, consulte [[!DNL Adobe Workfront Fusion] licencias](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Crear un escenario de práctica de automatización

[!DNL Adobe Workfront Fusion] le ayuda a centrarse en tareas importantes mediante la automatización de las repetitivas. Crea escenarios que administran automáticamente los datos en varias aplicaciones y servicios.

Cada escenario consta de módulos que guían el modo en que los datos se procesan dentro de una aplicación o se transfieren entre diferentes aplicaciones y servicios. Por ejemplo, puede crear un escenario en Fusion para buscar automáticamente un proyecto de [!DNL Workfront] y enumerar sus tareas. De este modo, Fusion le ahorra tiempo y esfuerzo al gestionar las tareas rutinarias.

Este escenario de práctica lo llevará a través del proceso de creación de un escenario que busque un proyecto [!DNL Workfront] y devuelva las tareas del proyecto.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Antes de empezar

Cree un proyecto con tareas en Workfront que pueda usar para este ejercicio. No es necesario que realice ninguna configuración adicional aparte de agregar tareas al proyecto.

Para obtener información sobre cómo crear un proyecto en Workfront, consulte xxx.

### 1. Cree y asigne un nombre al escenario

1. Inicie sesión en su cuenta de [!DNL Workfront Fusion].
1. Haga clic en **[!UICONTROL Escenarios]** ![](assets/scenarios-icon.png) en el panel izquierdo.

   >[!NOTE]
   >
   >Si no ve el panel de navegación izquierdo o sus iconos, haga clic en el icono Menú ![Menú](assets/main-menu-icon-left-nav.png).

1. En el panel [!UICONTROL **Carpetas**], haga clic en el icono **[!UICONTROL Agregar carpeta]** ![](assets/add-folder-icon.png) y, a continuación, escriba un nombre como &quot;Escenarios de práctica&quot; para la primera carpeta.

1. Abra la carpeta y haga clic en **[!UICONTROL Crear un nuevo escenario]** en la esquina superior derecha de la página.

1. Para este ejercicio, selecciona la aplicación **[!DNL Adobe Workfront]** y luego haz clic en **Buscar** cerca de la parte inferior.


1. Seleccione el nombre del marcador de posición **[!UICONTROL New scenario]** en la esquina superior izquierda y, a continuación, escriba un nombre como &quot;Practice scenario 1&quot;.

   ![](assets/name-the-scenario.png)

1. Continuar con [Conecte el primer módulo](#2-connect-the-first-module) a continuación.

### 2. Conecte el primer módulo

Ahora necesita establecer una conexión autenticada con su cuenta de [!DNL Workfront]. Cada módulo que agregue a un escenario debe tener una conexión con su aplicación.

1. En el cuadro **[!DNL Workfront]**, en **[!UICONTROL Conexión]**, haga clic en **[!UICONTROL Agregar]**, escriba un nombre para la conexión, como &quot;Cuenta de Workfront de Olivia&quot;, y haga clic en **[!UICONTROL Continuar]**.
1. Autentique la conexión en la ventana que aparece.

   El proceso de autenticación de una conexión puede variar un poco entre aplicaciones. El siguiente proceso es específico de [!DNL Workfront], pero el proceso es similar al de muchas aplicaciones:

   1. Escriba su dominio [!DNL Workfront] y haga clic en **[!UICONTROL Continuar]**.
   1. Iniciar sesión en [!DNL Workfront].
   1. Examine el acceso que [!DNL Workfront Fusion] está solicitando y luego haga clic en **[!UICONTROL Permitir acceso]**.

   Si necesita ayuda, consulte [Información general sobre las conexiones](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Configurar el primer módulo

Después de conectar [!DNL Workfront Fusion] a su cuenta de [!DNL Workfront], puede especificar un proyecto de [!DNL Workfront] al que tenga acceso y los datos que desea que procese el primer módulo.

1. En el cuadro [!UICONTROL Tipo de registro], seleccione **[!UICONTROL Proyecto]**. Esto configura el módulo para que solo busque proyectos.

   >[!TIP]
   >
   >Puede encontrar **[!UICONTROL Proyecto]** en la lista si empieza a escribir la palabra &quot;[!UICONTROL proyecto]&quot;.

1. En el cuadro **[!UICONTROL Conjunto de resultados]**, seleccione **[!UICONTROL Primer registro coincidente]**. Esto configura el módulo para que devuelva únicamente el primer registro que encuentre que cumpla los criterios. Para este ejemplo, solo necesitamos devolver un registro.
1. En el área **[!UICONTROL Criterios de búsqueda]**, configuraremos un filtro para que devuelva el proyecto específico:

   | Campo | Acción |
   |--------|-------------|
   | Campos de criterios de búsqueda | Seleccione el campo en el que desea buscar los valores. Para este ejemplo, seleccione **[!UICONTROL Nombre]**. |
   | Criterios de búsqueda | En el primer menú desplegable, seleccione **[!UICONTROL Nombre]**. |
   | Operadores básicos | En la segunda lista desplegable, seleccione [!UICONTROL Contiene (sin distinción de mayúsculas y minúsculas)]. Esto permite que el módulo encuentre proyectos con las palabras elegidas en el nombre, aunque no introduzca el nombre completo o el nombre con mayúsculas o minúsculas incorrectas (como todas las mayúsculas). |
   | Cuadro de texto | Escriba una palabra o frase que sepa que está en el nombre del proyecto que está buscando. |

+++ Amplíe para ver un ejemplo en pantalla.
   ![](assets/search-name.png)
+++

1. En la lista **[!UICONTROL Resultados]**, seleccione los campos de los que desea que salga el módulo. Para este ejemplo, seleccione los campos **[!UICONTROL ID]** y **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Puede usar **Cmd+F** ([!DNL Mac] OS) o **Ctrl-F** ([!DNL Windows] OS) para buscar un campo rápidamente.

1. Haga clic en **[!UICONTROL Aceptar]**.

   >[!NOTE]
   >
   >Dado que no se trata de un módulo de déclencheur, no elige dónde iniciarlo. Al utilizar un módulo de déclencheur, ahora debe seleccionar dónde iniciarlo.
   >
   >
   >Para obtener más información, vea [Elegir dónde se inicia un módulo de déclencheur en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Haga clic con el botón secundario en el módulo, haga clic en **[!UICONTROL Cambiar nombre]**, escriba un nombre que describa lo que desea que haga el módulo (como &quot;Buscar proyecto&quot;) y, a continuación, haga clic en **[!UICONTROL Aceptar]**.

   El nombre aparece justo debajo del módulo. Debajo de eso, [!DNL Workfront Fusion] incluye una breve descripción del tipo de acción realizada por el módulo.

   ![](assets/module-renamed-wf.png)

1. Continúe con [Agregar y configurar el segundo módulo](#add-and-configure-the-second-module).

### 4. Añada y configure el segundo módulo

1. Haga clic en el círculo parcial a la derecha del del del módulo para **[!UICONTROL agregar otro módulo]**.
1. Seleccione [!DNL Workfront] de la lista de aplicaciones y después elija el módulo de búsqueda **[!UICONTROL Leer registros relacionados]**.
1. En el cuadro **[!UICONTROL Conexión]**, seleccione la conexión que creó para el módulo anterior. Debe asegurarse de que este módulo utiliza la misma conexión que el módulo anterior.
1. Haga clic en **[!UICONTROL Tipo de registro]** y, a continuación, seleccione **[!UICONTROL Proyecto]**, porque queremos leer registros relacionados con un proyecto.

   >[!TIP]
   >
   >Puedes encontrar **[!UICONTROL Proyecto]** en la lista si empiezas a escribir la palabra &quot;proyecto&quot;.

1. Haga clic en el campo **[!UICONTROL Identificador de registro principal]**. Este campo necesita el Workfront ID del proyecto desde el que desea devolver las tareas.

   Al hacer clic en el campo, se abre la lista de variables que puede utilizar en el campo **[!UICONTROL Id. de registro principal]** para identificar el proyecto en Workfront.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Haga clic en la variable **[!UICONTROL ID]** para agregarla al campo **[!UICONTROL Id. de registro principal]**. Esto permite que el ID devuelto por el primer módulo se utilice como identificador del proyecto con el que desea trabajar en el segundo módulo, lo que garantiza que las tareas devueltas pertenezcan a ese proyecto.
1. En el campo **[!UICONTROL Colecciones]**, seleccione **[!UICONTROL Tareas]**. Esto indica que el módulo debe devolver las tareas asociadas con el proyecto elegido.
1. En el campo **[!UICONTROL Resultados]**, seleccione **[!UICONTROL Id]** y **[!UICONTROL Nombre]**.
1. Haga clic en **[!UICONTROL Aceptar]**

   Ahora tiene un escenario de trabajo.

1. Asigne un nombre al segundo módulo, como &quot;Devolver tareas asociadas con el proyecto&quot; y, a continuación, continúe con [Probar el escenario](#test-the-scenario).

## Prueba del escenario

Antes de activar el escenario, es importante probarlo ejecutándolo al menos una vez y viendo los resultados. Esto le ayuda a comprender cómo fluyen los datos a través del escenario y a encontrar cualquier error.

Elegimos que se devolviera 1 proyecto, así como las tareas asociadas con dicho proyecto. Si ejecuta el escenario, eso es lo que debería suceder.

1. Haga clic en **[!UICONTROL Ejecutar una vez]** en la esquina inferior izquierda del editor de escenarios.
1. Una vez que el escenario termine de ejecutarse, haga clic en la burbuja situada encima del primer módulo.

   ![](assets/click-bubble.png)

   En el cuadro que aparece, puede ver información sobre el conjunto de datos que procesó el módulo, incluidos los datos reales extraídos del proyecto que devolvió el módulo.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Haga clic en la burbuja del inspector de ejecución situada encima del segundo módulo para ver la entrada de información y la salida, que es una recopilación de tareas incluidas en el proyecto.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Puede obtener más información sobre cómo leer la información de ejecución de escenarios en los siguientes artículos:

   * Para obtener información general, vea [Flujo de ejecución de escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Para obtener información acerca de los paquetes procesados, vea [Ejecución de escenarios, ciclos y fases en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. En [!DNL Workfront Fusion], haga clic en **[!UICONTROL Guardar]** ![](assets/save-icon.png) cerca de la esquina inferior izquierda para guardar su progreso en el escenario.

   >[!IMPORTANT]
   >
   >Guarde con frecuencia mientras perfecciona y prueba un escenario.

>[!TIP]
>
>Recomendamos la práctica opcional pero útil de agregar notas sobre cada módulo.
>
>1. Haga clic con el botón secundario en un módulo de [!DNL Workfront] y luego haga clic en **[!UICONTROL Agregar una nota]**.
>1. En la nota que se muestra, escriba una descripción general del módulo.
>
>    Puede agregar varias notas para un módulo.
>
>1. Cierre el área **[!UICONTROL Notas]**.
>
>     Después de agregar una nota a un escenario, aparece un punto naranja en el icono **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) en la parte inferior del editor de escenarios.
>
>1. Haga clic en el icono **[!UICONTROL Notas]** ![](assets/notes-icon-w-dot.png) para ver sus notas.
>

## Activación del escenario

Este escenario de ejemplo no tiene un módulo de déclencheur. Si este fuera un escenario que usaría para datos reales, empezaría con un módulo de déclencheur y lo último que haría es activarlo. Después de activar un escenario, de forma predeterminada, se ejecuta cada 15 minutos. Puede cambiar esto definiendo cuándo y con qué frecuencia desea que se ejecute.

Para obtener más información sobre cómo activar escenarios, consulte [Activar o desactivar un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Para obtener información sobre las programaciones, consulte [Programar un escenario en [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
